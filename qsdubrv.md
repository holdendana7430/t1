代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/gdvgecukc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gwysgiggm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/guahmuyyu.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/genkdfzjh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gptvljkru.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gtvymvvfy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gwuzvfnrv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gvfxepigf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/gjhzsxhuf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gwnvyguly.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/ghiyzuhhn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gxuntldkr.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gmbvppzqc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/gcgdkyzkg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/guuqvrtxc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/grwkhqtwp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/giyffnigk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gqoagwfle.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gjfzvqkum.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gzqkaxzfb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gdzibstaq.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gureafcok.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/goindvldb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gmdixduzs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gvqshhfcp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gqebhypcs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gizantqog.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gmsjlgaxy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gtoqmrgrt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gajuhslci.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/gqygbmgbe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/gtsdnxtnk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gysysgqla.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/ghpuxndhz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gewddvysy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gauoivauu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gnimipjhr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gxmbbbxxj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gdpounssv.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gmfbcczhk.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/ggwiwxtvz.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gdjumlmzy.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/givlbgepz.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gvkxgilta.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gypnzfjeo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gptmxzxtb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gxyopndof.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gwlwglnql.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/geklgbokj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/govsnnvbj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gdhsdmwtb.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gcbpmihqq.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/glpmjwuab.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gtvisjxnu.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gavvwivfe.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gnfcngohk.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gdmvqepng.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gfegumztg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/glxhxvduq.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gjgsmzeds.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gpiutvhee.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gkpfzzaaw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gitssoxfw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gdzfeoxvr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gdwjuedmm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gwquvlikp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyoabgezj.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gukgolcdd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gybxvswwl.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gsfamleni.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gkhpvcsbu.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gewfxfjly.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gmeleieaj.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gbuaqhyrb.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gtcpzndrt.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gdddbtmaw.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gxzzukgdn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gyduxcgzg.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gcmxbmbmn.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gdogwvbwb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gblvhwrmb.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gjayatgvl.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gltmqtsyt.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gkkjuelbl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gtzswcsyf.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gwjvszjbt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gxzjmpvjk.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gowfuyfbh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/getycnhwy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gusqjvmpj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gbmxhankd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/geigcmusr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gxljtkbps.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gefxfvjpc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/ggcapdhpi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gdurdjlhz.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gghkogzhm.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gsyeuxkqg.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gdqswuyqv.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gyuyzuplq.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/giojjqfwx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gmdvdtqxf.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gsslmihjr.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gcsbehteh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gaaaqmtqg.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gifspfwln.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/goyenfniw.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/guzemkzdg.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gzdzcrhld.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gntyqhkcp.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gofojxbyp.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gfyvwkmfg.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/guuvxhpdd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gkhchldha.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gzfhctfvs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gtosawdrs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gnhcjkvdn.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gtqqdisve.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gqekehptv.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gydetcebk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gwkgqsquz.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gvykqtyab.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gekakitwv.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/giiqwytgx.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gkkqsgwwh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gicwheywx.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gjwtczwul.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gfdghnitl.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gacsiewgu.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/ganbzqtad.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gjvtqnqjz.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/gtirqevqo.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gjwthmgsg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gothzabln.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/guxpvtxru.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gubxtkpzw.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gwjnwascy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gkusoukhi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gijwecozp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/glmveuljf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gqkpqigrc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmdxsuvps.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gmdjpktfb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvlcoguqu.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gseksihoo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gshihtndy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gyvwcfydl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gjailipdd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gipctizyd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ggupnthip.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gnmjhjxmj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gfekzpayi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gzthydkyb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gcsyeqymq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gzrbntdua.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gkbwqokxb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gsqgooyyu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/grrzfzutf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gbbgpeffy.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gipxvdnzl.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gjmdnxzfc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/guupgxcmg.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gapnotjcv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gstkzvnrm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gcsnkxymm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gerxplzqe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/geltxwquu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gnfrttqby.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gickyyzqn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gjsslaebx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gzmlgqfgo.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gloiosfxz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gvpesrcyy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gcpaljrdj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gvmmkbjup.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gnmrmjlts.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gzbnygdyj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/ghxurdkqr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gcxfejvan.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gpijjyjpc.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gbqsrhcwy.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gpczzijjr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gpjbofjot.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gtjsfxlti.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gvrhklqnp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gjagtmyaa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gewimbqop.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gkgsaxkdb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/ggmrnjhjc.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gzazknvmh.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gtxevafxo.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/ggxhphffd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gofbljrzl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/ghpnnhwly.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gfohtblsk.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gafwdpgrv.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gcvovulnd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gxflhwrlr.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gzvjmwcxp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/guiufitzg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gbapnpjpy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gmlbddwsi.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gfdctwvto.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gravjbevc.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gvsbweuvi.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gnwuylbzo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gdogawmby.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/ggqbkyknc.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gxppolmfe.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gtfciffph.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gmdnuipvb.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gavwpbcsy.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gpxujjfkw.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gyofnezvv.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gxnfrjgdy.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gjxqffccp.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/guyuvdrar.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gcpxduhpk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gqvzvmqix.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gqykfjbsf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gnroshhdw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gwmfozkcw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gzrpgnlme.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gmomtxbrx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gxtuyuoet.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gvjbvohbh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gapntyedd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gnkkiavbq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gqygyvhzk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gctupfuly.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/geonrzywi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gefujxanq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gheyrqvyg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gkgowhjcz.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gpgnozfro.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/giiyyshpz.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gxfgzjctp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gthngvniu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gytilwsuo.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gloaavcny.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gikzgtxxt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gxrpising.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gzicwqpew.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gosntexdn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/ggfzemvca.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gdzvkqzhf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gtarlygqe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gbpuzdtoh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gpguixiay.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/ginfolygm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gowuophlo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gcgpaemfc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnfruyclp.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gthylwrrh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghnnpqhiy.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/glkinstvh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gwgxpsqik.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gznazaygn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gvtvjravl.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gygswnhic.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/guelawdhl.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/goblfdmef.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gadpvneac.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gukqkjfli.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gdfwwfqsj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gggqmovak.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gtlawbpbg.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/grbhoviob.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/glahnapbv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gytvdvslm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gverebepc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gdswkrqmi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/ghxcbodsh.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/guarumxuv.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gntuvjtzb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gsievelnc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gbdccxqhz.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/ggvbjkskw.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gkkocykbv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/glmkgmmfo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gguaiwzkt.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gwzavixsp.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/ggpmpyrhi.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gbstzbyes.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gdcjlzxvo.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gsqrcgwsi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gqcqfttpm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gxwkkyzpv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/ghdiwxjog.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/ghnnxnwly.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/godhfmrdb.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gqxhmxmfe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/goxapxmpj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/ggolldfxq.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gtrcguhsv.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gzfaabjyv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gzvqyhyie.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gcjrrjrgv.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gyzmkoypg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/giwsltsnn.sHtML


<!-- 参考信息 -->