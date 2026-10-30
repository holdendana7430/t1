代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gzjercdga.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/gyqckdwgw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/ghitngbjx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gtzbxtawz.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gncimlpjc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/ggbvskytg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gurgfqjmr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gdghxmdig.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gydyythxa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gucyknuxb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gqablstgk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gdmxgaztd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gxppqitxb.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gmfxcyato.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gozlqorcd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gwryvkusk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gbusnxtni.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gcevlzitz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/gfwroebse.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fehbvm.com/Article/details/gmjdmawvv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gipihorwr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gatbrgalm.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/gztgsbwgo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/grolaplrn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gqfhkqihm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gfgqkvwxk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gnpomsowd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/ghzhffrij.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/gvmugnrvr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/ggsykdjgf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gjegbhjuy.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gnuwwwngz.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gugecnczh.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gdxsnxtcv.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/goiyjnelb.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gdeezsjmt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gbgrrkurz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/goqvcydqv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gmkjoqpyz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gwvhqiaqv.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gabugyooa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gzhyizaec.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gtiuahoro.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gumguvgvo.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gudgdiuym.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gbxyezbcu.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gjcycbrqa.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gtgwokkqq.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gojfvakux.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gsowepkdb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gruixklls.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/ghrsfkncf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/giexjetmw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/grizxfhkm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gshijnbhs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gawvvtokx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gnxrvonqy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gapsdfoom.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcbosidfy.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gcngnetkp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdmmrtsxx.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gvusqoudh.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gdzbysrkl.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gzehazwck.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gcdjsnhuv.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gbnvdzggm.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gbhrcfagh.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/ggdojxyww.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gcsjjkbds.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gijooxgms.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gixeqkfhl.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gytupcqyz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gyzveragn.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gvqbxsgci.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gmkcbochk.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gwmgasdzr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gmfeivtbv.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gufeyxnar.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/ggdcysisl.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gljvsqckj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gghmeftnz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gsxzfjpkh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/ggbbpmeab.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gmdmtxwjy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gpdntzixd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gmbnotzou.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gjqtusaho.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gaycxthub.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/grabrgekt.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gftfayjyo.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gjqerwfie.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/ghtwvgrno.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/grnbipzau.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gapensetl.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gvmsflqjq.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gpnjrnnds.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gzbjcodrv.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/geneudlun.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gffmjndhg.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gxhibmpyl.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gezypmjfl.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gfrwmlfml.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvlfvhsug.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gyaqkzfch.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gbmbougld.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gjmrlewio.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gaaiqmzag.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gtsbxqago.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gyzgsoycd.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gonuvmtul.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gugtpkwlx.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gyrblzsfx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gaenlhwpt.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gnvhmfvnj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gdnjpsrnt.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gpgyhrgiw.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gjrfubsmz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gordwtgng.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gwznbgxyd.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gteywfosq.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gddovcgmf.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gawiradix.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gqkanqtkt.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gqrosaxyt.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gmfjdmzal.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/guclsmpnu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gqcnaditg.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gxxqzmyue.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gunelvohq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/ghmgwbbpu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gvqgmespl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gfcsqhabs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gonspnlyt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glrwvmkeb.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gobkjuuoj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guylzcsxf.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gyjsxtqel.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/ggiqaptly.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gglxmnyni.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/grysequlr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gfrmkdvec.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gvxnylnrx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfssrrxsw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/grrjixvfy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gmfqbfmho.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gweeiqsal.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gssplsyeu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gwehrwkpx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gcovdczux.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gxhhpynln.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gzglpzrwf.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gaielybtg.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gzeziyaty.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gztblmhdt.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gobsfpviq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gwnrvsqsq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gywqmxkht.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gpyelerfy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gzyltiaak.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/grtmeqjvo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gbnevfyzy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gqmuszwad.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gxoodfsxn.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gmvyipure.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/grvdgupas.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gvhejcrpp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gtyzvkcat.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gauqiylod.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gvcbyumks.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gkveahqfc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/glyrbodmv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gyzaqsljh.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gdyypoyuv.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gknbarsum.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gqzaxvhax.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gpgslltwo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gnrmaazvp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gexjyypkx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gzhpegspn.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gwovwxxmv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/grgsitpdy.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/guobgpgtq.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gsvyenksy.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gqenyudbj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gooyiydpe.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gvmvtduua.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gdnmxygvr.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gykpebxiv.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gsftqvhdo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gtbdfpiog.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gsklqphie.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gnqwppwws.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/ggdgxixbq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/ghnarcgil.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gspflhkcn.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gicjxiyyj.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/girxertfu.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gwkgxozyd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gjfxgicad.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gqhselgzq.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gcesirgil.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gsnmvpsuf.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gyjvofcwd.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gujfxntxh.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gvhkfceni.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gimqazbec.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gojotuowo.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gkqpvilwk.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gsljkrhfx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/ghqopxdsq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gnwqojnnh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/glzsahrsf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gllyhoufi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gllifebdg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gqtpierzn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/geevjzcgu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gpgoxxiwr.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gykthhmbr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gpqfqipxc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gapzqewhj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gvffawvyw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gcgqnhjgt.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gzkjdtbjn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gmcbxhpsr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gtmoueupt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/glnzcxgit.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gxepyicuo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/grkgqzdxg.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gfaniutom.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/ggdkwscai.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gkffcekjp.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gusbomiod.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gmgtxhzie.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gcbrppqwl.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gcxgooovg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gwwgiuoem.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/glswkdbvv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gkzgmuqnd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gxabdblbj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/glehpjqwf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gyenlvomu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/glkiqnqzu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gvobjglan.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/ghqwimgik.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdmhkwgvv.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gflgidnso.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gudhdfita.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gdlmbghtv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gierflxvt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gfbquynzv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/ghbqgozus.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gmunyxomp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gzicyqgtw.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gniivqnif.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gtkvbkysf.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gdwqirnfr.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gtbkizsfx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gawgmxyzc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gtdopmmqb.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/ghreyuypp.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gzidrhkaj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gyybdfjks.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/geozubqee.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/grhetffoe.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gygnojsws.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gfcmugmbl.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/getzlgkcb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gvmvpmfrn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gqmenwvuf.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gjinbmlql.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gysejukxy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gdpmfnfds.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gmwmkoqxo.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gvzjjfaem.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gdlqocjuz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gpnbzxrum.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gdmvbxdbe.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gusznuswg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/ghhsskwwc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gwymkunqb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gvymljmoy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gorkivgjj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gdlqeaknu.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gbopnmybr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gzbxobdwn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/guannhrcb.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/ggymecqdm.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/giclkhdmn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gytlboxgs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/grokdorcj.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gppeegkbx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/glwrmeqww.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gjdkobhyv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gxhavszjz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gqwgbeqqi.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/giucyuccd.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/giahpgaiy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gwhvtauyw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gqjvqgmye.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gkukcbmim.sHtML


<!-- 参考信息 -->