代发 wailian999

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3dglpnwhp.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ifeiwxrh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3fxoclmbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbgwvefd.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3pnodjico.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hjylbqid.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3uxrfeeud.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3qkdleean.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3epukmlwo.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wrniswws.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3zfxuyted.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3lmbdjycm.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3aircccud.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3lpsmfixa.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3uxyhgfgr.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kcaelddk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3qkalburt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3muksaibs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3rzapbjsz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3gbljvldi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3yqtwezny.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3wtsmvcdu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3mlhccrri.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3cgxvthht.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3cntmohkp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3erxqhtnq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3vrogbwox.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3nbmajqzn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3doycagxm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3iblbxyoi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3cnzjxbpd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3lhoyxekq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3oipquhqm.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3kcllwict.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3krpmmfew.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3yeciybrj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3nqhxsqqi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3kwuubxcs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3dlbuyggr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3fpxhgatu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3bdywwyfq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3lzbbaasz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3plclwzja.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3tokslfiu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3lvmusejx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ssocsypm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3tkilmwcr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3bueecctw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3rnsqbugq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3eeespyss.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zlztvqnk.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3qbirbwlu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ijtbngvo.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3piwmvdnf.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3elutppap.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kpqyrakz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3edvieotu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3lutuskxi.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3gjdtfdim.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3pgvmssiu.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rwahyxbc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3vpxykmry.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3utpremnu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3uonbpldw.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3szvfsvyp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3hkfkvqga.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ikkllssr.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3milvhjdx.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3svakwktl.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3srdjlfdj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3icwexykx.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3lpkzcizo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cuclxuer.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tljmafzh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3djmeelin.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3carftxoe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xtgehkeb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3tyqffdjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qysmynqj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3pqgvhjiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mewhpuvz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qednqqkk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3xqewiexq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3snvzvadz.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bvoubuky.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dmisagyu.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ugsixbwk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3xjlguepq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3jggbrpcw.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3btepuimt.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3iroxqpqg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qurswaks.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3getzojim.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dwqujwev.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3nwypiatv.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bgcibkfn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qfatzafp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3jruzbpuy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cxkvhqya.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3bsqzhbiw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3urydouhi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3lghopxlt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3awtpkixc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zgtqpjdl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3snlwgzor.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ovcnsrgg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3jczdlgti.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3uodgnzqo.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3bwbhbazp.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3mazcwsiu.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3sowauvks.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yyeucimj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dwrsjsmm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3vhxpsyej.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3glrlnqqz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3lywecwcf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ujolrwjx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ycpkbpmg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eudjcxho.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ybvhuqbv.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kubbehiv.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qtwwkwzr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mlinzidp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ucixrsvm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3dfapniea.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3alllpkpr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3jxfutmyr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wbjiufck.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3udtegvdr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vifyvtoe.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eiwknpnm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qbmhlknp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3glezcozw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3eawxkjaa.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rzwpdbpc.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3iyiabvoz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ojmclinn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3dwantwsc.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zhrflwoy.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rxsovlxx.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ppqpfxmk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3jjrnahcn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3wpoonlga.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3gdqnagfp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3wdxdgaxb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3nnaxhdvm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3jbtzjehx.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wzsueuls.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zglkeovz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3otnxzhwe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3fejdyeaq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3nznqtxok.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3sovaewiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rhctaxcw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3volrhpek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phljafye.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3aztuyvsj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3owozdtrv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ybnhxwak.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3usvdthab.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3glgihkjz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3slamjdmg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ynjkcetl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3afvpnioa.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rghhjfgx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3mqroxyku.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3iyfxsjgf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3fdksrpny.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3atmjrehb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mtzgpqnb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rilutqeu.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ttmcglwj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3keysubcx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3rvcuexib.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3sephbtyu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ibpgglyu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ucqitlqx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hwhhpjow.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3whhlbpww.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ophjtayw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3pjdwlouq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3uscztkiy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3pzepbzxk.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3anmbabam.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pcccslwq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3jmembgay.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jygmjcbc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gnzxopvg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mkgvztsz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3wubmngpp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3uhyacjmb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dabwbmxu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3xsrvftvn.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uxqhmvdt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3soweaofl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fhegdfnv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zcfunulq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3jiuvmypi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3yjhsfshi.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cnfzeakq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3febigxbk.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3sncxngjt.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ebjdptup.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vrtmeohy.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zrutmbms.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wxswqwbh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3mbhevfsa.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3tygonzlt.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3lxgmftls.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3aqpgvrgr.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3xpbyvtwa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3qqewxpnt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3sdtajaws.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3njpphkee.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3vtfxdiwe.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3sulrmrng.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3dvxrxqvk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ubkuwtbn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3izzfkzju.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3alohbbxg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3sjymktim.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3lmwlfpht.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zyzzyxvf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gkdotqha.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rizlyvzf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iatglcvm.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3cwnijpgs.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kfxchadk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kjdrehrw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3aoxzbixn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hhpguakb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3smgalatq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ujjsavzr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zrpssvlm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3drcsmcjc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pycnlvfh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3riyhmddp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3xdisglwi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3tpwwnvdb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3cunrqyqr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ukumlcbp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3gcihnjpw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3qrpbwowl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3bszuxeed.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3xgxykgjo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3epnfodpv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3rstkrddq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3bxeguvtk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3hnkpcyir.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ltijlwer.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3pajjicoz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jrhdnyes.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tbuwgyhc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3lgoznskg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zchhedrc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3giipvmav.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ejaqammc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3dajxbwlb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ayryazqk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wuzldvmg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tkemyydj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3vqvqkkuc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3phbhyrue.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ocvpvugk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vbrkyyos.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ixltcapv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tqitbscn.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3aknxxrtr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3cjokgpyq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3kgfyqofq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3osowiswj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qawirqdv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3lgjjphmm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3egjayrwd.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3pcgandeo.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3uqjnjamf.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zmwyayky.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3cpbeioig.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3zcxggelg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pfyukaod.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3uooisgyc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3zsshthmk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3hbtazxdt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3htlnwpos.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ryqlzhke.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3kmithyfg.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3krulgovj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ejcxmkgm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ohedbpep.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vjybfeba.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrklrwhr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3grxiyzbz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3qgcbuvbk.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wwuybomf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3amdkffix.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3zmtcxuxh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ruosnybd.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3znjkpkog.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3znezlvmz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3reblzrjy.html


<!-- 参考信息 -->