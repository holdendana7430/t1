代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://hz.sxryk.cn/gtyfgkdqvq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhiwuduotai.top/gtrmvamlsd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.tianlin.xyz/gtyjwsfccf.html

[L02] 发送 POST JSON
来源：http://hz.nanxinkj.top/gtpcsrggrv.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.wangshuangyany.cn/gtyjgtbucn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hnqzz.top/gtwsuzftwm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.smart0.xyz/gtoocuyxuf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fzhhl.top/gtewkxtjni.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hfpthk.cn/gtdzymzzor.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhengqikj.top/gtjtqoxfzr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jianghu66.top/gtqmnqelry.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sweek.top/gtsodvyhsd.html

[L03] 设置自定义请求头
来源：http://hz.daria6918.cn/gtkeinphts.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.feifeiyinyue.top/gtkagnyqim.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.tanke756.top/gtjhsmcfuk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shzxlz.cn/gtuymricrm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nwbrower.top/gtnyyimjhw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.vqdsnc.cn/gtqiabdmak.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.9152youxi.cn/gtwtveeajb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hysaishi.cn/gtzbnswmfh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shzxlz.cn/gteohiylhw.html

[L04] 设置超时
来源：http://hz.jqgufenzy.top/gtcyltoufn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xuanzx.com/gtknbdgabe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinqigfzy.top/gtmxxiwgtk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xziqi.cn/gtnrupbxil.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.andypj.xyz/gtbykdgsks.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sweek.top/gtrfskmsiq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.vqdsnc.cn/gtmyszlrhz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.c1oappe.top/gtuzfbdjxr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yj20258888.top/gtwcemcjoy.html

[L05] 上传文件（multipart）
来源：http://hz.redwolf501.top/gtvszajbky.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.fzhhl.top/gtdsvxyejc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.redwolf501.top/gttxhzduxz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.fengsongda.top/gtrjrmtkuk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.haohaochexian.top/gtbtfrhaab.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cheryme.top/gtmpkhwsdv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.andypj.xyz/gtmilzvque.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cdnleiting.top/gtfztkqnjn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj202588.top/gtdwuobxcw.html

[L06] 解析响应为 JSON
来源：http://hz.hysaishi.cn/gtaldavern.html

Py:   resp.json()
来源：http://hz.hfpthk.cn/gtbkrevjra.html

PHP:  json_decode($body, true);
来源：http://hz.daxiang520.top/gtwjylyruy.html

JS:   await resp.json()
来源：http://hz.shuidangran.top/gtwjbxvfef.html

TS:   await resp.json()
来源：http://hz.pycfn.com/gtinibmwyd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.svipenyu.cn/gtgjjjpcbb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.tian-w.cn/gtgvbhajjj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cashguo.top/gtnssnlhbe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ywan-chungtsiang.top/gtztxdzurt.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhijiandao.cn/gtwvytkdlp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xziqi.cn/gtddurnbii.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hysaishi.cn/gtskzwjdps.html

JS:   resp.ok;  resp.status
来源：http://hz.ydzc1.top/gtwaxltbkm.html

TS:   resp.ok;  resp.status
来源：http://hz.guannengcc.top/gtqtclahzs.html

Java: resp.statusCode()
来源：http://hz.yueranfly.top/gtwvldejyt.html

Go:   resp.StatusCode
来源：http://hz.yuxming.cn/gtfgfycvmk.html

Ruby: resp.code.to_i
来源：http://hz.hfpthk.cn/gtuwcuzrbn.html

C#:   (int)resp.StatusCode
来源：http://hz.jinqigfzy.top/gtwuwjxzev.html

[L08] 并发请求多个地址
来源：http://hz.wangshuangyany.cn/gtrdjfzcgv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xylfe.cn/gtscwxgzif.html

PHP:  curl_multi_init() 系列
来源：http://hz.xingfuxueyuan.xyz/gtinhsnoqg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuxming.cn/gtgotxiajh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yongpay.top/gtnjecxrqn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ywan-chungtsiang.top/gtcfjsvzaf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tanke756.top/gtbkarvgka.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.dianchejie.cn/gthxacjnhz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.wangshuangyany.cn/gthfpcugyp.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtarfnmmsx.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhixingplan.top/gtwwopsgoh.html

================================================================================
来源：http://hz.andypj.xyz/gtkhnnwpow.html

[M01] 读取命令行参数
来源：http://hz.shangyingyoupin.top/gtkbntdlna.html

Py:   sys.argv[1:]
来源：http://hz.ivvv.top/gtgnxrwsqt.html

PHP:  $argv;  $argc;
来源：http://hz.tian-w.cn/gtgsbrhlde.html

JS:   process.argv.slice(2)
来源：http://hz.ywan-chungtsiang.top/gtxdgitdso.html

TS:   process.argv.slice(2)
来源：http://hz.c1oappe.top/gtqqcclrcb.html

Java: args 数组（main 方法参数）
来源：http://hz.zhengqikj.top/gtxfsxlnnx.html

Go:   os.Args[1:]
来源：http://hz.daria6918.cn/gtdktscmow.html

Ruby: ARGV
来源：http://hz.dashuyun.cn/gtsieivrvu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenlongwang.top/gtrtxrpuvd.html

[M02] 读取环境变量
来源：http://hz.yanxiufei.cn/gtjistiemi.html

Py:   os.environ.get("HOME")
来源：http://hz.xuanzx.com/gteqtrzfbz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.fengsongda.top/gtgqnnxxkw.html

JS:   process.env.HOME
来源：http://hz.sxryk.cn/gtaipridst.html

TS:   process.env.HOME
来源：http://hz.zhiwuduotai.top/gtlxwkkecu.html

Java: System.getenv("HOME")
来源：http://hz.hnqzz.top/gtrefoozcg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yvedp.cn/gtpprflovv.html

Ruby: ENV["HOME"]
来源：http://hz.ivvv.top/gtibuvxfuw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xingfuxueyuan.xyz/gtwgcntwnh.html

[M03] 执行外部命令
来源：http://hz.shanyushiyangtech.top/gtwvythqmc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hammf.cn/gtkgenonem.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zdqjudy.top/gtebonpakt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.aizwys.cn/gtjbcxpeta.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shangyingyoupin.top/gtizuqnrzu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.pengpengdd.cyou/gttddwanil.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shanyushiyangtech.top/gtkgkmmhgi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hammf.cn/gtkjzludug.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yvedp.cn/gtquyuqvca.html

[M04] 获取当前工作目录
来源：http://hz.zdqjudy.top/gttluangeh.html

Py:   os.getcwd()
来源：http://hz.feifeiyinyue.top/gtpnywojye.html

PHP:  getcwd();
来源：http://hz.xuanzx.com/gtsatbqnyi.html

JS:   process.cwd()
来源：http://hz.chenzaomai.com/gtleoulvdb.html

TS:   process.cwd()
来源：http://hz.zhixingplan.top/gtvnetuoal.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yuanzhike.top/gtusjegfco.html

Go:   os.Getwd()
来源：http://hz.aizwys.cn/gtsnsydfcv.html

Ruby: Dir.pwd
来源：http://hz.jinqigufen.top/gtkvjcuhno.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhixingplan.top/gtwksxdlof.html

[M05] 设置退出码
来源：http://hz.ehwqpu.com/gtetnjcgoc.html

Py:   sys.exit(1)
来源：http://hz.jqgufenzy.top/gtzdrwdzww.html

PHP:  exit(1);
来源：http://hz.ppjwa.cn/gtrrlelsxx.html

JS:   process.exit(1)
来源：http://hz.guowangkeji.top/gtnszzspym.html

TS:   process.exit(1)
来源：http://hz.jiagoushi.top/gtxdvqklew.html

Java: System.exit(1)
来源：http://hz.aibaodan.cn/gtbfiqbsap.html

Go:   os.Exit(1)
来源：http://hz.sysykeji.top/gtqmdmhioz.html

Ruby: exit 1
来源：http://hz.bjfxy.top/gtqihqczgq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.fzhhl.top/gtaeceyaxz.html

[M06] 向标准错误输出
来源：http://hz.zhijiandao.cn/gtbzjykgql.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shangyingyoupin.top/gtqcedjxpj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinqigufen.top/gtyszwozyj.html

JS:   console.error("err")
来源：http://hz.cqqwz.cn/gtznhbpvpg.html

TS:   console.error("err")
来源：http://hz.chenlongwang.top/gtfttphmse.html

Java: System.err.println("err")
来源：http://hz.hfpthk.cn/gtfjisbobt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhengqikj.top/gtapignzqc.html

Ruby: warn "err"
来源：http://hz.redwolf501.top/gtfblswyku.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhijiandao.cn/gtlrayxflu.html

[M07] 判断是否为主入口
来源：http://hz.nwbrower.top/gtodjrhyak.html

Py:   if __name__ == "__main__":
来源：http://hz.chenlongwang.top/gtxgsvxdzq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.fengsongda.top/gtzetslxnp.html

JS:   require.main === module
来源：http://hz.feifeiyinyue.top/gtnitcjuuo.html

TS:   require.main === module
来源：http://hz.sysykeji.top/gtfjvezgro.html

Java: public static void main(String[] args)
来源：http://hz.0kj1m.cn/gtdaeqsrem.html

Go:   func main()
来源：http://hz.zdqjudy.top/gthndmprjn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.daria6918.cn/gtykzyvuxa.html

C#:   static void Main(string[] args)
来源：http://hz.jiagoushi.top/gthwkhaboe.html

[M08] 获取系统与运行时信息
来源：http://hz.shuidangran.top/gtyqkedssi.html

Py:   platform.system();  platform.python_version()
来源：http://hz.dianchejie.cn/gtlaomwaqu.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.9152youxi.cn/gtfquyyerd.html

JS:   process.platform;  process.version
来源：http://hz.9152youxi.cn/gtletwuxms.html

TS:   process.platform;  process.version
来源：http://hz.sysykeji.top/gtteeogjdj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zdqjudy.top/gtmsigziev.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhengqikj.top/gttshlucjo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ydjk.org.cn/gtakzonnnx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.gzhubu.top/gtbsuiynqv.html

================================================================================
来源：http://hz.chenzaomai.com/gtuwswfvma.html

N. 数据结构与算法
来源：http://hz.fengsongda.top/gthffxgjat.html

================================================================================
来源：http://hz.tanke756.top/gtkvagvhqc.html

[N01] 二分查找（有序数组）
来源：http://hz.tanke756.top/gtcgrywlql.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zycfv.cn/gtxxmngzcz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yangfankeji.com/gtrqemgfha.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhengqikj.top/gtyyzfccaf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.bjfxy.top/gtbybxltjy.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hfpthk.cn/gtxzeeecne.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.daxiang520.top/gtjysqdcvg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.dianchejie.cn/gtsckdqguz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jianghu66.top/gtlnnbfupj.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.pycfn.com/gtxpeefvpp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hnxiangtu.top/gtbcxxxbmz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhengqikj.top/gtwoatkgrb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtjvdojjtp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fengsongda.top/gtqdamqzgh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xinyue.icu/gtzdzujgwu.html

Go:   slices.Sort(arr)
来源：http://hz.shanyushiyangkeji.top/gtkzdhdaug.html

Ruby: arr.sort
来源：http://hz.sysykeji.top/gtigujkkyb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.tanke756.top/gtywhyjudt.html

[N03] 快速排序（分治示例）
来源：http://hz.snrcjt.cn/gtsuaedttj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cheryme.top/gtgjfpgsnu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cdnleiting.top/gttggsgane.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shanyushiyangtech.top/gtgwfbyvjd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ybcxt.top/gtkfjsixht.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinyuanbaomall.cn/gtyiacsxvu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhengqikj.top/gtzjkpanpu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zycfv.cn/gtqjiinbfc.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tianlin.xyz/gtrpoqvwju.html

[N04] 斐波那契数列
来源：http://hz.ydzc1.top/gtxbjljavm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.wangshuangyany.cn/gtsnvzpijw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yuanzhike.top/gtzxouszrm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xuetiantiany.cn/gtxgtumjuj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinyuanbaomall.cn/gtqzmozdnp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ywan-chungtsiang.top/gtvnpoqbwx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.pycfn.com/gtsmjftzzc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.c1oappe.top/gthsldinet.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj20258.top/gtoeyhpgth.html

[N05] 最大公约数
来源：http://hz.smart0.xyz/gtzwfczigd.html

Py:   math.gcd(a, b)
来源：http://hz.yanxiufei.cn/gtzllzvsur.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yuxming.cn/gtgqhvshiv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daria6918.cn/gtvmepgfes.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigfzy.top/gttvldnnhz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.tanke756.top/gtumlhvael.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.tianlin.xyz/gtoifsttzc.html

Ruby: a.gcd(b)
来源：http://hz.316326.xyz/gtxfnizvia.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.tanke756.top/gtpwaeycjm.html

[N06] 判断回文字符串
来源：http://hz.gogol.net.cn/gtppntjunv.html

Py:   s == s[::-1]
来源：http://hz.xuanzx.com/gtnzkgttdo.html

PHP:  $s === strrev($s);
来源：http://hz.yonumen.top/gtfuhbcrns.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cashguo.top/gtdpwuqdyq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtkjwpstue.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.c1oappe.top/gtpyrqqlxd.html

Go:   // 双指针从两端比较
来源：http://hz.yuxming.cn/gtpqqbjzro.html

Ruby: s == s.reverse
来源：http://hz.jinqigfzy.top/gtispmvpsg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tianlin.xyz/gtgdouiusd.html

[N07] 两数之和（返回下标）
来源：http://hz.shanyushiyangtech.top/gtgkujhwab.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.redwolf501.top/gtquhyanpc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhoulong.xyz/gtltmnmdnl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yongpay.top/gtvmnrcjov.html

TS:   // 手写 Map<string, number>
来源：http://hz.ehwqpu.com/gtvndrztry.html

Java: // 手写 HashMap
来源：http://hz.dianchejie.cn/gtrzwqaarg.html

Go:   // 手写 map[int]int
来源：http://hz.ydjk.org.cn/gttsuqofzz.html

Ruby: // 手写 Hash
来源：http://hz.meibo888.top/gtsblcwquk.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sxryk.cn/gthtjrheqm.html

[N08] 生成全排列
来源：http://hz.guannengcc.top/gtbcuckmsd.html

Py:   itertools.permutations(arr)
来源：http://hz.ppjwa.cn/gtuosnkfeu.html

PHP:  // 手写递归交换
来源：http://hz.ydzc1.top/gtmkenmurc.html

JS:   // 手写回溯递归
来源：http://hz.yuanzhike.top/gtrkfhghru.html

TS:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtvyjmwhls.html

Java: // 手写回溯递归
来源：http://hz.316326.xyz/gtouirljul.html

Go:   // 手写回溯递归
来源：http://hz.chenlongwang.top/gtxgjnbfys.html

Ruby: arr.permutation.to_a
来源：http://hz.pycfn.com/gtbjmwdrpi.html

C#:   // 手写回溯递归
来源：http://hz.cashguo.top/gttmxrucxr.html

[N09] 栈与队列
来源：http://hz.zycfv.cn/gtuzwwzbzu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.dianchejie.cn/gtaoejwmel.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.iojbl.cn/gtrxptjtcp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.meibo888.top/gttckhzdos.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xylfe.cn/gtrjootuuw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hnqzz.top/gteokcomqh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yvedp.cn/gtuxfbdact.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhijiandao.cn/gtwtuweijo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jlsjyb.cn/gtoshgnqns.html

[N10] 链表节点定义
来源：http://hz.ydjk.org.cn/gtbgqnziyc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cdnleiting.top/gtkjuqszbd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hfpthk.cn/gtrmutnwkk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.52xcode.cn/gtuvsrcbje.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.meibo888.top/gthpzmukgc.html

Java: class Node { int v; Node next; }
来源：http://hz.ybcxt.top/gtkjsafzma.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yvedp.cn/gttinhxbcw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhengqikj.top/gtjyuilgco.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhiwuduotai.top/gtgnbxefkp.html

[N11] 二叉树中序遍历
来源：http://hz.hywenlv.cn/gtpyztpvxa.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ydzc1.top/gtseehittl.html

PHP:  // 手写递归函数
来源：http://hz.ydzc1.top/gtfxjjxdnm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hongshengwenyu.top/gtmluswmqs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhixingplan.top/gtbhvpptoi.html

Java: // 手写递归
来源：http://hz.yangfankeji.com/gtuwdwpzfo.html

Go:   // 手写递归
来源：http://hz.zhengqikj.top/gteagxsusx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.sufxvd.cn/gtcrvcjxxu.html

C#:   // 手写递归
来源：http://hz.hywenlv.cn/gtcijmhcqz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinghuilouyu.cn/gtyxfovtvm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.52xcode.cn/gtxmweowiy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ydzc1.top/gtrdyhubai.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shangyingyoupin.top/gtamljvxdf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nwbrower.top/gtysewqwtv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.aizwys.cn/gtbwvtygli.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.gzhubu.top/gtjivslqtu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhoulong.xyz/gtfnrcgfbq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.bjfxy.top/gtdesrhadv.html

================================================================================
来源：http://hz.zhongyouzk.top/gtnebmgupd.html

O. 并发与异步
来源：http://hz.gzhubu.top/gtuknbjoiq.html

================================================================================
来源：http://hz.zhoulong.xyz/gtpvccnzmz.html

[O01] 启动一个线程
来源：http://hz.dashuyun.cn/gtkcqmvmbh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhengqikj.top/gtwbbowqip.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yvedp.cn/gtnvyywplx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fengsongda.top/gtingfpwtj.html

TS:   // 同 JS
来源：http://hz.redwolf501.top/gtestlxeqg.html

Java: new Thread(() -> f()).start()
来源：http://hz.yj20258.top/gtkjqeapyn.html

Go:   go f()
来源：http://hz.yangfankeji.com/gtwisojdyu.html

Ruby: Thread.new { f }
来源：http://hz.hnxiangtu.top/gtsrduflbk.html

C#:   Task.Run(() => F());
来源：http://hz.yonumen.top/gtqvowzzsx.html

[O02] 使用线程池
来源：http://hz.nanxinkj.top/gtfuvutdgb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinyuanbaomall.cn/gttvyuchso.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ppjwa.cn/gtyjhvrisz.html

JS:   // worker_threads 线程池
来源：http://hz.yj20258888.top/gtdxkmtkty.html

TS:   // worker_threads 线程池
来源：http://hz.zhongyouzk.top/gtibmicqim.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinqigfzy.top/gtfakctaba.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.feifeiyinyue.top/gthubkdwjt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cucudq.cn/gtmdmzejci.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.chenlongwang.top/gtmmmjkorc.html

[O03] 加锁保护共享数据
来源：http://hz.birdmap.top/gttbpyzowm.html

Py:   with lock: shared += 1
来源：http://hz.nwbrower.top/gtouabziya.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.aizwys.cn/gtllyhhjmh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gogol.net.cn/gtjyzpikir.html

TS:   // 同 JS
来源：http://hz.dianchejie.cn/gtxrylguha.html

Java: synchronized (this) { shared++; }
来源：http://hz.sxryk.cn/gtpkvmqtsk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yangfankeji.com/gtxkczhzuk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ybcxt.top/gtecpvrlag.html

C#:   lock (gate) { shared++; }
来源：http://hz.yonumen.top/gtguwhtazs.html

[O04] 定义异步函数并等待
来源：http://hz.hongshengwenyu.top/gtorrafqnp.html

Py:   async def f():⏎    await g()
来源：http://hz.yj20258888.top/gthnvinghb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.c1oappe.top/gtaofdgzxx.html

JS:   async function f() { await g(); }
来源：http://hz.hfpthk.cn/gtmuuymbxm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.bjfxy.top/gtgxzglmiu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hnxiangtu.top/gtyhcvaeql.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhijiandao.cn/gtnutwvwtd.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.birdmap.top/gtkdymuhuz.html

C#:   async Task F() { await G(); }
来源：http://hz.gaohongyu789.top/gtfccmzxvo.html

[O05] 并发执行并等待全部完成
来源：http://hz.gogol.net.cn/gtxanqfsqn.html

Py:   asyncio.gather(*tasks)
来源：http://hz.sufxvd.cn/gtqrampopb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.havefunace.top/gtsibiretc.html

JS:   await Promise.all(tasks)
来源：http://hz.hysaishi.cn/gtrexpvvlx.html

TS:   await Promise.all(tasks)
来源：http://hz.xziqi.cn/gthhdsxuvw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.chenlongwang.top/gtrtykyhwe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shanyushiyangkeji.top/gtoagrzdmu.html

Ruby: threads.map(&:join)
来源：http://hz.sxryk.cn/gtpursmiva.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.redwolf501.top/gtnquhoaqo.html


<!-- 参考信息 -->