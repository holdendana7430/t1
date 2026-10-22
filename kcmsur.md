代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2wmpmbelg.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2modabtti.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2pjmthmaw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2uiykkfnk.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2nhzgihkr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2vxruezpl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2panipqpo.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nwtnfwvv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2eiqxpqso.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xocrmjqr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ehbwwlsa.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2elidamth.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2uzdgsllo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2lepexguv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2gsqbemxq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ajppovwq.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2nvgykwkm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2fiiuonio.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qpispkth.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gvpjtyrn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2tmiuuxzq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2xcshrebu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2dxcietle.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2wmhgsoon.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qbwlnwfd.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2xvkhafsl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2zgyenapf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2lybnyqdz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2anqvueaf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2giqoefnf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2dzbeploo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2etiqtkwp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2fnwmqdlu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2hzqxaabw.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2hpwekxde.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ynoamtuo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2kmnkswnh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wezxkkyh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2xcxqozqx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2jajxhfnj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ctomlkyw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2hyeihnff.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2miftycux.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2iivsuxer.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vcdaybrv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2gomlvnne.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gzgekoin.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2iuazseui.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2cvfeiibz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2kdlblzzq.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2hcspbpum.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2enskncwu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2opquhnbv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2zvcxwxov.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2pchveppx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2heikvozn.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jwzxzdfr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ftvbdcdp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2fvepcpcj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2gpmtkhfe.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2magmpvfj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2uhbokfqs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2skymnduq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2tqkrzqgf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wwmufqbm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cgzwcbtc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2uydusogm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2dtskujet.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2afueljom.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2phxyrqik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqsbacxi.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2qjnjhejg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gwhehehk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vwwparft.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2esxevats.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2zfcqwybw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kfktfvbr.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gwojolqq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tbmvbggx.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2xxmlvsbb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2aqchrorv.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2omqwgyaz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hujizcfr.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kvjugvnh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2uhxdlbqi.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tanyxtln.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ierzstxi.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xpmbuupp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mjcmdxaz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2iljouttj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2sgrymvvb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2usyxwhko.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2svieiucw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2jmgsgcyg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2razyduau.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kuyrtwbl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2czuecktp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2nspmkhnb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2gbrnpyur.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2dvaqseef.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xcrrzbdq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jgquhxow.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2xkgdqqfk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vobvatxy.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zxbwsszd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2xfwlkqjg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2mpblozif.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ndgadvuw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2udryzemq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2rsivhccf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zkdiubmv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2fdihrejs.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2daamjgjm.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2poqhkbpj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ldamdnov.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pbqvphfe.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2taqozjre.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2tqtpmhnb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2gizdtwrs.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xlrldizw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hbnykgbe.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dgqzhhyh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2icagpviu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ysowjrio.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2fxiezcwm.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2xjosqqrf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2hifqwttx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2jphhgyfy.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2zqxnpmje.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2rsqgnksy.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ikdqqpxi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lnuewldz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2vefgwvco.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2brdfgsby.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2pqwvedoi.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ewysbtrf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2mqmwmilf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2qrmjqmht.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2gkveyfdz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2dzsomwya.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jlnxmbxo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ynuirtmm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2vsfvoeae.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2dnhzivfy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2imshhfmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yicflrbf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2onffkceo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owgnlequ.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2yocaqxnw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sivcttdn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ycildbno.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ivkvhddm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2opmesnuo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hofxonzf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vwldcyrf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2xwxnzwlm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pnnahesb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2jzzuqolz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wfipwdcy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tknguxsz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xhyrszyn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ngbqnumt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ktknmrod.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cinlhvjo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vtfnjovx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wzwuvcrr.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ebtdhamh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2vvjkqjyz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2goxlglqm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2fudeekvb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xapfnytb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2bdpspjup.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2hwryazyf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2bmbmwbti.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2yigqpqzf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2fryljevj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bnmmiyhi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2nlviiflr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iouwuwgj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hllrehnr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2iirlpgbf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2gatvytvq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2sqwaxitj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2epifxvww.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2pyrzzerm.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hfdlmekr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxrbazif.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ulgipbku.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2msdfjuha.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2mqacziin.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2vysvfqgu.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2luowmjyx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwfbwfdv.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ftwyjgsl.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xjlehlvh.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nqlyvjsa.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xttesext.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tjhomidk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2sgqgmdmx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2nvmkfwnl.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2whljxnct.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2soxujsai.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2qgvuqkes.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2slbbcncc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2iixfqajn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2zxnydoaq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2miucfidc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2rbluxsel.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2fhmdjjtw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2rwjbphuf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2dsvpugbq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2booyoors.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2okxscrhu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2mpubkqpf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ikhmywhf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nhbfypam.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jzsxygru.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zxlrhjqw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bfvomaar.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nrnhcudn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2emawijgt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nrkkiyuo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2egvxadup.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fayhpjox.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2pazetdww.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ckcemyvv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2pwmxsfct.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2aflrxbok.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2olideoll.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2zeajtqer.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2slnicdyi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2jdosmwlo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2puucpzja.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2rwrbhfdt.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2phkyjenn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2syjtuxds.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2qamkkndj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykxtkblu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pccprbck.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2lqzaglkd.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2zymaqysd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lizjzsbx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ixtlbvze.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wbgrzifj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yttuzeyc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2iuqyvhnv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bvmamoxm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ufzsjweu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2foneruye.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2egmhwrrw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2rujgfzca.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2afamtwhz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ivcuvnlx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2utskfrsj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kpnisnlj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2gbrcmrgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxtlymrv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2pprkrhyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdnvtovb.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ovbfsfev.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2atkkrqhe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2upabajak.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2snsxiuuf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qtdjkaaj.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2gjlieqos.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2cqkaoobp.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2oargpiim.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2rpvboyyn.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mboryvhf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2kntpeegl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2voxdvhpa.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fngqntwb.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ymxscomw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2fheioyxh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2oartgdma.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2yujwzrki.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2pbzkkgwc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2etqzygka.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hrzjwrix.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2kwumzetk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2cqszqhvp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2cxfrrknx.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2devfzrkl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ebruutmz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2whoxlndm.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmmbajmv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2fzqqtfvv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2vzaqmeph.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2tdydxjek.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2lafpvprx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bmqpqzlp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ugjaqsye.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2gfvkeekg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2rbmmlbgy.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xonkngeb.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2novbvjzp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qjovestf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2eqyxgpnj.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vrpbthgh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uxoiwlay.html


<!-- 参考信息 -->