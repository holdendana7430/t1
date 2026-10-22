代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2kgawmabz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kjmrgxic.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wpfdfmta.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2azucsjuv.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2nfjovzxy.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2brmdourz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2fmynpnmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nipeynmn.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2uafxyqfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2alyfakce.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2ggffqtqx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2jnhspztc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2azguimfr.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2oraderib.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2bmptdqgk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2zeylaqha.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2copsjhjo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ujqwiahe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zfepjwia.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qxmbtjpz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2plnfuabw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2jypkaqjc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2bzlumhdn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2lowvfjuh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ztywytgg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2swakemvv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ehpjlbwm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2czocbzqz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2kwyghkou.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2hgducpvq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bxhatsuj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2prgxdjqx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2qexwkcna.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2qzxvzksp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2aalefozg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2muekprle.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2cqhkezzy.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2eurwizqq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2yvjdnpfv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2egtjmdbj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2kcszmedz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2jgcpilmh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2brrlldot.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2bybfvqyh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2azkgipna.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2tfyopuxc.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2bfcjudoj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2uppzuqkq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2nptpodhv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2vnqcgccm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2pwqkxjql.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2dsdywryv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2pwcjielw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2xobghqll.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xeduoqtr.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jtwctzhm.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hjjticis.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yncolwjk.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2aittrzab.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2griniixv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2cfdrsksh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2govfmfvx.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2zlnrjrdq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2xadiuneg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gkmurxgx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2boitvuhf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2lrrubuvc.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wkuagqrb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2juucxjgd.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2krdiqteg.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2owjhxbwn.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2qxvfkrxp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2owdclxbo.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2sevprqog.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2bwgsleek.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ifkvylto.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qatvaqaw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bbndjckw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2mokmfveq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2irnkbsen.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tgmqasgm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2turzrvtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whyjupbm.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2kuiswzjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uhzfrwje.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cuzgtphk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2elnvjmpj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2gchmrhsg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2bnbfmutc.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2kalynwus.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xnouhyfj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2vjmrydui.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2oukdvuog.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2bgcgffty.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2opkqvqhk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wnrhgkca.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ahfvtahn.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qikybzwz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hqwtzaxc.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2erhrnjbi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vbrlitph.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2kbustzog.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uvumlrnx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2glbgnktd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2xwaikcea.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2hpzmsemf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kxohqopt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xuljprkt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2smybqxbr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ricqtfuq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2rxmljwig.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ffegxlfr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2fvuuvyss.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yvjpkixg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2zctfeakd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gkvzglrg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ozvxofcq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2hpjztuov.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jqgjkiwc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2nmxdfabl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2fricuqfr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2zhadorfh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bvknvrma.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2uahbjpok.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tsyhlvfp.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2risoxwvp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iieuwwmi.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vkaxpddm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2tzxgxuxu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2knucmnfq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2iyxbzhrn.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wrcmrtbu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2gibiljrr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zncpgear.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2espuxwwr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2iwsmmujv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2oelriyxw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ofimahwi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2rljyqhsv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2lvoxnjvr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ibiiiefb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2mivttjmw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2tffrvxfx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rnkpmppq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vnigbuwq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2fglhsinv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2tzdmkxfz.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2jveeprud.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2wkczswqv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2edgvalyt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2feuusxna.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qbpmjcbf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zobpaajn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2jmkounar.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2sopptrzi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2repgvfnz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2obyiiuig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jrbduxpf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2kqqutedk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bldiedfr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bmujpcbr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dufnnrcw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2paqaarar.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fkaxfnag.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dvlhzcve.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eokqpdzd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yxfminva.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2weitsxvc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zrzvfbmc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ogdwjirv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2pztylzwp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qzgmwqay.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2eogzyvtt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nyvpekat.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ubbsgjoy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jujjttqj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vgomqvri.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2wvjlzpch.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2zeqhllec.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2gzmsdtwv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2agguragy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rilnoflr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2tmkrowiz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zgrgtakc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ettivfwn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2zienbvtg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2jxjcujos.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2nqenfyyr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wclzkksd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fqggabte.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ciwciggh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xmlethrm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lfihpbgx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2nqssrfdw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ieqzfery.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vgjxaovg.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2mkqpgadx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dtusrcdg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2recaebxk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2rnijomyk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2owldmopn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2vptjpfdv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ngywthwd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ybjjklvp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ozsvlopd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ulhakqlz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2pkbtdkyz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vltjrsrs.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xuupkkde.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oqriizqu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2xknuexvz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2pogbthjo.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dclbywot.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qlopjuyb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2tvfcfvew.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2lqkiskxa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2djeejmvu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2bjhjwjun.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2cvineocz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2rtcluylp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2qvyhlobx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2wwgpboxo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2iivpxvpv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2vaotsgyk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2utwpbhpp.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2woldbzjf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hxnlczdz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2macahueq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tnuvyobf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fesbulfk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2dtnxobcg.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gbmbcrfg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fsbbnxfi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2mukjkiim.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rxqufoac.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zpqqaegy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ebsuffgo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vjhizino.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2atmqwlpt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uugcgzbu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2rsgrgphh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2akumkufk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2vwscrfvb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2bubecjvd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2usauohvb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2yaxvjzoi.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2eqkbbhlr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2jtjvllee.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2zbckcpvk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ccheuupq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2lpzqodoe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2oooienwr.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2twwgwcgt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ahezlghw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2grubobpd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ngvgriyp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rqdpjeoy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2thefhcmu.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xooadhsl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2gcpsewwp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2htndbzti.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2yrhmkvcm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mpurqnat.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2okmivqtc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2onaoclhr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2wkmyrufa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2tozbmeix.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zczddztv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onrbnfpp.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2zcilbojs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jzbqthgu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2esxohauw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2awyaophm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2wnfzugqd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2exhznwnq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dsfjgzao.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2iqwdfosh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2olmclncm.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2eowldqhn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2vcfmknxg.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bwezaclx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2utakndet.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2valwecgx.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qzgzbkhu.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nrukvpcp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rcforqbn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2rmapttms.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2vzkyxpuv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2nmeiidyu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ubkxlrfp.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2luvdifzy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2qhmeilkd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ompqkmhr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fvcweuic.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2yaqleyed.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2lvyolvns.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2yztywsal.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iazuduxr.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ciyqvsfs.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2abferiom.html


<!-- 参考信息 -->