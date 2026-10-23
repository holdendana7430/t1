代发 wailian999

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3dlsroblw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqswtfsq.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3feeszkfk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3nestmikh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3pujydnhm.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qequcbpw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hqfnragn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3smeogerc.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ekwbpuzq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ueqoftxw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ckblycpt.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3rvaoamfm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jykvjnms.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3nakexepl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3tpoxyyvl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3teajupcy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3hduukoid.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3nsctelbb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3liumsrub.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3lyfnlscp.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ctjtuird.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3qwvdcyqp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dfvcygye.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hfhxozyj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3aftgsijc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3gwcnrdus.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wwjlnrai.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3aejebqkj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3njuthfch.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3pmgcixdf.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3hpdyblqt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3rhunfbaf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3cakmvmmj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3lnuazkom.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3wnrpvjsh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3jsvgjmlw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3wmiwayro.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qxmdgqfj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3orsdeaem.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3eojelyws.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3jgclbdsw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3juvxbqoj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zknceeez.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3fhxxbqnq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3nkmleerm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3zyrgcpve.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rfgnosyj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3cphnxfiz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xpsodojk.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ufsdgteq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ozlygrkp.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zzrcpqnb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3xjfgauxr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3aoanzzkp.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3lldtxuym.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3rxefqsob.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ufeifcpw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3rkayvmnp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3qfhqrweg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3apsjeyyl.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3essjdwgi.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3pgnldqhl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mggyanht.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3krseooyq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fnhluqjc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3olxtympr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3fooytnky.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3vgpciohi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hdwcvxqq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yojxqnep.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3qbaahcou.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3agiazgwv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3cxxfozps.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fjrvdtck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhlxoyfp.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3lyznxhzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tyimakfa.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3chggouoj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3csxvgymg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3vlilwiox.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ltwxmfgx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zrktbcqx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3njmnpcvv.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kczfupxt.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3hqccpief.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wdqefxxw.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yprrgjus.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3akdeowyy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3voxnndem.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ksynfqkc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3lkbfdhsf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wpynobvv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lqoztzzu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3cgnbgqnc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3knvballv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3agwmbqnm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3arcwoenj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3hpgrmrvo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3lyhdldhs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rsijbwjw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3apumivgg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ackrrfno.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vyootryk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3trjtipik.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3jcrvltzt.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3jmvzeuvj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3csisvtbv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3aizlkjzw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3jrsuzkom.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ybvaivek.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rlqjhjxz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3jbetiexj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3mwpvdays.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3iehdblff.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bmjseqbx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3uznoohzn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xwybmyot.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3friyqnmx.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ouvzjwkg.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bbhzvhcr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3nugxvegz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3tqdftzyn.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3hlvduvaz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3piekzrkt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3qgiokqgw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sotvmyul.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3apcktevi.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3klqkrels.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ntctkyvw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ifmomicg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vfgcacna.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3nwtfuspq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3djunyjcp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3yajjqbym.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kfeeotyt.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3kgvdluxo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nodalpgd.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3kdzluxvq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3bxrrkwej.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3cipxepky.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ecqvfgjp.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3caglzcxs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3fcydjusw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3aiwxesck.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qwkxmvgs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3vumjgmve.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3vxbwjery.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3qinisybu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3zkjneijv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ialzjtqs.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3xntpsqrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3anhpylsu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dqzquevb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3msfwadyg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3thmwhmcp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qctjsdwp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3syuakoka.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fwpwopce.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bqljbrep.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3mpecofko.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3usyewaxi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3zxhsjiyh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fahwmcom.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3qzaakbni.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bqhcneri.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ucmbrgcr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3gzptwkxx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gzmhkfpp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3tsjesagl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3mzpwytxm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3vmfnwknc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3epcgptin.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3iipimjll.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xhtmhisc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3numzdvho.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3zghzqgol.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ibdxlxbq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3jmzzxtbw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3xvlxlbal.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3esjhpkwt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vxxiddwq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqmjpgqj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rxglntai.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dslpqlbt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3povggmrf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3wqcrgpou.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3omyevkvb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ltiskpvo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3bdbtxjyy.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hunyslzk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmphspab.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3spvsrpwh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3mxhldvyk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3dcvodveu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3qgcluerj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wbyqfnkw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3hrnsulvd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ficqwxql.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3osxorscg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xwnhmtok.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gzxqqczl.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sdsedmmr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3sokfrkfd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3bjqcjluu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zotkknnf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3clkokcqt.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3rqjvyumd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3yrjpserg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3aiynaimo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3uatuxrak.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3guuqsaav.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3qcedesvw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3hradcybf.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3czpyhkzz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3njmjrzxg.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3mppesjsg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gzetvyay.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3krywpzfy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3luvhyzrx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bwmjxkky.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ziathmbf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3umpbexib.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zgqvapeq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xoiuwixg.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3axuqgdqj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3nsnuhedp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ivedoijq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wrplqjcn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3pqdfcvts.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jaezasfo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3hnmznlnd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hfgyomkf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3dgiggttq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3dpcxopmw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3eivoigln.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcmbjfxz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qwhoioxk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3umezqzpq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3wgwecmrt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3fzgxrppi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3mtnmdihd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3kjtkpfot.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3gfpknisb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3qbiuxpts.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3izifhoaa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ocompmsh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jeikfbnk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bacfcwna.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tsoowlpv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3nmtvkmco.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bvxyhsaq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3jiyhpfsf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3hfvylbhy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3awdzdnyb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ukajcjtv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kiprlxfk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dhvynffy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3nrymmpti.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3vifgnlsw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tfgzppau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3npweibfr.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xclfkgol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bepaaltz.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3dwsjpguu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3okpjuuar.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ynptaikr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3crcvftyk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ltjonqzj.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wddqwajm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3taewrizc.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3zcapjvvz.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3dvvuphok.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3kredsvdo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3rwhklddk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3irhqtnum.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jmqsqlqf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3auklszwc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3djwbzbzx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3mynrrcrg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3sluehhon.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3jpekpqcz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3bkbqzdzx.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3graiaqns.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3cpupxpuf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3micrkqfj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3yrdaktkd.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ruztiacx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ibzrvimh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3byrpndfh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3omzjoccg.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3hvzqukpv.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3smjwlzwg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3nqkimmuq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3uxeidfdi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yossmcxk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3pevoeohg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3zbepuboq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3etozhtwx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nduirflq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3oomhusfn.html


<!-- 参考信息 -->