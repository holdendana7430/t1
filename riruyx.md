代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kbfzncgw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3oghvlypw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ocxsgtzh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mgopazmr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3cdbshftd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3krinpjzs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3twjzuhvb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3muylpxpw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3lyngxvbk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3mbfvutnd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3vhzszujh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3eeicoykd.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3lulgnzpm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ggxsahag.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3zgjawvng.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ljggnyvb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3vibtasgq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3eslolmyl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3thjjaqra.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3xvaogmns.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3cvawacsi.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3qnijxwhn.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3inczalld.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3uipvzzbv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3kraiiuzz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3tmfvnorz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3oyfadkwr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3uaxhmkny.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3swqxshxs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3bxpccpet.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3suhdgarw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3uoaejbzb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3qjmomhkz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3lrdcctmu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3lfhfhabl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3yodgljuf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3oejeesqm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3jbplmpxb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sxlrjxaf.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ixbmixss.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rlqteggp.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ltwxjyos.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zmwscora.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jtbhfslq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3nvksnutp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3yomgbaio.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3zgndrgfk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3lsjihksg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hegjbnkj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ufnbviqg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3kuglhtpm.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3cnhwnobn.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3pvxutzxs.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3yjzubfny.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fjrdgkte.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3bagiyser.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rcyivugb.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3kxjbkcya.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3wkdrknff.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ndondspk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pxurjxny.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3heqqmcdd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3mtirzvmn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3qcfzhntj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gnwzttqx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qmxzutuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3axklbykb.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3yarrthhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tjuefvre.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3lqubitpm.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3pnknssbx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ofavseii.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vevhyeik.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3afsumoft.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3yrcajfbr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3kiqmjrmr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ascztypn.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3aymscogz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ahyklumb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3iztltunx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3fqfjidvh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lnpsbfvx.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jttxjire.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fswgiopk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rdumiwbd.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3uvzjtwss.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nixupeoz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3nyvpsats.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3monmyfvn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3pigmxpig.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vnuxdckm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3txzcmovd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3xvmytmus.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3bbnlbccm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ggrzbudu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ezswpxfj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ruwdkgkz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wrwneaal.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3svaqlpee.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3brtpkvpf.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mretevkp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3emlqseei.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3itveeswf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3zklvxzae.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3mwsgkebj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3dyfthdzd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qxlgcyjc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3czpbmfud.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vuxujweo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tnqmztgn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wagzgjfz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qlxbfhoz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3qtsqssnr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3xbtpdnko.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3otuuwmyl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wyipnspf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3tdzoxrmg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3frhfopkt.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xrytxair.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ikpxovwb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3tcziemkx.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mxtayjiq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3xelzfchs.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3jvyjbyty.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3xqxwqcll.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3wtqubghs.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dpqdwjjm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3therdfhx.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zlivlwed.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3otpdrkvg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3xcyldfcl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3yomsulzo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ilwfowmf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3hoermmxy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3iukftrsu.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3iiniumgi.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3lauwotef.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3pzxpfvwz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3znuhqtzm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3tbogzkkm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3aaroyhxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3noqrhvzf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3xztqbwvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eagtzmbb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gghummwf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3debwbsej.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zcqwqkgx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zxkcaedi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xdpfpffd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sfygouli.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ijufrbif.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3znulfdus.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xcnbdwoo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3wbgpclux.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qxamcvig.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ndqbcxqf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3itnecbis.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wwdqrbxo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3upkrtqmb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ygzpqsih.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3naoeyqlt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3jcylbgrp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3bqooekzs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3fqucywzt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3fkezskix.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wpgskbet.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wbigmwsp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qzqhvfvs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3hsarzupi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3regikynb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3rrlbtcox.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3xfymmypr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pcjltoca.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3bjhmglcy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dbmuexdz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gjlvakyv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3muomogkh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ddwoflrd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zdcjwkyr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cbktrysc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3suoqqcem.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bcrdtumd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzxynjta.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sguahvpk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3arcbmvyh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ogysrass.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3otsgdiuw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kpqpoxtt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3jexghqou.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ozhvjzyb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ypsnsseo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3skddgxnr.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3meridqws.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pmmsstat.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ixthdrwn.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3xdbnloud.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3msrownkn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wqexoolr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3kagurjmv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3mxcudrjb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ovfyofsq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3vjagjier.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3nwovvkqz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3cnwbcbdu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3qpvkzyfc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3aghjccmp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3pjwbfdrf.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ubxihjfk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3szyeccab.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3rdakgrzd.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nqtxxqvb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eqiuuctf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ikwalwlp.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3llwwsagm.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3wrrvburc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bsqctanf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ufnapcmp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3zlpnwdbm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lrgkqrso.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xijbcxkv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3rdqkwnwd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jhjshurk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3irhgxzck.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yfipfcgx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nzmjsjzt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3xndcucpr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3mhjfmpec.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfepgini.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kssaupyr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3gjbcmaqs.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3yfzicyrg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3qhpfcfep.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3htcwjvbm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwfrleqo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3icbdbuze.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3qqfwomom.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3cwqfvnug.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hcgipdly.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hnisubfj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ecqrkjye.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gywvbywi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3vydxhklp.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3akfzeugd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3dsiekcpt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3rzskjxuv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3evaafngy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3xharixpd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3czubhuhh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3mozdvdvw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3gpoheexj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3yvqrirng.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3wbshhzdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udjspccv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3surlaqii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mnpqotnu.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3rhptjuok.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3oztuilhk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3zbzywwfi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3lsymuzek.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vcyayplx.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zcqlbxmu.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3kyfbmuhb.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3aqkxdnfv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3cldbxbcy.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3jenugiab.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3cbeehsmp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3nporrjao.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lczyuuas.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3akqxldcy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3xqkjfyvr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3vuakdkwz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3dsjnipsi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3eumtkgij.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3mxkzfkbx.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3sbfjfxdm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3hhjlnpzd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ujkuxgsv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ilpyqbyl.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgwxtytz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ixdalymf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3godpvccg.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgqrabix.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3rhhllxig.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3kpctyyxw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3wpopmfjb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rjnzyrjx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3coeifwzq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3biuxavsj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ynrazyfa.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ipdejvrx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3hjdzrhwi.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3aecvyxoq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3rbcspkoh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3gtjysnau.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3sympgmjj.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3bmoyhtwg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3kzezkewc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3sazjfbvx.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3giqyyjlp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3azmleydm.html


<!-- 参考信息 -->