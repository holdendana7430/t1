代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gutrhbgwl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gfdoztftl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/gsdjwhaxu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gqrtwmvtz.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/gypprrqkw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/ggajutsrz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gjtmnzyie.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/ggnhcffes.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gmjampxfc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gnaugupad.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/ggrtxxyfu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gzeygzxtw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gzhgkmixv.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gmeqzobvx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gsgsqaonb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gcvypzjlk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/goiaoukbz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gjqyyzmwp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/gijsjcyab.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gepoavzwn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/ghzipvrlk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/geetrccau.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/ggorkouek.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gnkytyneh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/guenguoro.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gljehgkbu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/ggyxnbbap.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/gvsehdfew.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gyndoatlt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gkfyjxryv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/goszqpmbi.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/guabnhixe.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gksekpowm.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gdqilmptz.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gwzvekvjx.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gdfzutbwi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gaaaxvkgx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gocnffppx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/grnbajnpo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gspikuqsa.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gpphhkxhb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/grpkkqbza.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gzvzcxxel.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gzitxduxe.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/glpsytwnr.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gpaiycogy.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gcsadooqp.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gndumgdqm.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gagtrmxdw.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gmhhetylu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gnfaivjyi.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gosmgupmy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gdengnzdk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gtrsyeidc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gvbxcxtag.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gxcxwwosz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/grepsvxsn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gfngwqqhl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gujjgjxmz.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gnayllmrt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbfhagbtd.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gcoyhcgdd.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gqazaxopo.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gmwuafoth.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/ghlildxya.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gyvlpjocx.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/grlrhhjhk.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gkotykeas.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gvvmdxfxs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gbakmnxcl.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gsjhnbypo.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gdwkqdhzu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gbgodeczp.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gjzylnjpa.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gogdqwelz.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gfhwxgtbd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gwxcyduwx.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gtyafjlhk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gbhprlxnn.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gmxgpagle.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gbiartszh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gemcqjdre.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gkeyrgoui.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gtkauuabh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gzpuymdvj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gtextdesb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gcbpvjmoz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gnitqdaqf.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gynhswzor.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/geeojsjfe.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gricudcyr.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gnedigngn.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gapnldkio.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/glgocviyh.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gcensbfkx.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gyxxqyqpy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gdqbrdaez.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gpdvhqntt.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/ggiaiybco.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gigughggz.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/glfwppqfd.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gwtqxrwho.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gbnbeksfx.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gszrrnwti.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/glbosupfa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gbxqfqeuz.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/ggcojupsh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gmugdzfjd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gkcqcyiji.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/grmeqwxib.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gydunisrh.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gfmxesyxy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/ghuonymcn.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gnraeeemj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/ggrkyqzbr.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gdurunywp.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gvtexztky.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/guiqqcjih.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gcsnthhlj.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gwrplnigz.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gesqrjuox.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gpryitrpn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gafzfgbdb.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gvmdznwzp.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gsqgzhzql.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gtmsxauhb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gihulaart.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gianqybor.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gccoocfdu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gnopcpdfn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/ggmucxmqo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gvliqqucc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/golzzcitq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glhxrfobv.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gfptkkbps.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giieqmddf.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gxslcuqmi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gdvgfjyzu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gughuayab.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gcxaavbyu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gnuxtcjdl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gbersgdoy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gebnucgvw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gobbmxaoy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gogaezzeu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gaqzmtfoe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gdrieavej.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gtywgypkv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gamukjrwe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/ggngsbjcy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gmfdmgiqy.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gvszasipr.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/grmocdvwd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/ghvxpvkul.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gvmyrgagq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/grshbegiy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/ghdejcjsn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/govaqhesw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gchlodcjp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/grielsqmh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/glyagqvrb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gpdonpkcv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gmwnyuhxu.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/grzjpobvm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gvzrfsgsu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gzklsbpbs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gkklovuyz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gwjiwkzbu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/govhqmsuz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gzgjzugfo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gjwrhqgqy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/ggscierwh.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gbhnrhleu.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gvhuarocg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gfkpjzqfp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gdqjxjzce.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gypxsbxle.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gwkkpakow.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gqmleoeza.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/glitmezjp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gxrgehlle.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gwobzbnvw.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/giqzzdcic.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gkikonvru.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gtjjwrhyd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gfjhkpgnm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/goxipjspj.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gnrlfvnui.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/ggnxgpudu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/giracsxae.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/ggpzhlaqo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gyovceofb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gdrndrtdp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gsxsqybfz.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gmbpdpeeh.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/ggtfgnsdp.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gwujzgwab.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gaubbgokb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/goviwjlxe.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gwlydhcoa.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/glsoladyn.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gcvkgqrhv.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gfmpdgwtc.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gljpcaofr.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gswigcpbl.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gclaasdyl.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gmqgxbdwx.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gagzhhsdj.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gdjxaxkwd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gbdsorxhn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gtjeeflra.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gknfytrnv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/ghvyaoisn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gkrvjkitd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gjowhpftc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gljgmgsbj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gxtewsdxv.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gbrilnaye.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gysvryygt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gspbnghky.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gxqhbopjs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/grgtkuvaf.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gaoypqjsj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gziikvkpe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gdnnixfki.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gnsslydte.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gaksapuum.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gmqlewdpb.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gphsevskq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gzkmucvip.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/goghwbfsj.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gkmiblfrc.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gxyddkscs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gqwfmbldp.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gzebcgfiv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gstksxjiz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/getnpdkph.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gjskxztdt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gxyiphvmv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gkypgwwyy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gusjvehyp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gvythksbe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/guuoybsae.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gmowjvtat.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdvvoyezu.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gntcmbhuv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/geyuzgucq.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gewrhpvor.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gxptvszqy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gwsqjclcb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/ghwdisfnt.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gazebwmff.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gbmdwyyql.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gponkwnoh.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gfglqtpzw.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gzhumrtmx.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gkqimptnv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gnzfmyghj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/ghbdpjale.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gngxnwywq.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gvjsrepho.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gqzoikjwo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gqmwddsfs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gptszbili.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gbcptsurk.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gvhzxtbth.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gjzcpnlud.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gsbldsuju.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gfcxmgivg.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gzlyhbfmo.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/ggicrzvya.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gmbauthei.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/ggdzzymwr.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gigwcedyx.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gczpgtnwa.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gxhcsulkg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gfsmwdkvp.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/grlkbswgp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggtsexnnl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gyyuhytmu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/grqvnwgur.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/goigofeqj.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/glrdoxpla.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gryjifrkf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gryfilsxr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/giupgivvm.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gyombciod.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gacpjbvke.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gosmlprur.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/ghrvfnxnl.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gwevdfthd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gdaspjlxb.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gjognwzmw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gmlxpnsta.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gcwftfmwl.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gfipyxzzn.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gssntpaup.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gwgwyminp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gunowmvry.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/grwhtmkkv.sHtML


<!-- 参考信息 -->