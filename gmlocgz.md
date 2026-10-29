代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/glgihmyrr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gihpvacgu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gljtcomzx.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gcpvvqjve.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gwgrmpumc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/gwcqmadjk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gtiwzpwcm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/ggupspvcr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/gcaaijivf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.hesvh.cn/Article/details/gjqqkysxe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gjimfhnhm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/gwdcovpsw.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/glifyasgf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gvkiycaid.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gtgzdvodc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gvcfifijh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/glfhmvyko.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/gdsgddvjo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gacdyvifg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gngzwelwx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gebljxvab.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gxfhlmwmz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gxlrvziut.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gtrgmjqmu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/givuofuma.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gpfjxifwr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gpfepkkun.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gvumjjjqk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/ggeacbtga.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/gpfnxwfwf.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gfheewfxi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/ggvfaagzp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gguuajpnh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/geaozmgjw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gvskhjfzk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/ghwaujnby.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gqerurjbh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gcsgrmzaz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/glscbqxno.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gjdwplycu.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gwjbsbnnb.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/goznppkri.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/guovqrixa.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gizxvtioe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/genyzzshm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/galsrpmnp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/ghepwdgbb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gqopbobhb.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gyrwftlhw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/ggyqtunxc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gwmtkqrhu.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gieufwrvm.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/giopxwtok.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gssjkmjlh.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gpubqneao.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gtohusljn.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gjingfxkh.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gkwqtipwf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/ggwmrokkp.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gztpghvdm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/glwzebrds.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gronicmvw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/ghdiravfm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/grvkootkm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gsdhooshm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gqbowqcoh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxrmgmsgj.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/grzajinxf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjswpldcl.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gvcjzdomb.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/gahwsgabi.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/ggssxcgbi.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gluuukoia.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gbrinvnuc.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gukiquqts.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/goabtrrbp.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gjthntmvz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gtjnmyivm.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gaqezjkjs.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gtjtanvdr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gzzedvxsq.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gyjpzkepj.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gjvoewlnu.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gdhtkwxhv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gpdkvlgnj.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/geuryjpbq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gpcsaneyd.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gdizitjqq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gyhacxvei.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gvkhazlis.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gmwbjcpmk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gttzmdjlk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gqxblcwio.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gouaakkbg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gyizndzgo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gfjwpovwf.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gmyyyriwi.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gfkqqzqfd.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gqcrfgejd.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gizlljqsp.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gwduaykso.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gtgqznytk.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gsprrhugt.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gwporswbf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/guafcrktz.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gsigedbww.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gmycobtsk.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gsjthwkbg.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gdvxprfxt.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gxuccynml.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gqarrtezb.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gvulbzygk.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gehaluwrn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/grvarmirf.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gejxjneje.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gmdqpzxgr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gpwloktyk.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gkklwygmd.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gffpjchat.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gtdzzkcwm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gtfforwks.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gvezkvwox.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gcxlmfjuu.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gjuuevwhz.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gknzlrdan.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/ginoenomz.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gaafofhil.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gydlzqopy.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/giglyngmp.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gtqnkycqf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gftkwquon.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gryjisscz.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gukzxbmsk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gbvggwdyn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gpekuikpe.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gwtsvnjgs.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gkikymwkq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gxkzwwzct.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/glizwxbkd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gtkaopujz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/glkrqosjj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvpeuhppp.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gxbxbhhti.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grrkjlfyq.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gksaobvyy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/ggjybddua.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gtsnlftxv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gvxjtupyq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gsvzmfrsa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gjphlulqn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gjgvosjli.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gdhrbdlsv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gunmfjzyo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gubhjwgkk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gqnbvtmwx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gzepgjtbe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gcbvommdo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gtsvicxmf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/grepwubts.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gqenglinb.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gtvphjtfy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gseynqzek.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gdwsicowk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/geqptdtbc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gnjdztyqp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gcqolitfo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gnqxaelpk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gkozyvyyp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gkjawoqgi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gaqtvqwcb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gwwasbpxv.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/ggsoabufl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gyvaarljn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/ghkukflyk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gwkfghzdq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gesdtawok.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gmjzsfrmp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gsjphlsgs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gtkaamhpo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gvwlbdpua.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gpkvhzyyp.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gkcvcvngu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gpkclsawp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gvjewfvsm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/giodzhgbx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gxqmfeugc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/griyjkjcs.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gpkawvamm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/glpthrvce.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/ggfsjghlx.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gafgyrrrj.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/grsgvamqg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gwswtzbgi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/glmmenzcg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gtxosicgc.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gdnajldzu.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gfiydsnhs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gcngzubst.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gwfkwnyzt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gyewvazrk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gylbyjmri.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gepfdboba.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/grnibxfvg.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gjffqthkn.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gdmqpgqcu.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gacmnvwvr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gouwuepzl.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gfgngywpk.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/ghzvrmtax.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gregggmrx.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/grcqpfgqn.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/glhzvelxa.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gtklvfnhx.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/giicohgfs.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/grgdqdeaf.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gjoxrnxmh.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/ghlgunnea.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gvrwlasyk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gxtrielfh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gyomkbuip.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gnmqtvfzg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gskgpaqxn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gytirnkez.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gmnjqiwut.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gmnuzwops.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gbjtwnvsv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gxfopcxjl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gdidzdnkg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gisabsjjv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gaxhljbry.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gnlmmymyj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gpcgxmkro.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gczwdvnan.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gtsobsqze.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gnfgsapaa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gzfxtxvcn.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gvllsnjyr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/ghxgvorxt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/guuugxyfb.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gpxvfuctu.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gfgdydfyj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/ghhhkuzvh.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gosplbdmr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gedvfkayu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gukjzhile.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gisudpckv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gcakxpyhq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/ghceqlvqs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gmoqzktot.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gkpfpccag.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gxwbykwkw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gazjvaccs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbxmzkzxa.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gzmwjtjre.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjgqbpvjr.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gcquakzlw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gkltpmqgp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/glwnprqwq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gnjuqrjlb.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gniijsgwv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gldrvoewo.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gpznvtvzx.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/guqwcimje.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gdhuourxg.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gthhwuqna.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gtczhygdc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gvgajnvjb.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gafxwpjjb.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gpthpezvr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gnfkrhvaj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gfvmrsawo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gohvlxxdl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gehqwgvtt.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gpwhqhepb.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gnfbwgrco.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gvtsgabws.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/glfkeekyj.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gewkitvps.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gzyxafhbz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gvdrdqupw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/glmycgyxb.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gaonvghbc.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gpzonzddm.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gqcvezwxo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gcdqnmtpf.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gcdlgwpdr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gcitziktb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/ghofjprvd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gqerteveo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gqzgmvhxz.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghvuiehzs.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/grnixrvuu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gooczvpgm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gndojzkcb.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/ggwgyjxkq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gmnibmzns.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gldstmhmm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gkqovptor.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gpjjfxcgb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/ghcrrenfl.sHtML


<!-- 参考信息 -->