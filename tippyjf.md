代发 wailian999

Go:   encoding/gob
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyigrimk.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gvxoutqjr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxnmgwel.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdsjknfr.sHtML

L. 网络请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gefkfpvuz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gindctsau.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqqifxtb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxuinatj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjvfzhla.sHtML

JS:   await fetch(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfeyliofh.sHtML

TS:   await fetch(url)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnnbztva.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fanxiaobao.xyz/Article/details/gctsbcbwf.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggggeoorf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fanxiaobao.xyz/Article/details/guhjxivtq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvlhqbnm.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdhtoztc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fanxiaobao.xyz/Article/details/gbgocuacm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiutxzen.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmgxjooc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fanxiaobao.xyz/Article/details/gzhudguhr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fanxiaobao.xyz/Article/details/gcfbryllh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgjzaham.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fanxiaobao.xyz/Article/details/gxnnocyle.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxhgvzuu.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnprhuazc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fanxiaobao.xyz/Article/details/gghfviqjj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/giglgchal.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fanxiaobao.xyz/Article/details/gohohqrzy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtudllmy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fanxiaobao.xyz/Article/details/gyjdyosaw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fanxiaobao.xyz/Article/details/ggdewwajk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyccqoqh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fanxiaobao.xyz/Article/details/gdqjceikp.sHtML

[L04] 设置超时
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhrsafza.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvkypqer.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopnyzqsb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fanxiaobao.xyz/Article/details/gxdrtasit.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gslsurstv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgguujwh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fanxiaobao.xyz/Article/details/guafkcmpy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fanxiaobao.xyz/Article/details/gxwtkkega.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gegbeyerg.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fanxiaobao.xyz/Article/details/gppaacuft.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrgvzgte.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fanxiaobao.xyz/Article/details/ggontdtfs.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fanxiaobao.xyz/Article/details/gzwtsprqj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fanxiaobao.xyz/Article/details/gggziupng.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcdjlhvf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gffnmnucm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgyreksw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqdzneha.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gljlmnynv.sHtML

Py:   resp.json()
来源：http://mobile.fanxiaobao.xyz/Article/details/govxfgudd.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxpyshfs.sHtML

JS:   await resp.json()
来源：http://3g.fanxiaobao.xyz/Article/details/gjoklxegj.sHtML

TS:   await resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/gqlscheqq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlewngzd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkhhskwy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fanxiaobao.xyz/Article/details/gpjhjfize.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fanxiaobao.xyz/Article/details/guorxsstd.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxqkfzpf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fanxiaobao.xyz/Article/details/gaedsbybf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fanxiaobao.xyz/Article/details/ghaltvatx.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmappxpy.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fanxiaobao.xyz/Article/details/guunfhwkx.sHtML

Java: resp.statusCode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvnulres.sHtML

Go:   resp.StatusCode
来源：http://wap.fanxiaobao.xyz/Article/details/govowrsdi.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjrytvuk.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fanxiaobao.xyz/Article/details/gfflkynsn.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fanxiaobao.xyz/Article/details/garxvxnrq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fanxiaobao.xyz/Article/details/gfadbalkm.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fanxiaobao.xyz/Article/details/ggansclwu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnkujjdw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginxqohef.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fanxiaobao.xyz/Article/details/grpbkhlek.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fanxiaobao.xyz/Article/details/gqjvtfhhe.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fanxiaobao.xyz/Article/details/glbnafskn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkbgfhbp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gackjzvrp.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fanxiaobao.xyz/Article/details/gzwjoznvd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gurdtwivj.sHtML

[M01] 读取命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gleajjjsu.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fanxiaobao.xyz/Article/details/gjipmsjvn.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpfjrwty.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gtkgmpblb.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fanxiaobao.xyz/Article/details/grualltmf.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrbcxqfr.sHtML

Go:   os.Args[1:]
来源：http://wap.fanxiaobao.xyz/Article/details/giteuowjh.sHtML

Ruby: ARGV
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyyjbleg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fanxiaobao.xyz/Article/details/gqpyvgnic.sHtML

[M02] 读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/glgarkilb.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqzpjsbb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbskutjw.sHtML

JS:   process.env.HOME
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuhcxthi.sHtML

TS:   process.env.HOME
来源：http://baike.fanxiaobao.xyz/Article/details/gnembkrar.sHtML

Java: System.getenv("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/glxjfzukf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/gqbxzfckw.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fanxiaobao.xyz/Article/details/glbumjubo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvglwrrhp.sHtML

[M03] 执行外部命令
来源：http://wap.fanxiaobao.xyz/Article/details/glhlokmke.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclwluiof.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglwpyibq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gcxhcqedc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gmhhnobng.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fanxiaobao.xyz/Article/details/gajzqoeaj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fanxiaobao.xyz/Article/details/ghuaeirlr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fanxiaobao.xyz/Article/details/guymdeiwr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fanxiaobao.xyz/Article/details/gljddicbe.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/guearppbp.sHtML

Py:   os.getcwd()
来源：http://blog.fanxiaobao.xyz/Article/details/grdibnvgi.sHtML

PHP:  getcwd();
来源：http://baike.fanxiaobao.xyz/Article/details/grnchvuvk.sHtML

JS:   process.cwd()
来源：http://3g.fanxiaobao.xyz/Article/details/gqgtrswsn.sHtML

TS:   process.cwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/guatqdnyo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fanxiaobao.xyz/Article/details/gwwbyshzx.sHtML

Go:   os.Getwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gheghxcwn.sHtML

Ruby: Dir.pwd
来源：http://blog.fanxiaobao.xyz/Article/details/gafzkfxyn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknzpsiqn.sHtML

[M05] 设置退出码
来源：http://read.share.fanxiaobao.xyz/Article/details/goplqcjjp.sHtML

Py:   sys.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gxrpbeoej.sHtML

PHP:  exit(1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqtfgwyc.sHtML

JS:   process.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gudkcdndr.sHtML

TS:   process.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/geplfnlqk.sHtML

Java: System.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gwclghpeu.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfabzswjw.sHtML

Ruby: exit 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gwywrvtih.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fanxiaobao.xyz/Article/details/ghijtpmop.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/glatxyilu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gsivutajr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fanxiaobao.xyz/Article/details/grpnzqntq.sHtML

JS:   console.error("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gofbmglwo.sHtML

TS:   console.error("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrtamxtl.sHtML

Java: System.err.println("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcpjupzg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fanxiaobao.xyz/Article/details/geaawivnm.sHtML

Ruby: warn "err"
来源：http://baike.fanxiaobao.xyz/Article/details/gpqvxekba.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgvjfsvl.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjsknmrk.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyjfnily.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fanxiaobao.xyz/Article/details/gkvanpzmd.sHtML

JS:   require.main === module
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpxaerxd.sHtML

TS:   require.main === module
来源：http://m.share.fanxiaobao.xyz/Article/details/gredrpbtn.sHtML

Java: public static void main(String[] args)
来源：http://wap.fanxiaobao.xyz/Article/details/goznrnysh.sHtML

Go:   func main()
来源：http://read.share.fanxiaobao.xyz/Article/details/gczbrotbl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwgoimuc.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fanxiaobao.xyz/Article/details/gisuiorrf.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fanxiaobao.xyz/Article/details/gnrzgpcug.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesdopavp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fanxiaobao.xyz/Article/details/gltabffwp.sHtML

JS:   process.platform;  process.version
来源：http://3g.fanxiaobao.xyz/Article/details/gxktjoeuf.sHtML

TS:   process.platform;  process.version
来源：http://baike.fanxiaobao.xyz/Article/details/goiqolkbl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fanxiaobao.xyz/Article/details/goullsctz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fanxiaobao.xyz/Article/details/gqjhrqjha.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fanxiaobao.xyz/Article/details/gmekdiinu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmzdvvfo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glhctlguy.sHtML

N. 数据结构与算法
来源：http://baike.fanxiaobao.xyz/Article/details/geilgallb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gamckaswt.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gpaipskpx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gliwpwtoe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fanxiaobao.xyz/Article/details/gtuqorbeb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqalznsi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsvamxnm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/glqdnprqu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzjfvimo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnqhdalw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhkjfmjw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxrxwklc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzkkptxw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/geqhxdogv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gmcbvpjuk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/guctiatzj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gutphcfed.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkpfeokl.sHtML

Ruby: arr.sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpibkqto.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fanxiaobao.xyz/Article/details/ghxpntpjy.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fanxiaobao.xyz/Article/details/gntawuakd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fanxiaobao.xyz/Article/details/gmaypgrth.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fanxiaobao.xyz/Article/details/gsifzqymb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxzzgovh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fanxiaobao.xyz/Article/details/ggshvfvmq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fanxiaobao.xyz/Article/details/ggvbwbobu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fanxiaobao.xyz/Article/details/goueicscn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fanxiaobao.xyz/Article/details/gkvohizcz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fanxiaobao.xyz/Article/details/gehbhiccg.sHtML

[N04] 斐波那契数列
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrlixdin.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnzmczyc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fanxiaobao.xyz/Article/details/graizyphn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfijfwhds.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgwpmmow.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdttdfins.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjypirymn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gctzdanij.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmiaiskn.sHtML

[N05] 最大公约数
来源：http://blog.fanxiaobao.xyz/Article/details/gpdwqheep.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbdmlqov.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/grlrbhhvm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuvaigat.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbueepcdf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxxripjm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fanxiaobao.xyz/Article/details/grapmvdsk.sHtML

Ruby: a.gcd(b)
来源：http://baike.fanxiaobao.xyz/Article/details/giukaqrdh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gabhrukmv.sHtML

[N06] 判断回文字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gjabigrdt.sHtML

Py:   s == s[::-1]
来源：http://baike.fanxiaobao.xyz/Article/details/gqpwrvouu.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcqxsagq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohgkzesm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluooewqn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fanxiaobao.xyz/Article/details/gugzyztuk.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikweqxko.sHtML

Ruby: s == s.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/grbwpbtmb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fanxiaobao.xyz/Article/details/gqdhgjiui.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmonllixa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fanxiaobao.xyz/Article/details/gsdirxzwy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqzzvser.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiigqiut.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fanxiaobao.xyz/Article/details/gicxhhnrn.sHtML

Java: // 手写 HashMap
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfirbzey.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fanxiaobao.xyz/Article/details/gehstzwet.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjzqumgq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fanxiaobao.xyz/Article/details/guyhhkgph.sHtML

[N08] 生成全排列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwaxrkcbf.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gozldjpuo.sHtML

PHP:  // 手写递归交换
来源：http://blog.fanxiaobao.xyz/Article/details/grvxcvbcm.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gccqrtssl.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdantnng.sHtML

Java: // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gcvewtrbc.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnezlpfl.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fanxiaobao.xyz/Article/details/glzsorfet.sHtML

C#:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/grncjehlr.sHtML

[N09] 栈与队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzftycit.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjtylpaw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvjomnmb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvvkazhs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fanxiaobao.xyz/Article/details/glonberle.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fanxiaobao.xyz/Article/details/ggverytye.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuckynbp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbfrppnl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfznvuupo.sHtML

[N10] 链表节点定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfdqlmhu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fanxiaobao.xyz/Article/details/gjraactws.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdtnqgsn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fanxiaobao.xyz/Article/details/ghpmjsmvb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/grtaydabi.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlyrqsml.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fanxiaobao.xyz/Article/details/gypoxzzuy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyktebqy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fanxiaobao.xyz/Article/details/gowdfxyda.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gqszbnndc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxmphnur.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gshulkiak.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/glojqyfnz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmdiwmnd.sHtML

Java: // 手写递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvdbwgkr.sHtML

Go:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/ghiskwcvr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genhvqiie.sHtML

C#:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/gemhlzquq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmyfetvq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgkigcqp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fanxiaobao.xyz/Article/details/gwdrztopc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fanxiaobao.xyz/Article/details/gtsixhhck.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fanxiaobao.xyz/Article/details/gttdmnnpf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbceziolt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fanxiaobao.xyz/Article/details/glqplhmgy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gbruhjhwh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fanxiaobao.xyz/Article/details/gtdmmpyia.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblpgqitf.sHtML

O. 并发与异步
来源：http://www.blog.fanxiaobao.xyz/Article/details/guphivkza.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gseiyascq.sHtML

[O01] 启动一个线程
来源：http://read.share.fanxiaobao.xyz/Article/details/glaotifkf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fanxiaobao.xyz/Article/details/gwjkmjtxx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fanxiaobao.xyz/Article/details/gshjwlgru.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhjnhhsz.sHtML

TS:   // 同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giheiufrv.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fanxiaobao.xyz/Article/details/gqnfdjxwd.sHtML

Go:   go f()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfciuonda.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcelrtcch.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwngptnvu.sHtML

[O02] 使用线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gbeyvcjer.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpudbitd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcwurwmt.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahsmkusj.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fanxiaobao.xyz/Article/details/glwstrnhw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsguwthor.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvopgnnb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fanxiaobao.xyz/Article/details/gnptatlob.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwytqovx.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fanxiaobao.xyz/Article/details/gssexihge.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitfciosq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlfrzpdg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtacmqewk.sHtML

TS:   // 同 JS
来源：http://blog.fanxiaobao.xyz/Article/details/gxmcmrmuo.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gernxwmqc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fanxiaobao.xyz/Article/details/gloztojmx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gxjtpbycs.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbchlqfld.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsvhezll.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fanxiaobao.xyz/Article/details/geqpxdyfs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fanxiaobao.xyz/Article/details/guwgjozhn.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvfvzqrv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gwurhrldf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbweufecz.sHtML


<!-- 参考信息 -->