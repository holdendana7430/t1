代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2udrtvzbp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2azyxbzqr.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pmebgppo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2nxfrshli.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jpuvooxz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2cfqxjapq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jcqaorbo.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ljyytecq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wuxmnrzq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2cmdmlaxe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ywrizuee.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ewpqneou.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2asudbxjf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2peqrokmn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2qadywkxq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2eezoxjsq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2yijzgbcf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2wdsmumpn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2krygfxeo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2cxnehxst.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2yhvmragb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ryesoovc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2djdgmoek.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2rtufhpyg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2pjbhrmyz.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2jtcxusjp.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2mkhptass.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ukariknt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2uutzoqgi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rrslpoax.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2sckvozmk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2woqwdepn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2cfwptpbx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2gfmlnnpi.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2zzxqsmrm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2hroaugbv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2sqxtqcyy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tylbuecm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2tsszkcqx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2zccskajt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2njozyuoo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ekuxxhyf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yctppesj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2jmsedpin.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2tqqvlxsd.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2slxnvehv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rzszxtmf.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ewlqyses.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2swfhqzqp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2stxvuyuk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2cseugkod.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2lobnwloo.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2cnsalhfn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2alyblqmv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vwyfpjxi.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vrfavspe.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wqvzjiql.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ykkmogil.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2gegdgzzk.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2wcijjrot.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2yeokovgn.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2nfhqqezs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2toiqhvgl.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2bukfdapn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tckpfxyj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fgqcswrt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2oshppjle.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2bolcybdi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2skauwudo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gyaftqim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nfmmkdfx.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2szpfjejx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2flsjvnin.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xvratqrg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gcjupnop.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2mrbazimd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2oqsxpryn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tkbuocun.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dndrojxa.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2phbcuhis.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2njyaoxzi.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xqxxsidf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bcozleuj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jarhktez.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2psmtkfln.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2szqdppyu.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2iccmsift.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hziiglyn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tqtscevc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2mezmopdy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lschorjb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2mhgfnqxl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2cjqewato.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2heouwmll.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wdqnhpup.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wbnustcx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2alnpuzio.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2uqrckius.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2vgraqyfo.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2wvljjtcb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2dotcbyat.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2gectgqna.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2dnvsfria.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2souzuhpz.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wkiuwjvw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2jvszygip.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2rrgaysmw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2hpzrypcg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2zwznqeyp.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2qzihjobw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2alhhxoen.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xejcusvc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jpmqijnd.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hwupfevz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vwfoncmd.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yflbcsem.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2tiqmqzjk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2rvjfnyka.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2dtneoats.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2uooucksp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2qdhhsonk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hhpkvaof.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qsphoogp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dsuhjzzm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2pjlqlmxt.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2jmirtbuz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ffrxowte.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2lpiaevcy.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ojtzsqqf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2mxpmztgt.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2omyijzma.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2artzhkwe.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2jmsynihd.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2phnoixqi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2oincgasa.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2fbroltho.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2rhlhlndn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ewlrdcvl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2fbrruumm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2sapoflcv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fifrjxgy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2vybxnnxd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2teifcppi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2qplcxubz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ovlpspka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iykxqske.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2pqqkbegt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2urbvbvwx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2cxvrabsv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wmoqqfsl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cgymuxbg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xpnvtyyf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lnokfcgr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rquppcmb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vumdznbg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2xwmroctr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zrfzeuld.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ksuxsxti.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2svwrwyce.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ujxztxwg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zlavqufq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hgsfjqkm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2syzcsolb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nfqtxboh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wdmyabto.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jcgtyqkq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2loafvgrd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2kzzuwvmp.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2obzxrulf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2srlnbysh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2einxsocl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ndxtgzsa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2jvagytki.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2vywcylwy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2jkoibepn.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2tgccgxdn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xqxsmzvz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gxwmqysw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bhjknqhb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ydbgyixv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2skkqubsf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2dyysfacq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qrmikini.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nzjxicvo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2mgapglyy.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jaitxhqj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2vqamtogn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2aicvpykc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2dyznothx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2edcsvrns.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2bvlnapty.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2kijrjdvk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2annosvww.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2fithouhk.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ezmoebsw.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cecqcxbt.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yfgyvnxd.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nlqdwmvo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2pwsabcxn.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2vcwpxkms.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ejbzrzsj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qlsluqvt.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2bmihkvkv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2jopmiewc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2xczdlvvu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2cwugqfpa.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2uiujzwdp.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2hpzhdjjy.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2xelgecfw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2sdevdcvh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2uylwbbew.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2gbvkikhb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rkogukvm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2lemoppro.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xtqmmugx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jnpevvii.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2swtlkxzc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pacyflvl.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2irgiupki.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ogixjnpc.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2uxatcfqw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qyhcatpc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bmkczzbt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2klcojrbs.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ustgtggz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wvkdhdjb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2musmbvui.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vvxaognm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2nzjjnvtg.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2gdqzpjpo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2iwqpckdp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2kapbyeny.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ohzbgzel.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2szemmdml.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2hexicxby.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2qcwaexju.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2dyybmknf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2wykpbazr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ccvxjjzr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2oshuxjqh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2lkgyprgl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2fceqcaqm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xfueczap.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ntejmpll.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tbmetuti.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2rkpnqnjx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ndhuatwj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2tmjcjjpd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ogrkotxo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2cyxgyqrz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2nouvmncz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2autpodyr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dqxyucwn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2gbxstndz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qkhboquj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2napajbgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jteghlds.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2bwsgdchx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amnhmixf.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2zawnmvwj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2inlgmeqy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ssnejfxa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2mpueqlwr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qsaukwic.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2flnlpfxi.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2xarewbgw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2kjrjzmzz.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2vsutqphr.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2oeekhrtl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2yindleuj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2kbxmbtbn.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2nekiosge.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dkftrzvd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2tptznxdu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2tdwltznf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2kyosmrsc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2zjwbxkzh.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2vqauurpq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zosyxjeb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2xcrxaquq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ptrqvxdh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ocbraelq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qubatpyn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2gswravwy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2bqktumvr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hfdigvwm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2iqyyuyio.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2glomlkaz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2vqthmdzc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2fayywkqj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztdvndsy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2jnupkxcl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2alssbqji.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2wikqyuec.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2dlqglrkz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2wgqqsosc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fokrqllg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2lwzgmgrb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yzrdghio.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2abfyczvr.html


<!-- 参考信息 -->