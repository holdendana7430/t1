代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgzvkplr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fanxiaobao.xyz/Article/details/gjhoqfhhi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fanxiaobao.xyz/Article/details/gifswifuz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fanxiaobao.xyz/Article/details/gbuqabvuw.sHtML

[L03] 设置自定义请求头
来源：http://wap.fanxiaobao.xyz/Article/details/gtuloldmx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbwxqcgg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gngvoowwr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfmvdugy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fanxiaobao.xyz/Article/details/gcpotvtxj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fanxiaobao.xyz/Article/details/gyomutiwn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwasrktmk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fanxiaobao.xyz/Article/details/gaksyitpk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknkoczeb.sHtML

[L04] 设置超时
来源：http://baike.fanxiaobao.xyz/Article/details/glnmknkiv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvvvcexg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqacsrmpd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gksnltvdq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlhcrlfs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fanxiaobao.xyz/Article/details/gbncanhxb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fanxiaobao.xyz/Article/details/gfkdchalm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoevlxqh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gjxrzbpea.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fanxiaobao.xyz/Article/details/gxpdhpgbx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fanxiaobao.xyz/Article/details/gvdnzpcly.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqzvhwgx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fanxiaobao.xyz/Article/details/guticobvj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fanxiaobao.xyz/Article/details/gykdozoxm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrukwzfh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gazqomomi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqqwskmn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvmafcet.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gsngivprr.sHtML

Py:   resp.json()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjggvdgs.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/guhknjjxd.sHtML

JS:   await resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/gddtjgtyp.sHtML

TS:   await resp.json()
来源：http://blog.fanxiaobao.xyz/Article/details/ghjvnheft.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fanxiaobao.xyz/Article/details/guxzehhez.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeiadgnt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fanxiaobao.xyz/Article/details/gkddzrmcl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fanxiaobao.xyz/Article/details/gnrzhwsdy.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gskncmgta.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtykhnzri.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fanxiaobao.xyz/Article/details/gntmyerpt.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmtprknz.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvmwdtfb.sHtML

Java: resp.statusCode()
来源：http://mobile.fanxiaobao.xyz/Article/details/gioddioyz.sHtML

Go:   resp.StatusCode
来源：http://wap.fanxiaobao.xyz/Article/details/gwzshrish.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fanxiaobao.xyz/Article/details/gciwitwij.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsjvptlo.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrgipkzl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fanxiaobao.xyz/Article/details/gkvharpws.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fanxiaobao.xyz/Article/details/gkvwgfbfs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmjkufbw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gdbusnxpk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fanxiaobao.xyz/Article/details/gedvgedmn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fanxiaobao.xyz/Article/details/gdqilptls.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fanxiaobao.xyz/Article/details/gjlcyrylp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxtrbkff.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkacbxab.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goowamyak.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gslfkyrdp.sHtML

[M01] 读取命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiewdkap.sHtML

Py:   sys.argv[1:]
来源：http://baike.fanxiaobao.xyz/Article/details/gpeusvpiv.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxhiomqd.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gxpmzonqx.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqslpfuq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fanxiaobao.xyz/Article/details/geinbrwyg.sHtML

Go:   os.Args[1:]
来源：http://m.share.fanxiaobao.xyz/Article/details/goveasyjs.sHtML

Ruby: ARGV
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwpuywke.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqantyws.sHtML

[M02] 读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gexthkakg.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxqlxfpj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgtwyqao.sHtML

JS:   process.env.HOME
来源：http://read.share.fanxiaobao.xyz/Article/details/gltiukaad.sHtML

TS:   process.env.HOME
来源：http://baike.fanxiaobao.xyz/Article/details/gkjunexss.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fanxiaobao.xyz/Article/details/glreqqmfs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fanxiaobao.xyz/Article/details/goiznwyux.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdpcrqcw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/gfspncjwk.sHtML

[M03] 执行外部命令
来源：http://baike.fanxiaobao.xyz/Article/details/gogwlcgaf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/guzsaljaw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fanxiaobao.xyz/Article/details/gbqtotbxp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhtsgrqh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gmzjbioxh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxnflwmn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fanxiaobao.xyz/Article/details/gikcoziig.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzztbbaql.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlehqipl.sHtML

[M04] 获取当前工作目录
来源：http://3g.fanxiaobao.xyz/Article/details/gimrbdtxk.sHtML

Py:   os.getcwd()
来源：http://baike.fanxiaobao.xyz/Article/details/gubfurvcf.sHtML

PHP:  getcwd();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnubdtkyj.sHtML

JS:   process.cwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpatenop.sHtML

TS:   process.cwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gifybjhhz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfvemuoq.sHtML

Go:   os.Getwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtwwdrkx.sHtML

Ruby: Dir.pwd
来源：http://m.share.fanxiaobao.xyz/Article/details/guitnafnp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fanxiaobao.xyz/Article/details/gaonjsnyy.sHtML

[M05] 设置退出码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzegkgko.sHtML

Py:   sys.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gaxqzqbka.sHtML

PHP:  exit(1);
来源：http://www.share.fanxiaobao.xyz/Article/details/grmlxiprg.sHtML

JS:   process.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzzncfcn.sHtML

TS:   process.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzllwgjnx.sHtML

Java: System.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljlhbmzs.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girnrsvgq.sHtML

Ruby: exit 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gitkkqxcw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyqoyrdt.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexjuahrl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgrypxna.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fanxiaobao.xyz/Article/details/gpcwmyfmy.sHtML

JS:   console.error("err")
来源：http://wap.fanxiaobao.xyz/Article/details/gwqvyahno.sHtML

TS:   console.error("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpwzraew.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacuybfix.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fanxiaobao.xyz/Article/details/glkyplkov.sHtML

Ruby: warn "err"
来源：http://baike.fanxiaobao.xyz/Article/details/gvyonkgjw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gtvliexpy.sHtML

[M07] 判断是否为主入口
来源：http://baike.fanxiaobao.xyz/Article/details/gvdmyfltv.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fanxiaobao.xyz/Article/details/gczgpghyb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fanxiaobao.xyz/Article/details/gtmdhpsux.sHtML

JS:   require.main === module
来源：http://baike.fanxiaobao.xyz/Article/details/gplymxnkg.sHtML

TS:   require.main === module
来源：http://3g.fanxiaobao.xyz/Article/details/gvmvtkqbf.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqutqhia.sHtML

Go:   func main()
来源：http://wap.fanxiaobao.xyz/Article/details/gklsxvypm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fanxiaobao.xyz/Article/details/gyxuobsfx.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fanxiaobao.xyz/Article/details/glhyzkkwj.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fanxiaobao.xyz/Article/details/gohcsvysh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdglgamwo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fanxiaobao.xyz/Article/details/geevxurwk.sHtML

JS:   process.platform;  process.version
来源：http://wap.fanxiaobao.xyz/Article/details/gbxmmcygt.sHtML

TS:   process.platform;  process.version
来源：http://baike.fanxiaobao.xyz/Article/details/gxenzxnrn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fanxiaobao.xyz/Article/details/grjpuutkt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmxnwlsc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvavcabj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fanxiaobao.xyz/Article/details/gwprvmhik.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggulbponu.sHtML

N. 数据结构与算法
来源：http://m.share.fanxiaobao.xyz/Article/details/gxshzrixq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghetvjxbg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdulpzrsj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdqtjtoh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fanxiaobao.xyz/Article/details/geeilfgem.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fanxiaobao.xyz/Article/details/gnlengvlx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fanxiaobao.xyz/Article/details/grswolvpj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gudnvibeg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyapelsvm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwjiozax.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gceuoaehq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fanxiaobao.xyz/Article/details/gelxagvzb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdlkvkqy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnryghqd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gqsmxlpim.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbojwoapb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gwtltfjuz.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/guihaduzf.sHtML

Ruby: arr.sort
来源：http://3g.fanxiaobao.xyz/Article/details/gowulxjvk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fanxiaobao.xyz/Article/details/geqrgteuy.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fanxiaobao.xyz/Article/details/gpoyyhdsn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwwnlzbn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmforvvyc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fanxiaobao.xyz/Article/details/gncccjqls.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fanxiaobao.xyz/Article/details/gbtvnqgdy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/guttuthxn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuxaorly.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmykxpfk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fanxiaobao.xyz/Article/details/glzdgeeuy.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimwkjnvx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxempatn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fanxiaobao.xyz/Article/details/glknmguuv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gbgqqbxmb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gohyzhpts.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fanxiaobao.xyz/Article/details/gknhjlycx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbgvpbxc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gebwkymgl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckruspww.sHtML

[N05] 最大公约数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjkceskl.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghajlqcsj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyqtunftf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/giexjlqwu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsqbkaahq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gkysdnyhu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fanxiaobao.xyz/Article/details/grixkbtix.sHtML

Ruby: a.gcd(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gseiatlhy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfljgwmbc.sHtML

[N06] 判断回文字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gnozqziuy.sHtML

Py:   s == s[::-1]
来源：http://baike.fanxiaobao.xyz/Article/details/gvfzsbivs.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcoibioj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnxjtgbq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gfheewqbg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgxlvffb.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fanxiaobao.xyz/Article/details/grvqbvjep.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjqfanne.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fanxiaobao.xyz/Article/details/gnbslzgbk.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fanxiaobao.xyz/Article/details/gtgjtbjjy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fanxiaobao.xyz/Article/details/gzdynypkv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fanxiaobao.xyz/Article/details/guflvntnh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fanxiaobao.xyz/Article/details/gopgefcbk.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fanxiaobao.xyz/Article/details/gzojdlwvx.sHtML

Java: // 手写 HashMap
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfrqyoco.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fanxiaobao.xyz/Article/details/gljnihufl.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fanxiaobao.xyz/Article/details/groalsgxt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fanxiaobao.xyz/Article/details/ggjchfjgg.sHtML

[N08] 生成全排列
来源：http://www.blog.fanxiaobao.xyz/Article/details/getdpkxya.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpyoloxk.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fanxiaobao.xyz/Article/details/gakdmrbyo.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvuuuhts.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/ggaakhrcq.sHtML

Java: // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gnzaxvunu.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/geazlrcde.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyizmlzmm.sHtML

C#:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/ghxxwgckx.sHtML

[N09] 栈与队列
来源：http://3g.fanxiaobao.xyz/Article/details/gqdbnlniu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gsbdsqkuw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoghiyal.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gphvfnzqq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fanxiaobao.xyz/Article/details/ggkkinogs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwzyadon.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhqxrqus.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtsermni.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fanxiaobao.xyz/Article/details/glwgvfuwy.sHtML

[N10] 链表节点定义
来源：http://baike.fanxiaobao.xyz/Article/details/gluxswylr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fanxiaobao.xyz/Article/details/gkhcvjaow.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdzousspw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylewvxkk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fanxiaobao.xyz/Article/details/grcgnnfxd.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjwusdau.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzrrflcr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fanxiaobao.xyz/Article/details/grnclmurm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqpjuunos.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnsbnijy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fanxiaobao.xyz/Article/details/gdrxttmst.sHtML

PHP:  // 手写递归函数
来源：http://wap.fanxiaobao.xyz/Article/details/gaccytcqe.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fanxiaobao.xyz/Article/details/giokfnofv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fanxiaobao.xyz/Article/details/gpmplzusc.sHtML

Java: // 手写递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdndboggc.sHtML

Go:   // 手写递归
来源：http://mobile.fanxiaobao.xyz/Article/details/grpugnrgv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fanxiaobao.xyz/Article/details/gxparwwle.sHtML

C#:   // 手写递归
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrhzdxrc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fanxiaobao.xyz/Article/details/gtzkxtxnq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fanxiaobao.xyz/Article/details/gziuoddoy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrdhnrue.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fanxiaobao.xyz/Article/details/gpvrjyfaw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctdwenmz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fanxiaobao.xyz/Article/details/galwxkhnl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucrgyurb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/glnkqkeyb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fanxiaobao.xyz/Article/details/gjawsvkrd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghysaospj.sHtML

O. 并发与异步
来源：http://baike.fanxiaobao.xyz/Article/details/gbeytkbaf.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvseubgyu.sHtML

[O01] 启动一个线程
来源：http://3g.fanxiaobao.xyz/Article/details/gisxginoy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fanxiaobao.xyz/Article/details/gobwdeooj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxooggsyx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fanxiaobao.xyz/Article/details/gvvogzjrj.sHtML

TS:   // 同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/gvnpmoech.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrkcvlzv.sHtML

Go:   go f()
来源：http://blog.fanxiaobao.xyz/Article/details/gelidogno.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlmsparn.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxrifpkv.sHtML

[O02] 使用线程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gurjyohgw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gclydqxcs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fanxiaobao.xyz/Article/details/goomymscq.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gskegmbmp.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsaceubs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gfywkqyhi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fanxiaobao.xyz/Article/details/gmczbtcdx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fanxiaobao.xyz/Article/details/grjgnvvjf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepzfbzxb.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvdyaseb.sHtML

Py:   with lock: shared += 1
来源：http://baike.fanxiaobao.xyz/Article/details/gaotzwmnf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fanxiaobao.xyz/Article/details/gkaamwvcw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fanxiaobao.xyz/Article/details/gghfqyhmd.sHtML

TS:   // 同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrojzwgi.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvhxswjco.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fanxiaobao.xyz/Article/details/gtahysjyy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gsgdsilur.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwwrmkqi.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqhmerjd.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fanxiaobao.xyz/Article/details/gaucamhgk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fanxiaobao.xyz/Article/details/ggvswucuc.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gskepfxae.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfpbodaq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fanxiaobao.xyz/Article/details/gnprbdabr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fanxiaobao.xyz/Article/details/gmbpnenej.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fanxiaobao.xyz/Article/details/gdczrrudi.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gfhwysnsy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fanxiaobao.xyz/Article/details/gracoprwo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoylrntx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fanxiaobao.xyz/Article/details/gjsknkade.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/grdvopfcn.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fanxiaobao.xyz/Article/details/gmfqfomts.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fanxiaobao.xyz/Article/details/gettiscoq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbbstpzw.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fanxiaobao.xyz/Article/details/gmavdqxbn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fanxiaobao.xyz/Article/details/gnkglrmsf.sHtML

[O06] 使用进程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapdzgsvp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtzxadhw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaijrmmxq.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fanxiaobao.xyz/Article/details/ggugbgzqp.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fanxiaobao.xyz/Article/details/gabeleygh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslzxkhkl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fanxiaobao.xyz/Article/details/ggnhsbnae.sHtML

Ruby: // fork 块
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcwixans.sHtML


<!-- 参考信息 -->