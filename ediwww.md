代发 wailian999

L. 网络请求
来源：http://hz.xingfuxueyuan.xyz/gtkwbatnor.html

================================================================================
来源：http://hz.jyoumei.cn/gtgtorlagh.html

[L01] 发送 GET 请求
来源：http://hz.feifeiyinyue.top/gtrdkkxdnd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yonumen.top/gtetdwwruq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gogol.net.cn/gtgpshkgyj.html

JS:   await fetch(url)
来源：http://hz.tanke756.top/gtuglcqbce.html

TS:   await fetch(url)
来源：http://hz.cheryme.top/gtbvnnprhu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cheryme.top/gtzwqmbspo.html

Go:   resp, err := http.Get(url)
来源：http://hz.meibo888.top/gtdnahvbjk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.c1oappe.top/gtoesawglm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhaomingkeji.xyz/gtjquvfrvg.html

[L02] 发送 POST JSON
来源：http://hz.316326.xyz/gtcjaqeilf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.kuanghao11.cn/gtakdzvcxl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.tian-w.cn/gtjffdjtlp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenzaomai.com/gtbalggspu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cashguo.top/gtwteupjpm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.nwbrower.top/gtoidyhtqp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.guowangkeji.top/gtysvbludg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xingfuxueyuan.xyz/gtgwhehpcj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jlsjyb.cn/gttmfjwspm.html

[L03] 设置自定义请求头
来源：http://hz.dianchejie.cn/gtqneyqrzj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yanxiufei.cn/gtjeozivwc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jqgufenzy.top/gtbeukyiqv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shangyingyoupin.top/gtvdocaygy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sufxvd.cn/gtxjhgnvdl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.aibaodan.cn/gtlqxfvobz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.tanke756.top/gtzprfxgyd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhixingplan.top/gtbwssgagy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shuidangran.top/gtzjtzkylx.html

[L04] 设置超时
来源：http://hz.yanxiufei.cn/gtbsvqbvwm.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xziqi.cn/gtkjtubope.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xinyue.icu/gttilnmnis.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ydjk.org.cn/gttrjqlsqi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.birdmap.top/gteduzxlru.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ehwqpu.com/gtwwjazjhq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.fzhhl.top/gtwpxbnzdr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhongyouzk.top/gtlcfbtllb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.snrcjt.cn/gtbrqxxwyc.html

[L05] 上传文件（multipart）
来源：http://hz.yonumen.top/gtqpfgfkqq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yueranfly.top/gttlajnrkl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.aizwys.cn/gtqxadvvug.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhengqikj.top/gtxacdjdkm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sxryk.cn/gtamogshmu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhoulong.xyz/gtkonwgelr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nanxuanxn.top/gtfveujvnh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.andypj.xyz/gtchcnpdko.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shzxlz.cn/gtmnzhxqso.html

[L06] 解析响应为 JSON
来源：http://hz.cheryme.top/gtypprytqz.html

Py:   resp.json()
来源：http://hz.ydjk.org.cn/gtpwnfmedd.html

PHP:  json_decode($body, true);
来源：http://hz.gzhubu.top/gtjrhymghg.html

JS:   await resp.json()
来源：http://hz.ybcxt.top/gtctaolyic.html

TS:   await resp.json()
来源：http://hz.sxryk.cn/gtzwwhpiya.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zycfv.cn/gtijpevocn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.smart0.xyz/gtwanhgurc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xylfe.cn/gtfqtyjxfo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.9152youxi.cn/gtwswfjlex.html

[L07] 处理 HTTP 状态码
来源：http://hz.andypj.xyz/gtykwqzsbk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhijiandao.cn/gtkyybkimn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhixingplan.top/gtpodrytte.html

JS:   resp.ok;  resp.status
来源：http://hz.pycfn.com/gtvylhsbxz.html

TS:   resp.ok;  resp.status
来源：http://hz.quarkkingdee.top/gtmpgiybjy.html

Java: resp.statusCode()
来源：http://hz.yj202588.top/gtzmzgmrkw.html

Go:   resp.StatusCode
来源：http://hz.tanke756.top/gtpkcuedai.html

Ruby: resp.code.to_i
来源：http://hz.jqgufenzy.top/gtspskfqpg.html

C#:   (int)resp.StatusCode
来源：http://hz.fengsongda.top/gtqnwdrgfh.html

[L08] 并发请求多个地址
来源：http://hz.tian-w.cn/gtwmipeqmw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.bjfxy.top/gtdjkgvdct.html

PHP:  curl_multi_init() 系列
来源：http://hz.kuanghao11.cn/gtrdmimfyp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgfzy.top/gtteoyeyjv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtetrddexx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tianlin.xyz/gtcnkvmver.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yj20258.top/gtegvvytef.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.redwolf501.top/gtqpndegpn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.pengpengdd.cyou/gtwwcxsuis.html

================================================================================
来源：http://hz.sweek.top/gtkfswzgwr.html

M. 命令行 / 进程 / 环境
来源：http://hz.aizwys.cn/gtbgryeqlb.html

================================================================================
来源：http://hz.jqgufenzy.top/gtrihqsjks.html

[M01] 读取命令行参数
来源：http://hz.cdnleiting.top/gtrknpykeb.html

Py:   sys.argv[1:]
来源：http://hz.yj202588.top/gtnummdiws.html

PHP:  $argv;  $argc;
来源：http://hz.0kj1m.cn/gtwlxycxpu.html

JS:   process.argv.slice(2)
来源：http://hz.zhengqikj.top/gtwqzpxtbq.html

TS:   process.argv.slice(2)
来源：http://hz.xingfuxueyuan.xyz/gtdoxycduo.html

Java: args 数组（main 方法参数）
来源：http://hz.ivvv.top/gtjqgreepk.html

Go:   os.Args[1:]
来源：http://hz.mhx1999.top/gtcfqbocvo.html

Ruby: ARGV
来源：http://hz.zhijiandao.cn/gtobnpypef.html

C#:   args 数组（Main 方法参数）
来源：http://hz.bjfxy.top/gtieyapgqy.html

[M02] 读取环境变量
来源：http://hz.meibo888.top/gttscnlvsa.html

Py:   os.environ.get("HOME")
来源：http://hz.hnxiangtu.top/gtirzribdg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinyuanbaomall.cn/gtcabknwke.html

JS:   process.env.HOME
来源：http://hz.zhaomingkeji.xyz/gtuwrzerwn.html

TS:   process.env.HOME
来源：http://hz.shuidangran.top/gtudzzjona.html

Java: System.getenv("HOME")
来源：http://hz.gogol.net.cn/gtlkuuhkft.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ppjwa.cn/gtwpllawlh.html

Ruby: ENV["HOME"]
来源：http://hz.xylfe.cn/gtwjqxoqju.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.daxiang520.top/gtzcteebnc.html

[M03] 执行外部命令
来源：http://hz.c1oappe.top/gtjlybxodb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.daxiang520.top/gtugoaiefe.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.0kj1m.cn/gtoquhmcwa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sweek.top/gterjulbbd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.quarkkingdee.top/gtywlsdwnh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yuxming.cn/gtagzyyuhp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.nanxinkj.top/gtncgozkrs.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jyoumei.cn/gtuokorlsv.html

C#:   Process.Start("ls", "-l");
来源：http://hz.guannengcc.top/gtswwszaau.html

[M04] 获取当前工作目录
来源：http://hz.xuanzx.com/gtrbjtsikg.html

Py:   os.getcwd()
来源：http://hz.birdmap.top/gtctksirme.html

PHP:  getcwd();
来源：http://hz.jqgufenzy.top/gtjjdzudwz.html

JS:   process.cwd()
来源：http://hz.zhijiandao.cn/gtodzguxll.html

TS:   process.cwd()
来源：http://hz.bjfxy.top/gtcnjzzanj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.52xcode.cn/gtdxmaoyhw.html

Go:   os.Getwd()
来源：http://hz.fengsongda.top/gtyicaelyy.html

Ruby: Dir.pwd
来源：http://hz.birdmap.top/gtsgidyahy.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sufxvd.cn/gtfeopvcpn.html

[M05] 设置退出码
来源：http://hz.xingfuxueyuan.xyz/gtfglivola.html

Py:   sys.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtcgmjvcdy.html

PHP:  exit(1);
来源：http://hz.zhaomingkeji.xyz/gtollckstv.html

JS:   process.exit(1)
来源：http://hz.haohaochexian.top/gtmaequdba.html

TS:   process.exit(1)
来源：http://hz.nanxuanxn.top/gtijgfhzux.html

Java: System.exit(1)
来源：http://hz.jinqigfzy.top/gtivbciuhj.html

Go:   os.Exit(1)
来源：http://hz.xuetiantiany.cn/gtskbwipgg.html

Ruby: exit 1
来源：http://hz.yueranfly.top/gtzghruewc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.feifeiyinyue.top/gtzywyatng.html

[M06] 向标准错误输出
来源：http://hz.bjfxy.top/gtznzajmtr.html

Py:   print("err", file=sys.stderr)
来源：http://hz.aizwys.cn/gtrqdgzyot.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sweek.top/gtdmdpshlz.html

JS:   console.error("err")
来源：http://hz.yuanzhike.top/gtiaayvcmd.html

TS:   console.error("err")
来源：http://hz.xylfe.cn/gtdapbhfie.html

Java: System.err.println("err")
来源：http://hz.hammf.cn/gtnacqvnba.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hysaishi.cn/gtjrqhysrt.html

Ruby: warn "err"
来源：http://hz.nwbrower.top/gthxxaglok.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ybcxt.top/gtxzzvcvrl.html

[M07] 判断是否为主入口
来源：http://hz.mhx1999.top/gtutapnkgm.html

Py:   if __name__ == "__main__":
来源：http://hz.chenzaomai.com/gtdocgbtzb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jlsjyb.cn/gtmjkrdeqc.html

JS:   require.main === module
来源：http://hz.dashuyun.cn/gtoiqkeiyc.html

TS:   require.main === module
来源：http://hz.redwolf501.top/gtdfdngogh.html

Java: public static void main(String[] args)
来源：http://hz.haohaochexian.top/gthybohkmf.html

Go:   func main()
来源：http://hz.zhoulong.xyz/gtqwtwrrjp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinqigufen.top/gtnrdmshpf.html

C#:   static void Main(string[] args)
来源：http://hz.ydzc1.top/gtnktiffjx.html

[M08] 获取系统与运行时信息
来源：http://hz.nwbrower.top/gtivubjeed.html

Py:   platform.system();  platform.python_version()
来源：http://hz.meibo888.top/gtgxlauprn.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhengqikj.top/gtdmyxovxw.html

JS:   process.platform;  process.version
来源：http://hz.cqqwz.cn/gtpkkjmxgo.html

TS:   process.platform;  process.version
来源：http://hz.hammf.cn/gtknxopbzu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yongpay.top/gtrgrmxasi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.fzhhl.top/gtaptemgym.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xylfe.cn/gtxpudykrx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.quarkkingdee.top/gtdtgbmcmm.html

================================================================================
来源：http://hz.zhoulong.xyz/gtzhuteoyt.html

N. 数据结构与算法
来源：http://hz.redwolf501.top/gtzruiomac.html

================================================================================
来源：http://hz.ybcxt.top/gtojtycvwk.html

[N01] 二分查找（有序数组）
来源：http://hz.hnxiangtu.top/gtbehatweb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.dashuyun.cn/gttouuimjl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yangfankeji.com/gtwxpytotz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shzxlz.cn/gtikltiula.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhixingplan.top/gtavbnoehu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hammf.cn/gtoyochfjh.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.aizwys.cn/gthjzaqfiw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jqgufenzy.top/gtwhupvtxp.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.daria6918.cn/gtxuweyvkp.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.mhx1999.top/gtdhercguc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhaomingkeji.xyz/gtxfffgufh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sweek.top/gtyskhyhmb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenzaomai.com/gtqkwrmwaf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ppjwa.cn/gtdhubsdps.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.fzhhl.top/gtzramxycv.html

Go:   slices.Sort(arr)
来源：http://hz.cqqwz.cn/gtzhugnmck.html

Ruby: arr.sort
来源：http://hz.shanyushiyangtech.top/gtobjxtwvd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hnxiangtu.top/gtovpygmfq.html

[N03] 快速排序（分治示例）
来源：http://hz.fzhhl.top/gtzuzthryi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.fzhhl.top/gtedibifpl.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tian-w.cn/gtmiflveyd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.0kj1m.cn/gtmemebltb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cucudq.cn/gtgdwpxiir.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinqigfzy.top/gticwdqzcm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.quarkkingdee.top/gtiijuoawm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.tian-w.cn/gtbsrwsase.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.fengsongda.top/gtnmaglojw.html

[N04] 斐波那契数列
来源：http://hz.gaohongyu789.top/gtscazjrjh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shuidangran.top/gtlmcypuho.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhixingplan.top/gtvyncozbx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hammf.cn/gtyskgklrq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhongyouzk.top/gtbjrayyrr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.fengsongda.top/gtvvpfmotn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.c1oappe.top/gtmrsdhxos.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cdnleiting.top/gtgivhiwpx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.feifeiyinyue.top/gtfhnjaaxk.html

[N05] 最大公约数
来源：http://hz.yuxming.cn/gtaibylsku.html

Py:   math.gcd(a, b)
来源：http://hz.zdqjudy.top/gtpamdygjw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jqgfzy.top/gtgnemvwez.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hammf.cn/gtvtfrqrfy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydjk.org.cn/gtlpseuxvu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.andypj.xyz/gthhjzittp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jianghu66.top/gtgrvyivqy.html

Ruby: a.gcd(b)
来源：http://hz.yj20258.top/gtupatzuli.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.0kj1m.cn/gtburiszst.html

[N06] 判断回文字符串
来源：http://hz.vqdsnc.cn/gtcblylbzk.html

Py:   s == s[::-1]
来源：http://hz.jinghuilouyu.cn/gtmyxmiqfd.html

PHP:  $s === strrev($s);
来源：http://hz.yj20258888.top/gtvkqjtgoi.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhijiandao.cn/gthdsxgrnl.html

TS:   s === [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtpzuqnidv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.kuanghao11.cn/gtxdenesbs.html

Go:   // 双指针从两端比较
来源：http://hz.sweek.top/gtozskhokg.html

Ruby: s == s.reverse
来源：http://hz.shzxlz.cn/gtkdzagkfl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinqigfzy.top/gtgmumjens.html

[N07] 两数之和（返回下标）
来源：http://hz.xuanzx.com/gtxqpheske.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.aibaodan.cn/gtahyiqued.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hysaishi.cn/gtjhrhsqqh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jlsjyb.cn/gtwrjgfysm.html

TS:   // 手写 Map<string, number>
来源：http://hz.dianchejie.cn/gtbqkilxfo.html

Java: // 手写 HashMap
来源：http://hz.yj20258888.top/gtxyygfjvg.html

Go:   // 手写 map[int]int
来源：http://hz.yueranfly.top/gtmjupythb.html

Ruby: // 手写 Hash
来源：http://hz.aizwys.cn/gtkbiwvpwv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.meibo888.top/gtpxqnwjkp.html

[N08] 生成全排列
来源：http://hz.ydjk.org.cn/gtqvqnocea.html

Py:   itertools.permutations(arr)
来源：http://hz.zhoulong.xyz/gtumpgdzty.html

PHP:  // 手写递归交换
来源：http://hz.gaohongyu789.top/gtfrrqeouy.html

JS:   // 手写回溯递归
来源：http://hz.jqgufenzy.top/gtgvappaqg.html

TS:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtxhzwfxxn.html

Java: // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtvhipspdk.html

Go:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtogioqjzd.html

Ruby: arr.permutation.to_a
来源：http://hz.wangdashe.top/gtwmaupokl.html

C#:   // 手写回溯递归
来源：http://hz.cqqwz.cn/gtyqxucgjb.html

[N09] 栈与队列
来源：http://hz.zdqjudy.top/gtcdycsctu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jianghu66.top/gtfjcehvyu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.dianchejie.cn/gtbdklvytt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.gogol.net.cn/gtpaqteary.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xziqi.cn/gtmlbtioaq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.feifeiyinyue.top/gtwkrrklhp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xuetiantiany.cn/gtvrkrpyhu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhongyouzk.top/gtuyflcexn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhaomingkeji.xyz/gtinpwznrr.html

[N10] 链表节点定义
来源：http://hz.yj20258.top/gtnkxrxfdq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hnqzz.top/gtupqtqtod.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.guannengcc.top/gtdnujhswp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yonumen.top/gtuoogqegk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hfpthk.cn/gtagfcruxn.html

Java: class Node { int v; Node next; }
来源：http://hz.yanxiufei.cn/gtiletsmdz.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.nwbrower.top/gtkdwmxfeh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.tian-w.cn/gtdkxanyxa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yongpay.top/gtdtjchjut.html

[N11] 二叉树中序遍历
来源：http://hz.cucudq.cn/gtjrfqznyg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yonumen.top/gthgceyqoc.html

PHP:  // 手写递归函数
来源：http://hz.ydjk.org.cn/gtvllrmgfh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hfpthk.cn/gtatijojav.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sysykeji.top/gtoxqgnvxs.html

Java: // 手写递归
来源：http://hz.ivvv.top/gtdcpvtvnl.html

Go:   // 手写递归
来源：http://hz.daria6918.cn/gtbqxoysdy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shanyushiyangtech.top/gthqnwnknl.html

C#:   // 手写递归
来源：http://hz.guowangkeji.top/gtmlmxacqn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cheryme.top/gtfbxbtvai.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.aizwys.cn/gtubkkvdhg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.0kj1m.cn/gtikuzsjqn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgufenzy.top/gtnsqvftlo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinyuanbaomall.cn/gtkkqvowdr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.0kj1m.cn/gtbsgwdqpd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.havefunace.top/gtefuqcmpc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.guannengcc.top/gtpkbkhlmv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ehwqpu.com/gtmsruvgup.html

================================================================================
来源：http://hz.jlsjyb.cn/gtfnrsgdji.html

O. 并发与异步
来源：http://hz.daria6918.cn/gthralvmev.html

================================================================================
来源：http://hz.cqqwz.cn/gtdtudvlaz.html

[O01] 启动一个线程
来源：http://hz.jinyuanbaomall.cn/gtsiktftee.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.nwbrower.top/gtbxhwesfp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.redwolf501.top/gtthiliuld.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.andypj.xyz/gttdmskmln.html

TS:   // 同 JS
来源：http://hz.yongpay.top/gtvfudrfiy.html

Java: new Thread(() -> f()).start()
来源：http://hz.cqqwz.cn/gtwfohszsd.html

Go:   go f()
来源：http://hz.aibaodan.cn/gtwylwxxvd.html

Ruby: Thread.new { f }
来源：http://hz.aizwys.cn/gtltjyyhif.html

C#:   Task.Run(() => F());
来源：http://hz.hysaishi.cn/gttghetgmh.html

[O02] 使用线程池
来源：http://hz.ybcxt.top/gtkdmbjkyd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xziqi.cn/gtekaxuhxy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shangyingyoupin.top/gtuxmypvpp.html

JS:   // worker_threads 线程池
来源：http://hz.zhiwuduotai.top/gtbsfsuazi.html

TS:   // worker_threads 线程池
来源：http://hz.hfpthk.cn/gtuvwifjis.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.c1oappe.top/gtapibsvmj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ehwqpu.com/gtcjimqpwa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.nanxinkj.top/gtrlynnvkp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.daria6918.cn/gtkflvqeux.html

[O03] 加锁保护共享数据
来源：http://hz.birdmap.top/gtmolldiui.html

Py:   with lock: shared += 1
来源：http://hz.meibo888.top/gttubjulsm.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.haohaochexian.top/gtgurxqbcp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cheryme.top/gtmzcncxrg.html

TS:   // 同 JS
来源：http://hz.iojbl.cn/gtqclwbvjn.html

Java: synchronized (this) { shared++; }
来源：http://hz.xuetiantiany.cn/gtnbeyzfgo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.birdmap.top/gtchpqslja.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhijiandao.cn/gtuesuufvs.html

C#:   lock (gate) { shared++; }
来源：http://hz.hongshengwenyu.top/gtakvxtsxq.html

[O04] 定义异步函数并等待
来源：http://hz.kuanghao11.cn/gtpoqwfefe.html

Py:   async def f():⏎    await g()
来源：http://hz.smart0.xyz/gtjzstcjfz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ywan-chungtsiang.top/gtohffbbik.html

JS:   async function f() { await g(); }
来源：http://hz.ybcxt.top/gtmhicucug.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.nanxinkj.top/gtwnevcoel.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cashguo.top/gtjgryekdc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sweek.top/gtalgddonc.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ydjk.org.cn/gtocfafpcx.html

C#:   async Task F() { await G(); }
来源：http://hz.sysykeji.top/gtinjbgsvy.html

[O05] 并发执行并等待全部完成
来源：http://hz.jiagoushi.top/gtobmmqsdn.html


<!-- 参考信息 -->