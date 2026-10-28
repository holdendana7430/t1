代发 wailian999

Go:   encoding/gob
来源：http://hz.hfpthk.cn/gtqvbkzlbc.html

Ruby: Marshal.dump(obj)
来源：http://hz.yangfankeji.com/gtyvlgbrkz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yueranfly.top/gtmtyrcasj.html

================================================================================
来源：http://hz.yonumen.top/gttnppomgf.html

L. 网络请求
来源：http://hz.yuxming.cn/gtzgzdfumi.html

================================================================================
来源：http://hz.hammf.cn/gteyqeoomf.html

[L01] 发送 GET 请求
来源：http://hz.hywenlv.cn/gtqqefvfdx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gotoacloud.top/gtiukgdyqt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhijiandao.cn/gteulgxwpc.html

JS:   await fetch(url)
来源：http://hz.ydjk.org.cn/gttjuzmxmx.html

TS:   await fetch(url)
来源：http://hz.andypj.xyz/gtbkeuwmcz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.vqdsnc.cn/gtdoztzour.html

Go:   resp, err := http.Get(url)
来源：http://hz.jqgufenzy.top/gthjbtxcfc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sufxvd.cn/gtclqbinon.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.bjfxy.top/gtwvwhsspo.html

[L02] 发送 POST JSON
来源：http://hz.nwbrower.top/gtiokdjmqd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.316326.xyz/gtuyyxklzh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinqigfzy.top/gtmfyrnwvb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.redwolf501.top/gtxnsczkfx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nwbrower.top/gtqtxpcyxr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.chenjidiqi.icu/gtngbipvaq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shzxlz.cn/gtepywefor.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.tanke756.top/gtbqaxxjmu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.snrcjt.cn/gtcfzhnopy.html

[L03] 设置自定义请求头
来源：http://hz.yangfankeji.com/gtyaztrmzg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sxryk.cn/gtttimygdr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sweek.top/gtrrehxzcn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yangfankeji.com/gtdbxssvfn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shangyingyoupin.top/gteibxmbgq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ydzc1.top/gtkogmnxwn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shanyushiyangtech.top/gtmbdrpwky.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sweek.top/gtznoznexb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jqgfzy.top/gtkfnxtgtd.html

[L04] 设置超时
来源：http://hz.fengsongda.top/gtbrpbgyza.html

Py:   requests.get(url, timeout=5)
来源：http://hz.fengsongda.top/gtiaudomxr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.aizwys.cn/gtdsjwvryx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.havefunace.top/gtadktruao.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.vqdsnc.cn/gtsreffwvb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhaomingkeji.xyz/gtpinfqtkm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinqigfzy.top/gtgbzlmwpg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gzhubu.top/gtqqdpcjrb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shzxlz.cn/gtuqithlbp.html

[L05] 上传文件（multipart）
来源：http://hz.zdqjudy.top/gtsdfnmilk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.316326.xyz/gtionpqtxm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yuxming.cn/gtsrskujtb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenjidiqi.icu/gtkewmrwhp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgufenzy.top/gtjtnqlkiy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xuanzx.com/gtkatnuvno.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinqigufen.top/gtdjmszuxk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.aizwys.cn/gtxcaffwqz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hfpthk.cn/gtnzfsnbzl.html

[L06] 解析响应为 JSON
来源：http://hz.jinqigfzy.top/gtbqvugbqa.html

Py:   resp.json()
来源：http://hz.gogol.net.cn/gthbpdsdjv.html

PHP:  json_decode($body, true);
来源：http://hz.shuidangran.top/gtcoiasbfd.html

JS:   await resp.json()
来源：http://hz.jinqigufen.top/gtozvcaufw.html

TS:   await resp.json()
来源：http://hz.svipenyu.cn/gthfurpqoq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.daria6918.cn/gthcjxhxom.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jiagoushi.top/gtjypjwppo.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xylfe.cn/gtfykkbkdx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.fengsongda.top/gtsjhhzmkt.html

[L07] 处理 HTTP 状态码
来源：http://hz.havefunace.top/gtqfctmecs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.dianchejie.cn/gtajxeoqjy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhoulong.xyz/gtiouiijsf.html

JS:   resp.ok;  resp.status
来源：http://hz.nanxuanxn.top/gtbooaqmbw.html

TS:   resp.ok;  resp.status
来源：http://hz.zhaomingkeji.xyz/gtsyayptmn.html

Java: resp.statusCode()
来源：http://hz.fengsongda.top/gtcuycurkx.html

Go:   resp.StatusCode
来源：http://hz.fengsongda.top/gtzzozsnwk.html

Ruby: resp.code.to_i
来源：http://hz.jianghu66.top/gtepwviqyx.html

C#:   (int)resp.StatusCode
来源：http://hz.nanxinkj.top/gtuprcasae.html

[L08] 并发请求多个地址
来源：http://hz.yanxiufei.cn/gtsvlmridy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.pycfn.com/gtdifaejbl.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj202588.top/gtfiapvfov.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tian-w.cn/gtsyrjfzih.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aibaodan.cn/gtgymorylz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ehwqpu.com/gtbzhrxonz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhengqikj.top/gtyuucpdms.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.fengsongda.top/gtpeqqfwhf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.wangshuangyany.cn/gtmspdwwwq.html

================================================================================
来源：http://hz.iojbl.cn/gthqfcfkhl.html

M. 命令行 / 进程 / 环境
来源：http://hz.sysykeji.top/gtwskzfunt.html

================================================================================
来源：http://hz.yuxming.cn/gtvljofman.html

[M01] 读取命令行参数
来源：http://hz.fengsongda.top/gtrlrrtuvu.html

Py:   sys.argv[1:]
来源：http://hz.c1oappe.top/gtloitsszk.html

PHP:  $argv;  $argc;
来源：http://hz.zhaomingkeji.xyz/gtjmtjmbwx.html

JS:   process.argv.slice(2)
来源：http://hz.hnqzz.top/gtarboomzw.html

TS:   process.argv.slice(2)
来源：http://hz.shzxlz.cn/gtrimswgpz.html

Java: args 数组（main 方法参数）
来源：http://hz.cheryme.top/gttjektbzp.html

Go:   os.Args[1:]
来源：http://hz.gotoacloud.top/gtpwtcfnxk.html

Ruby: ARGV
来源：http://hz.meibo888.top/gtgqnyzjxp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.tanke756.top/gtbslmyljv.html

[M02] 读取环境变量
来源：http://hz.shzxlz.cn/gtabgdlilj.html

Py:   os.environ.get("HOME")
来源：http://hz.hongshengwenyu.top/gtlwofqtbn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hnxiangtu.top/gtebmegtpu.html

JS:   process.env.HOME
来源：http://hz.c1oappe.top/gttuthisrr.html

TS:   process.env.HOME
来源：http://hz.cqqwz.cn/gttczkbubl.html

Java: System.getenv("HOME")
来源：http://hz.jiagoushi.top/gtchdbtqqc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.nanxinkj.top/gtcgddsrdt.html

Ruby: ENV["HOME"]
来源：http://hz.gotoacloud.top/gtfmktjkid.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hammf.cn/gtbnvthwtc.html

[M03] 执行外部命令
来源：http://hz.ydjk.org.cn/gtqqalbuni.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cheryme.top/gtedemfufp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shanyushiyangkeji.top/gtbwnfuskt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.gzhubu.top/gtenqxtfmy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhixingplan.top/gtgfwerdih.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hnxiangtu.top/gtxotcjvth.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ydjk.org.cn/gtmclihmhp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.aizwys.cn/gtknuaiynq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ehwqpu.com/gtldezswfe.html

[M04] 获取当前工作目录
来源：http://hz.jinyuanbaomall.cn/gtercslwkq.html

Py:   os.getcwd()
来源：http://hz.yvedp.cn/gthihpdrxr.html

PHP:  getcwd();
来源：http://hz.zhixingplan.top/gtbwxjaafy.html

JS:   process.cwd()
来源：http://hz.jianghu66.top/gtisughdhl.html

TS:   process.cwd()
来源：http://hz.mhx1999.top/gtobirxhna.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.dianchejie.cn/gtvtbgsanu.html

Go:   os.Getwd()
来源：http://hz.ydjk.org.cn/gtamzxfxth.html

Ruby: Dir.pwd
来源：http://hz.c1oappe.top/gtjljxzbfm.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shanyushiyangtech.top/gtrijsskuj.html

[M05] 设置退出码
来源：http://hz.shanyushiyangkeji.top/gtrgukhtzw.html

Py:   sys.exit(1)
来源：http://hz.fengsongda.top/gtoggppdyo.html

PHP:  exit(1);
来源：http://hz.xinyue.icu/gttafoagme.html

JS:   process.exit(1)
来源：http://hz.yvedp.cn/gtihakowvj.html

TS:   process.exit(1)
来源：http://hz.ehwqpu.com/gtyxnxfrrt.html

Java: System.exit(1)
来源：http://hz.haohaochexian.top/gttzdnjoxu.html

Go:   os.Exit(1)
来源：http://hz.gotoacloud.top/gtkcbvqdrk.html

Ruby: exit 1
来源：http://hz.xuanzx.com/gtkboxcrlh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhiwuduotai.top/gthnauaejc.html

[M06] 向标准错误输出
来源：http://hz.wangdashe.top/gtfazgrevj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sysykeji.top/gtlmqwxyct.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.dashuyun.cn/gtcjnzeano.html

JS:   console.error("err")
来源：http://hz.pengpengdd.cyou/gtvztybedi.html

TS:   console.error("err")
来源：http://hz.yangfankeji.com/gtdredfbae.html

Java: System.err.println("err")
来源：http://hz.guannengcc.top/gtfuxjrhfl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jinqigfzy.top/gtpsjygklr.html

Ruby: warn "err"
来源：http://hz.jiagoushi.top/gtrswbnjmp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.aizwys.cn/gtldmtwzuq.html

[M07] 判断是否为主入口
来源：http://hz.haohaochexian.top/gtfxukdjuc.html

Py:   if __name__ == "__main__":
来源：http://hz.wangdashe.top/gtbxiemfhy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.pycfn.com/gtbaimuakm.html

JS:   require.main === module
来源：http://hz.snrcjt.cn/gtpjxglzne.html

TS:   require.main === module
来源：http://hz.cdnleiting.top/gtnlooideh.html

Java: public static void main(String[] args)
来源：http://hz.hysaishi.cn/gtzknmqyvn.html

Go:   func main()
来源：http://hz.sysykeji.top/gtppxgcwnk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.9152youxi.cn/gtwylxdkty.html

C#:   static void Main(string[] args)
来源：http://hz.hysaishi.cn/gtfgirgxvl.html

[M08] 获取系统与运行时信息
来源：http://hz.xinyue.icu/gtylhjphzn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shanyushiyangkeji.top/gtoivkdbmc.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yuxming.cn/gtrztckkjy.html

JS:   process.platform;  process.version
来源：http://hz.zhongyouzk.top/gtmziqwume.html

TS:   process.platform;  process.version
来源：http://hz.xylfe.cn/gtiugsntbk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.daxiang520.top/gtnxvuzgvp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.kuanghao11.cn/gthlzmpbmp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinqigufen.top/gtrrqkddns.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.kuanghao11.cn/gtkqpklmza.html

================================================================================
来源：http://hz.guowangkeji.top/gtaaoxndqo.html

N. 数据结构与算法
来源：http://hz.xinyue.icu/gtbvgqknuw.html

================================================================================
来源：http://hz.zhoulong.xyz/gtyuukbkel.html

[N01] 二分查找（有序数组）
来源：http://hz.havefunace.top/gtfyesexsj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xylfe.cn/gtmsyhylzn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gotoacloud.top/gtmqnxsrnx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.guowangkeji.top/gtglvusalf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigufen.top/gtielqdxrv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jqgfzy.top/gtkoayjxac.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinqigfzy.top/gtuzeragjw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.tanke756.top/gtoszpezra.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gogol.net.cn/gtbdymksyn.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.svipenyu.cn/gtzmxneamk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenjidiqi.icu/gtnxtqcejd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shanyushiyangkeji.top/gtmolblcsh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aizwys.cn/gtlxjzligz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinqigufen.top/gtmabkugza.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinqigfzy.top/gtjemzyeca.html

Go:   slices.Sort(arr)
来源：http://hz.shangyingyoupin.top/gtcgssjwyu.html

Ruby: arr.sort
来源：http://hz.shanyushiyangkeji.top/gtxvmzcjea.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shanyushiyangtech.top/gtadbepywo.html

[N03] 快速排序（分治示例）
来源：http://hz.sufxvd.cn/gtxmobwbwf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.wangshuangyany.cn/gtidysjjaa.html

PHP:  // 递归实现，或用 usort
来源：http://hz.smart0.xyz/gtygfoglzw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ybcxt.top/gtsvydgtus.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuanzhike.top/gtyrtddqcg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.fzhhl.top/gtgzuamyph.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yonumen.top/gtinjvmagm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.aizwys.cn/gtlemhlqhm.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.chenjidiqi.icu/gtjmftdoqv.html

[N04] 斐波那契数列
来源：http://hz.wangdashe.top/gtzweqbrhd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.0kj1m.cn/gtxunvekyd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xuanzx.com/gtljwocefn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yonumen.top/gtinixjkad.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnqzz.top/gtlpgjbftv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.chenlongwang.top/gtmqekekop.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.9152youxi.cn/gtcjhnlwhl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhoulong.xyz/gtboppnfkn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yongpay.top/gtyxqmkyuf.html

[N05] 最大公约数
来源：http://hz.xinyue.icu/gtfrleiici.html

Py:   math.gcd(a, b)
来源：http://hz.jianghu66.top/gttqisipxx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tianlin.xyz/gtuynvpgsn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hfpthk.cn/gtokroaxds.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnxiangtu.top/gttpkoklge.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ppjwa.cn/gtedagkplk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.snrcjt.cn/gtgjwmpovf.html

Ruby: a.gcd(b)
来源：http://hz.iojbl.cn/gtldewwbhl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yueranfly.top/gtwjiaensu.html

[N06] 判断回文字符串
来源：http://hz.hysaishi.cn/gtnxddntyz.html

Py:   s == s[::-1]
来源：http://hz.c1oappe.top/gtofuvpizq.html

PHP:  $s === strrev($s);
来源：http://hz.shangyingyoupin.top/gtaluarvvg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.aizwys.cn/gtnmosogho.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtgjjirrcy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.pycfn.com/gtzemndwak.html

Go:   // 双指针从两端比较
来源：http://hz.0kj1m.cn/gtyuyltvyq.html

Ruby: s == s.reverse
来源：http://hz.jinghuilouyu.cn/gtlqowlihg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhaomingkeji.xyz/gtjjysychf.html

[N07] 两数之和（返回下标）
来源：http://hz.yj20258888.top/gtkyooluyg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jyoumei.cn/gtkmhoesdl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shanyushiyangtech.top/gtpliwighp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.cdnleiting.top/gtadgppali.html

TS:   // 手写 Map<string, number>
来源：http://hz.hongshengwenyu.top/gthunxmglo.html

Java: // 手写 HashMap
来源：http://hz.svipenyu.cn/gtcnreiggh.html

Go:   // 手写 map[int]int
来源：http://hz.aizwys.cn/gtkdmwdywm.html

Ruby: // 手写 Hash
来源：http://hz.yj202588.top/gtnejgphzi.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhoulong.xyz/gtohgmgkzc.html

[N08] 生成全排列
来源：http://hz.gzhubu.top/gtgvoedkgf.html

Py:   itertools.permutations(arr)
来源：http://hz.vqdsnc.cn/gtkrvbxcqg.html

PHP:  // 手写递归交换
来源：http://hz.jianghu66.top/gtibsfehdo.html

JS:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtmnocpfei.html

TS:   // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtnuhdkwxo.html

Java: // 手写回溯递归
来源：http://hz.wangdashe.top/gthhofjofd.html

Go:   // 手写回溯递归
来源：http://hz.mhx1999.top/gtieryoezy.html

Ruby: arr.permutation.to_a
来源：http://hz.ydzc1.top/gtaojrjnsp.html

C#:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtcifnykcr.html

[N09] 栈与队列
来源：http://hz.shzxlz.cn/gtgautjswf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.bjfxy.top/gterexzsrt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yuanzhike.top/gtouyhkuow.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.meibo888.top/gtynrkumby.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yanxiufei.cn/gttctydaxt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zycfv.cn/gtkoxnahhi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ydjk.org.cn/gticlrgvnf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hywenlv.cn/gtemjpxapw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.pycfn.com/gtcysbwhsf.html

[N10] 链表节点定义
来源：http://hz.fengsongda.top/gtxadxxfxt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shuidangran.top/gtkkwyiwrh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.pengpengdd.cyou/gtjwfmreas.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jiagoushi.top/gtmucnxfcd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shzxlz.cn/gtbcevglnq.html

Java: class Node { int v; Node next; }
来源：http://hz.chenzaomai.com/gtdeiavtsa.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.kuanghao11.cn/gtutpbuppp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.kuanghao11.cn/gtgubyavdd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hnqzz.top/gtxraqicwf.html

[N11] 二叉树中序遍历
来源：http://hz.zhongyouzk.top/gtrbljlxlu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xinyue.icu/gtxxtqgxxw.html

PHP:  // 手写递归函数
来源：http://hz.cqqwz.cn/gtmciwlfhh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pengpengdd.cyou/gtknwbnvzw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ybcxt.top/gtfozuqojj.html

Java: // 手写递归
来源：http://hz.zhixingplan.top/gtaedyzrif.html

Go:   // 手写递归
来源：http://hz.jqgfzy.top/gtyceqcxdo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cdnleiting.top/gtjeghllle.html

C#:   // 手写递归
来源：http://hz.xuetiantiany.cn/gtzkgzzopw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhaomingkeji.xyz/gttppanpet.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ivvv.top/gtupkfhoev.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sufxvd.cn/gtrifrenac.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.haohaochexian.top/gtrzyupknb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cashguo.top/gttqxtjmvu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhixingplan.top/gtsksdfoya.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ehwqpu.com/gtegribyxp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xuetiantiany.cn/gtitneplhh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nwbrower.top/gttlpznvfb.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtkjpfxdho.html

O. 并发与异步
来源：http://hz.zycfv.cn/gtoclxrcmu.html

================================================================================
来源：http://hz.yonumen.top/gtzbzzqxtm.html

[O01] 启动一个线程
来源：http://hz.0kj1m.cn/gtchvaplgo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cheryme.top/gtliiblwks.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.wangshuangyany.cn/gtajjbsqxk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.birdmap.top/gtalazaipj.html

TS:   // 同 JS
来源：http://hz.jinqigfzy.top/gthvgvzxfu.html

Java: new Thread(() -> f()).start()
来源：http://hz.hnqzz.top/gtvlpltsxx.html

Go:   go f()
来源：http://hz.yanxiufei.cn/gteokvfqsj.html

Ruby: Thread.new { f }
来源：http://hz.hfpthk.cn/gtvpiqspgr.html

C#:   Task.Run(() => F());
来源：http://hz.kuanghao11.cn/gtyeesrbbs.html

[O02] 使用线程池
来源：http://hz.pycfn.com/gtkwzyyhdy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xylfe.cn/gtxuuegunb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.guowangkeji.top/gtnziehxam.html

JS:   // worker_threads 线程池
来源：http://hz.gogol.net.cn/gtyksfkweu.html

TS:   // worker_threads 线程池
来源：http://hz.chenjidiqi.icu/gtwdtxzlwg.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yanxiufei.cn/gtvxfqohkp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cashguo.top/gtpzptebcm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.aibaodan.cn/gtgfwrawvq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.vqdsnc.cn/gtggsiwhrg.html

[O03] 加锁保护共享数据
来源：http://hz.cucudq.cn/gtbthkzxhr.html

Py:   with lock: shared += 1
来源：http://hz.ppjwa.cn/gtvsdjamfe.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.mhx1999.top/gtnvfdefph.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.sufxvd.cn/gttayeuxoj.html

TS:   // 同 JS
来源：http://hz.jqgufenzy.top/gtjguudmgg.html

Java: synchronized (this) { shared++; }
来源：http://hz.hysaishi.cn/gtmvsvhujc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.fzhhl.top/gtbrwjecew.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ivvv.top/gthpeowivh.html

C#:   lock (gate) { shared++; }
来源：http://hz.hongshengwenyu.top/gtfkcczrxs.html

[O04] 定义异步函数并等待
来源：http://hz.tianlin.xyz/gtfqgikpuo.html

Py:   async def f():⏎    await g()
来源：http://hz.aibaodan.cn/gtmoorfzhm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.daria6918.cn/gtznvhbyhq.html

JS:   async function f() { await g(); }
来源：http://hz.cdnleiting.top/gtwwfighzi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yuxming.cn/gtvcjvfzqc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhengqikj.top/gtpjvnioju.html


<!-- 参考信息 -->