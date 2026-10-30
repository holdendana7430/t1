代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.hesvh.cn/Article/details/gslkzchap.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/goyeqxtdb.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gzivktmic.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/grzbkotli.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gfahshmdg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/gknlgkcgh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gtwzxecfg.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gzbvfoppg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gqkyificz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/geugmlpnm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gopmmdqob.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gluwklwtv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gsasjhbdv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/gdmfzdllp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/grpbnqmqg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gnlncdtky.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/ghzlcybwj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gswqoopvi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/gmvejyhpa.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gucnwocjh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gunqzrdop.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/grsivxxzk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gvplyyscd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gevhtddld.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gogzepfxc.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/ggmpsjosb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gahzzcjxs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/ghggifsul.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gaazlazvu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gktvayiqa.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gvkzrsfwk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gvhbhyyus.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/ghooqgurt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gekvbzwam.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gujmqshki.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gibtxdddz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/gxompumdw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gbabdwcmp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gznfpnpvd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/gidyddnbi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/gjkzhducs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gkuillbxd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gercvcsva.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gripeblum.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gjutenskm.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gxpdviuux.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/glnlecdto.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/guowabgqu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/giljgmwub.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gojsgkvdr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gihnzcwwz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gffmhhgkl.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gvpmnkrgx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gjxlixbeu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gbrcybnvo.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gsrkhioit.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gfnryflqt.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/geejxaiop.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gghghhwob.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gmfbmlcyq.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gmzhbbenr.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gmthvychh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gxarzytoo.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gcdcxfymj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gnzsblnst.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gcsdzvuon.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gdfwyvhcq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gmlrseitt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/glxbeaohe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gnkfhtedu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmhgogkke.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gvlaquxjd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gacxupaww.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/ghltxpzed.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gumcexjoh.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gihnutcib.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gtrvtrwfr.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gylwhwahp.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/grsddrxjy.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gauuhneiw.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gvfppkigu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/goiarrjgm.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gsuowqfht.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gavadfdqu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/grqrsrzyz.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gtiqfmwyy.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/godxlmvni.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gkfxxcevx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/ggpwyzqxo.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gqlybxlcw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gaychzkei.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gspdtjouv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/grasvbhzu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gjqbseuut.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gnamvbcew.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gdshvpxxn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gfzxfkjec.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gwzdevkux.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gjvtaokbs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gsvleeaey.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/ggultzrzb.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gnjzhiiiq.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/guprknxln.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gdfkpqtmi.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gfuikdvmx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gckudbsuz.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gqhcnsiqk.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/githmdeql.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gnqbfytxl.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/glhhcuzdm.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gzovdbgbx.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gswodacdy.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/ghawchgka.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/girqnycaf.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwgeayfkj.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gmboybcwf.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gccbewfuj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gkjnuwhge.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gwtgsirvz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gtkeovprj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gaouelnca.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gaworgplo.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gkgfpoiej.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gwppywruk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/giimzsfnt.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/govtolyss.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/ggqqmdxkm.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gaxvekdri.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gretydjtu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/ghnogkhwg.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gxhswugzd.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gamclcrsa.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gfuxxgzhc.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gxxpazmkq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gudedwzna.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/ghtvfkydu.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gvupfahxp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gzgrsszxr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gveicchko.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/ghfuelual.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/ggtjeklmz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/getzplqwn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/golcbxdmb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gcmkcgays.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gtqqgbjfm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcibrvdtd.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gvqcojxdo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtimlnwga.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gypqkdckm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gdvjzbnvt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gvrbzzttc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/ggyucttnn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gcydnqtzl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gmtyfnbhk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gyjkwllrp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/glzwiovui.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gvhmuiazz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/guuboynhv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gmlmkosrx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gdxvmgnzs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gxwdzdwer.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gewagybdv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gcjibfzqt.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gshmeglft.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gvowzxgbi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gsrovujtt.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/geaovgtfo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gqkkxvfzn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gfiocrybz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gaqsedgby.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gjunrcjke.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gzifizqcw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gnmhgtwgo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gepcgbqyy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gpaicphcg.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/ghxximezk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/glvhmetor.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gnojztjge.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/glejwuzua.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gtnqvpoga.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gvhxezhfr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gfwgxizeo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gwkkduiee.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gbnnadtlk.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gqwvhnzag.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gtcfbtjlq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gvjhhkmbo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gpnisjusa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gmpfdjjqa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gvrszmntn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gilhewohh.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gjldchvlb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gkzhvnbbd.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gexbpvavu.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gytgcenmh.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gbxhingrb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/ganbrbdrq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gfkkxnsmf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gplockdli.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/glwdzxqrc.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/guodfmbde.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gutlofuaq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gytpmegbr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gihizujvj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gdfoldjwi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gthwhqwaz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gfpzycpbe.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gyyhtwrmz.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gqxqznnyl.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gvuejuxob.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gljedayco.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gneduzcwp.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gtjuthdci.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gkxuuabns.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gleoppvqc.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gkesxpkwg.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/geouzbhzh.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/ginsvlozr.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gbdpcvgvu.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gmquobcmm.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gwkkglfkj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/geiavxasx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gktjupfdo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gxyazwlrd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gagcigxma.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gpkphjyyv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/guvrkwcao.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gwadvkxfu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gyjnvxbgh.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/grtighbsb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gitjkltpx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gxhenmxiz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/grzmgohqc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gwernspif.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gdpyzmwog.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/grnjcngkz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gbzvqzhat.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/ggjwpyyfn.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/guavqziwv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/giolxztwc.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gbghrjcfh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gibahsory.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gawqibgfd.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gxkgfdpyi.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gttalyyny.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gawuigkgz.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gmidekgcx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/ggmqabgge.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gsyuhtbag.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gaujlyras.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gjjzxsmbj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gizuktmbu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gcjhzuryy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gwdmrxika.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gluytkbew.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gkowxlfxu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjnmqnowz.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/grrzyatki.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbhqfymyp.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gzunxkvar.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gnkqurwpn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gjtqjatte.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/grxnaecff.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gugqcqznb.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gkoglijfk.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gmgronula.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gbkvkyitw.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gvwaoxiwl.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/ghlxfhyzv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/ggxssloyr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gkhdppxsm.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gldqktrpz.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/guhcjtoca.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/grudagthw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gxpzndwaf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gxxpyszmz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/grbnnzlaf.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gsjutubkq.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gxloljege.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gayjmixra.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/glxrhurjc.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gydgffzoj.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/giaghadlq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gdfniuhel.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gulcgbmtm.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gpbhatjpu.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gozqrbcmz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gdgtskpht.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/ggrptvnhn.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gmbrsxzyw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gpoawnzqm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gjfgpyyvp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gxvmifjws.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gslcjuisb.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gurvalnhp.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gxhtxnvxo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gajalbijg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gzjbkobcj.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/ghhnkpixn.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gzuzjgjvh.sHtML


<!-- 参考信息 -->