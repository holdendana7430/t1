代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuvrxlsa.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fanxiaobao.xyz/Article/details/gmalquszm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkglwvqoz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbdnaeaw.sHtML

[L03] 设置自定义请求头
来源：http://blog.fanxiaobao.xyz/Article/details/ghxdbkwyv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fanxiaobao.xyz/Article/details/gnsaojiuz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcazkdzdn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fanxiaobao.xyz/Article/details/ggybcjahd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxipkyvm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrijpnui.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnkodvst.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fanxiaobao.xyz/Article/details/geivouszs.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fanxiaobao.xyz/Article/details/glzzwbfbr.sHtML

[L04] 设置超时
来源：http://baike.fanxiaobao.xyz/Article/details/gdzvtstcg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fanxiaobao.xyz/Article/details/gatgyezhc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuryzmua.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fanxiaobao.xyz/Article/details/gdeuiilaj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fanxiaobao.xyz/Article/details/gnppnonyg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fanxiaobao.xyz/Article/details/gdnferwzn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwymqenj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fanxiaobao.xyz/Article/details/gblalocos.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gyubdjaup.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoslgctp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fanxiaobao.xyz/Article/details/gamsnuflp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fanxiaobao.xyz/Article/details/gakpaxwqv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fanxiaobao.xyz/Article/details/guljkzgia.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fanxiaobao.xyz/Article/details/gueewlnrj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fanxiaobao.xyz/Article/details/gwffgltpc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyfwishzf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrlhnved.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gxbvrdncw.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gwdihhmpb.sHtML

Py:   resp.json()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmubrubn.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gqfaldcpc.sHtML

JS:   await resp.json()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtnycxtn.sHtML

TS:   await resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/ghdavdvad.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fanxiaobao.xyz/Article/details/gvzbhixim.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fanxiaobao.xyz/Article/details/gwydybccx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fanxiaobao.xyz/Article/details/gwtjsphkc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fanxiaobao.xyz/Article/details/gifxjnslq.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihknvykp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fanxiaobao.xyz/Article/details/gchuhdngm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fanxiaobao.xyz/Article/details/gmxxzjjar.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fanxiaobao.xyz/Article/details/gmcgvaevp.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fanxiaobao.xyz/Article/details/gkebbogsr.sHtML

Java: resp.statusCode()
来源：http://baike.fanxiaobao.xyz/Article/details/grsaqowep.sHtML

Go:   resp.StatusCode
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqwifmyp.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbctyavh.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fanxiaobao.xyz/Article/details/gqzqirutb.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnrfdlvc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fanxiaobao.xyz/Article/details/gatlioaoj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhookxym.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzkvzcdn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gcysmoqfi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fanxiaobao.xyz/Article/details/gzirhveaw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfcxapco.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpacxurcc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgljhdcq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxwpfcgxr.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpwlveat.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnewpweu.sHtML

[M01] 读取命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/glwkyhygx.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fanxiaobao.xyz/Article/details/grvqkamht.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fanxiaobao.xyz/Article/details/gbrrdyqzv.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvdffqfn.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdvhcwqn.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fanxiaobao.xyz/Article/details/gqbwlasna.sHtML

Go:   os.Args[1:]
来源：http://mobile.fanxiaobao.xyz/Article/details/gtymrqvkt.sHtML

Ruby: ARGV
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyreigur.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fanxiaobao.xyz/Article/details/grvmqovzn.sHtML

[M02] 读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gkwjjizpw.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gbklvfbrz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fanxiaobao.xyz/Article/details/gtzvkgoyx.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpyfhzdo.sHtML

TS:   process.env.HOME
来源：http://blog.fanxiaobao.xyz/Article/details/gjqthbjrd.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqfqxfig.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gqznglozk.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkmmxfub.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfgetmmv.sHtML

[M03] 执行外部命令
来源：http://blog.fanxiaobao.xyz/Article/details/gtmfavclc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcovefzlk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fanxiaobao.xyz/Article/details/giemvwxgv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcgamhlf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgpxsfwn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fanxiaobao.xyz/Article/details/gxrnyzira.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fanxiaobao.xyz/Article/details/gcsqqhtpf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fanxiaobao.xyz/Article/details/gajhvycnc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fanxiaobao.xyz/Article/details/gdxkxxhcq.sHtML

[M04] 获取当前工作目录
来源：http://baike.fanxiaobao.xyz/Article/details/geaoyjkce.sHtML

Py:   os.getcwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopkjjurf.sHtML

PHP:  getcwd();
来源：http://baike.fanxiaobao.xyz/Article/details/gapnrbkug.sHtML

JS:   process.cwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpjjmtki.sHtML

TS:   process.cwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvfbsayx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fanxiaobao.xyz/Article/details/gbnmnjsab.sHtML

Go:   os.Getwd()
来源：http://baike.fanxiaobao.xyz/Article/details/gjfjpamfj.sHtML

Ruby: Dir.pwd
来源：http://wap.fanxiaobao.xyz/Article/details/gvtemhpnl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyesxkfl.sHtML

[M05] 设置退出码
来源：http://3g.fanxiaobao.xyz/Article/details/gomioksnw.sHtML

Py:   sys.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtbyasse.sHtML

PHP:  exit(1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjloyzcb.sHtML

JS:   process.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdikkbjo.sHtML

TS:   process.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gjskwqond.sHtML

Java: System.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gbsvjgwfu.sHtML

Go:   os.Exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnpmlmsq.sHtML

Ruby: exit 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gexipnvhv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzecfrboz.sHtML

[M06] 向标准错误输出
来源：http://baike.fanxiaobao.xyz/Article/details/gzxrdhnfn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlrtthbk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fanxiaobao.xyz/Article/details/gaerwywir.sHtML

JS:   console.error("err")
来源：http://wap.fanxiaobao.xyz/Article/details/gbshopghr.sHtML

TS:   console.error("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfbbhntb.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsdqqktm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fanxiaobao.xyz/Article/details/gilolxxqj.sHtML

Ruby: warn "err"
来源：http://wap.fanxiaobao.xyz/Article/details/gdinyqmqh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgbnijda.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjrrsxlh.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fanxiaobao.xyz/Article/details/gfsdelgtd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gahbctuia.sHtML

JS:   require.main === module
来源：http://wap.fanxiaobao.xyz/Article/details/ggcivohyp.sHtML

TS:   require.main === module
来源：http://3g.fanxiaobao.xyz/Article/details/genchbrhh.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdlmnjjn.sHtML

Go:   func main()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwckbfzo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fanxiaobao.xyz/Article/details/giqqwyvhy.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuusifif.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fanxiaobao.xyz/Article/details/gqvgtqegk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fanxiaobao.xyz/Article/details/gybptipnp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fanxiaobao.xyz/Article/details/gumnbiuhh.sHtML

JS:   process.platform;  process.version
来源：http://blog.fanxiaobao.xyz/Article/details/guprgutwv.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjfaijyn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuqjuwvb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fanxiaobao.xyz/Article/details/gmcoxuuaq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fanxiaobao.xyz/Article/details/gdatdmjqt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuhyvoab.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjcpfuwwi.sHtML

N. 数据结构与算法
来源：http://m.share.fanxiaobao.xyz/Article/details/giacqjulu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckrbflmy.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gvushtbog.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuoyvbbo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fanxiaobao.xyz/Article/details/gelzzejsk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/giezoodsj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grktjpcdf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqozeujq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gwazyefgw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fanxiaobao.xyz/Article/details/glailwvud.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeajoukz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgjnbrwu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyhngwuw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gtimhkyvj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gombgdkjl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqjasvhl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gyonqeewj.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiwqvqzu.sHtML

Ruby: arr.sort
来源：http://baike.fanxiaobao.xyz/Article/details/gilprkijq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fanxiaobao.xyz/Article/details/grethynxz.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fanxiaobao.xyz/Article/details/gswkoayyz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsoiojdi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fanxiaobao.xyz/Article/details/ghmahzloa.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcgmpuog.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fanxiaobao.xyz/Article/details/grstgxamz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fanxiaobao.xyz/Article/details/gywmeqzun.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyzpthvu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuzkavmf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fanxiaobao.xyz/Article/details/gudnpcuom.sHtML

[N04] 斐波那契数列
来源：http://m.share.fanxiaobao.xyz/Article/details/gfffhcrmn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxbbifdm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fanxiaobao.xyz/Article/details/gyiuszpwa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdusdbojp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubynkmoj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fanxiaobao.xyz/Article/details/gdxtmxfvt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fanxiaobao.xyz/Article/details/gkbqzvocf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gndqswufz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gkkoqrmeb.sHtML

[N05] 最大公约数
来源：http://read.share.fanxiaobao.xyz/Article/details/gaalpybea.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/gnvjgohnm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkopfjvx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpemzgxyr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/giszghjpd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufjkbmhx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxcnyjlv.sHtML

Ruby: a.gcd(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gxlfntakm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fanxiaobao.xyz/Article/details/ggrymeixe.sHtML

[N06] 判断回文字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gqslwupts.sHtML

Py:   s == s[::-1]
来源：http://blog.fanxiaobao.xyz/Article/details/gbwynchmp.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiemfayj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gcqnfshix.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdrwwfoe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuhxwior.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gfokiuygg.sHtML

Ruby: s == s.reverse
来源：http://blog.fanxiaobao.xyz/Article/details/gwlklaefs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwswpfvh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqsqdwlb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fanxiaobao.xyz/Article/details/gseyweofz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwwbiijg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcokmkuvi.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fanxiaobao.xyz/Article/details/gptefhrrr.sHtML

Java: // 手写 HashMap
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhzshbee.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvurirdg.sHtML

Ruby: // 手写 Hash
来源：http://blog.fanxiaobao.xyz/Article/details/ghjqbkcpp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fanxiaobao.xyz/Article/details/guibfbzvw.sHtML

[N08] 生成全排列
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoufhdzi.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxpfhfkx.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlwtrrmn.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzayhpkz.sHtML

TS:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gxdyyafah.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimpqbmzr.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvnpffna.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbdobmrt.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtywagbrk.sHtML

[N09] 栈与队列
来源：http://3g.fanxiaobao.xyz/Article/details/glcdvnawk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcckmivv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/gggbrusji.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikixdrow.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fanxiaobao.xyz/Article/details/gsxbcqpcw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fanxiaobao.xyz/Article/details/gainomlay.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcvvksoz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubocjtfi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpygilmy.sHtML

[N10] 链表节点定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gudcfsqki.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjcxlcam.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhmqxokj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gzonejdqi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gxiomnktk.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjjqoqlz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fanxiaobao.xyz/Article/details/glxwsfndq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghywvwpii.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggejynmvb.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdevvajm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiyueiww.sHtML

PHP:  // 手写递归函数
来源：http://3g.fanxiaobao.xyz/Article/details/gfknvylfb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfflmxep.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gvariwnfz.sHtML

Java: // 手写递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gsazradfu.sHtML

Go:   // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gieuhspcn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fanxiaobao.xyz/Article/details/geyccztxl.sHtML

C#:   // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/gqechhuqj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbopuvgcx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fanxiaobao.xyz/Article/details/grbebhztd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrxnxzlz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fanxiaobao.xyz/Article/details/gnlthcima.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fanxiaobao.xyz/Article/details/grvrghefn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fanxiaobao.xyz/Article/details/gbhimfzqr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fanxiaobao.xyz/Article/details/geoctciui.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfskwasi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkpptibx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gglndxnir.sHtML

O. 并发与异步
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbryptgnf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gihqirhjm.sHtML

[O01] 启动一个线程
来源：http://baike.fanxiaobao.xyz/Article/details/gieljyran.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhpomwzq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fanxiaobao.xyz/Article/details/gjynofzjp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdfyelqz.sHtML

TS:   // 同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajpwihkl.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fanxiaobao.xyz/Article/details/glbztptxp.sHtML

Go:   go f()
来源：http://wap.fanxiaobao.xyz/Article/details/gdojskaho.sHtML

Ruby: Thread.new { f }
来源：http://blog.fanxiaobao.xyz/Article/details/gxiexktvu.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fanxiaobao.xyz/Article/details/gyshqmdhr.sHtML

[O02] 使用线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gokxsamei.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqccmjto.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtoelcfx.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/grimsskbu.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fanxiaobao.xyz/Article/details/gfipntjxa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzhryxyy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fanxiaobao.xyz/Article/details/glidgusvz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fanxiaobao.xyz/Article/details/guyhfqyvt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fanxiaobao.xyz/Article/details/gzamlfidf.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fanxiaobao.xyz/Article/details/gddqnmkrq.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbgiguqi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzhvylpn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fanxiaobao.xyz/Article/details/gexdzrzdn.sHtML

TS:   // 同 JS
来源：http://blog.fanxiaobao.xyz/Article/details/glqwufdvx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjdygdbb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fanxiaobao.xyz/Article/details/gwuoalwcl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpzqjcig.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbwbxyuaa.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gjljtfpzo.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxtpaplb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkevxwie.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gleatwxqq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcosxwqv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fanxiaobao.xyz/Article/details/gvyjhlroo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjzntnav.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbdelzmy.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fanxiaobao.xyz/Article/details/godvvcnlb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhubyhig.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbryjxjg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmnmoxmx.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxdztslr.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/gbuzjfccb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fanxiaobao.xyz/Article/details/gjmomgxif.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyycyaio.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbdubgpm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fanxiaobao.xyz/Article/details/gygniddny.sHtML

[O06] 使用进程池
来源：http://wap.fanxiaobao.xyz/Article/details/gmpntavst.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydyvcbyn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyagljsfg.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fanxiaobao.xyz/Article/details/gplrxvcgl.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fanxiaobao.xyz/Article/details/ghgfguzkc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fanxiaobao.xyz/Article/details/gunpvfkeg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtaetuutm.sHtML

Ruby: // fork 块
来源：http://wap.fanxiaobao.xyz/Article/details/gwpkzwnqb.sHtML


<!-- 参考信息 -->