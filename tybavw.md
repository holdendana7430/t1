代发 wailian999

Go:   encoding/gob
来源：http://hz.hnxiangtu.top/gtfknwpfhq.html

Ruby: Marshal.dump(obj)
来源：http://hz.redwolf501.top/gteqrywkue.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhixingplan.top/gtfisibaqc.html

================================================================================
来源：http://hz.jlsjyb.cn/gteewpgknj.html

L. 网络请求
来源：http://hz.dashuyun.cn/gtrwgibbbk.html

================================================================================
来源：http://hz.gaohongyu789.top/gtfhtditnl.html

[L01] 发送 GET 请求
来源：http://hz.sxryk.cn/gtyjlwyhot.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.smart0.xyz/gtfbwvasga.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hammf.cn/gtucqarqen.html

JS:   await fetch(url)
来源：http://hz.jinqigufen.top/gthoqmvyys.html

TS:   await fetch(url)
来源：http://hz.nanxuanxn.top/gtmwxrhezt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hammf.cn/gtvlvzpnkf.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhoulong.xyz/gtqpuimwrq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sxryk.cn/gtzjxnojsm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xziqi.cn/gtttdnwyby.html

[L02] 发送 POST JSON
来源：http://hz.c1oappe.top/gtoenmfiyd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.tian-w.cn/gtdjucuged.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cheryme.top/gtdrtzsqwr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dianchejie.cn/gtgrkflney.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xingfuxueyuan.xyz/gtcpyznscw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jyoumei.cn/gtnsxnxhfv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zycfv.cn/gtlktsviqh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.iojbl.cn/gtvgefypfr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shangyingyoupin.top/gtejxgsnbs.html

[L03] 设置自定义请求头
来源：http://hz.gotoacloud.top/gtezfhnlag.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.haohaochexian.top/gtqaabegdj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.nanxuanxn.top/gthyujkbgx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cucudq.cn/gtnrnwmdnu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.52xcode.cn/gtcqmsgmui.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xylfe.cn/gtvwqzwasd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sweek.top/gtnmuvsojg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jyoumei.cn/gtrmkuukvy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.haohaochexian.top/gtztvzqgwc.html

[L04] 设置超时
来源：http://hz.shanyushiyangtech.top/gtzcyftjgo.html

Py:   requests.get(url, timeout=5)
来源：http://hz.aibaodan.cn/gtxnkrlsro.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yj20258888.top/gtgxrggkof.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yueranfly.top/gtdlqmwnby.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sufxvd.cn/gthgapbqvf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.0kj1m.cn/gtmmuctpcf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.tanke756.top/gtdszpnrqz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gogol.net.cn/gtoylkivsi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yj20258.top/gtmzvkhoyi.html

[L05] 上传文件（multipart）
来源：http://hz.yangfankeji.com/gtkaykkmfi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zycfv.cn/gtneonakoi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.pycfn.com/gtzcbjrqqw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhixingplan.top/gtzkquwpyk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.vqdsnc.cn/gtihwaxwzb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.kuanghao11.cn/gtlmjdhzhw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jiagoushi.top/gtbhuwxbaq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhixingplan.top/gtpelrxbwr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhixingplan.top/gtxfcvzpxv.html

[L06] 解析响应为 JSON
来源：http://hz.dashuyun.cn/gttqsucebt.html

Py:   resp.json()
来源：http://hz.vqdsnc.cn/gtntjrvrec.html

PHP:  json_decode($body, true);
来源：http://hz.jqgufenzy.top/gtixqzhxfg.html

JS:   await resp.json()
来源：http://hz.jinyuanbaomall.cn/gtzkyjqfnk.html

TS:   await resp.json()
来源：http://hz.dashuyun.cn/gtaallzeok.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.mhx1999.top/gtomfwrzeo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.birdmap.top/gtwtjlsuqa.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jlsjyb.cn/gtlcnvncsr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ydzc1.top/gtnymphnci.html

[L07] 处理 HTTP 状态码
来源：http://hz.andypj.xyz/gtzxkaautt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.vqdsnc.cn/gtdphalfpk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xylfe.cn/gtyapswfhn.html

JS:   resp.ok;  resp.status
来源：http://hz.havefunace.top/gtdcfuysea.html

TS:   resp.ok;  resp.status
来源：http://hz.daria6918.cn/gtpggcamij.html

Java: resp.statusCode()
来源：http://hz.gogol.net.cn/gtcvrtrcni.html

Go:   resp.StatusCode
来源：http://hz.daxiang520.top/gtsmilqzly.html

Ruby: resp.code.to_i
来源：http://hz.zdqjudy.top/gtydarcajq.html

C#:   (int)resp.StatusCode
来源：http://hz.cqqwz.cn/gtbaglqlvt.html

[L08] 并发请求多个地址
来源：http://hz.jianghu66.top/gtkukttnmo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cdnleiting.top/gtzklfbsnp.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhaomingkeji.xyz/gtrsygmgbm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtzdtvglbt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.feifeiyinyue.top/gtwhgqwrdi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shangyingyoupin.top/gtxvsvkxwr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yonumen.top/gtgrrikidc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.snrcjt.cn/gtcwylwrws.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hywenlv.cn/gtaokqbysb.html

================================================================================
来源：http://hz.haohaochexian.top/gtomlbgrqa.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhengqikj.top/gtqnrwhmiq.html

================================================================================
来源：http://hz.yvedp.cn/gtjlzywisr.html

[M01] 读取命令行参数
来源：http://hz.zdqjudy.top/gtgawdhtok.html

Py:   sys.argv[1:]
来源：http://hz.zhixingplan.top/gtqkjyhhwv.html

PHP:  $argv;  $argc;
来源：http://hz.chenjidiqi.icu/gtyjrkmzmm.html

JS:   process.argv.slice(2)
来源：http://hz.zycfv.cn/gthaphdxmd.html

TS:   process.argv.slice(2)
来源：http://hz.gaohongyu789.top/gtrrcchxre.html

Java: args 数组（main 方法参数）
来源：http://hz.guannengcc.top/gtniwhywgq.html

Go:   os.Args[1:]
来源：http://hz.cheryme.top/gtfsougpqs.html

Ruby: ARGV
来源：http://hz.aizwys.cn/gtywedcuze.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shangyingyoupin.top/gttztgtzci.html

[M02] 读取环境变量
来源：http://hz.bjfxy.top/gtayiatnea.html

Py:   os.environ.get("HOME")
来源：http://hz.jinyuanbaomall.cn/gtuxefwyiq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.fzhhl.top/gttgrxrwxm.html

JS:   process.env.HOME
来源：http://hz.mhx1999.top/gtawuopdwy.html

TS:   process.env.HOME
来源：http://hz.hfpthk.cn/gtswocxbsq.html

Java: System.getenv("HOME")
来源：http://hz.xylfe.cn/gthplvutji.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yueranfly.top/gtjwmawujr.html

Ruby: ENV["HOME"]
来源：http://hz.jinyuanbaomall.cn/gtlpbrvfvn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ybcxt.top/gtzekjyplp.html

[M03] 执行外部命令
来源：http://hz.havefunace.top/gtpoiayivl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hysaishi.cn/gtggyascsf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.svipenyu.cn/gtlfvpijjv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hysaishi.cn/gtpdzuwobe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xziqi.cn/gtqorjpwfg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hongshengwenyu.top/gtdkttouyh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jinqigfzy.top/gtvbjwmtix.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinqigufen.top/gtdnxaawcw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhaomingkeji.xyz/gtglrmdsst.html

[M04] 获取当前工作目录
来源：http://hz.gotoacloud.top/gtdkgsgrnh.html

Py:   os.getcwd()
来源：http://hz.guannengcc.top/gtggtvkopr.html

PHP:  getcwd();
来源：http://hz.fengsongda.top/gtxegwobaw.html

JS:   process.cwd()
来源：http://hz.snrcjt.cn/gtjhgxrqru.html

TS:   process.cwd()
来源：http://hz.jqgfzy.top/gtrkfbmhqf.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhoulong.xyz/gtthujdfor.html

Go:   os.Getwd()
来源：http://hz.xziqi.cn/gtgqnkbkfm.html

Ruby: Dir.pwd
来源：http://hz.shzxlz.cn/gtwhludzlz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.tanke756.top/gtuiuofmvb.html

[M05] 设置退出码
来源：http://hz.chenlongwang.top/gtgjcftvxj.html

Py:   sys.exit(1)
来源：http://hz.yj202588.top/gtpaztbtpq.html

PHP:  exit(1);
来源：http://hz.tianlin.xyz/gtzikidbgn.html

JS:   process.exit(1)
来源：http://hz.yuanzhike.top/gtnicqsxnf.html

TS:   process.exit(1)
来源：http://hz.yonumen.top/gtwzafhqtl.html

Java: System.exit(1)
来源：http://hz.sufxvd.cn/gtltpiwlsb.html

Go:   os.Exit(1)
来源：http://hz.hongshengwenyu.top/gthcmggjlj.html

Ruby: exit 1
来源：http://hz.mhx1999.top/gtbcqofido.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj20258.top/gtufdzpkhb.html

[M06] 向标准错误输出
来源：http://hz.dashuyun.cn/gtmlocygvm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hammf.cn/gtueezxjru.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.havefunace.top/gtyvigrmgh.html

JS:   console.error("err")
来源：http://hz.dianchejie.cn/gtozxtjycp.html

TS:   console.error("err")
来源：http://hz.jlsjyb.cn/gtprdwlsey.html

Java: System.err.println("err")
来源：http://hz.zhixingplan.top/gtrpqltiqw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jianghu66.top/gthhwivqlb.html

Ruby: warn "err"
来源：http://hz.sxryk.cn/gtfiwwcznl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yonumen.top/gtayykuzag.html

[M07] 判断是否为主入口
来源：http://hz.fengsongda.top/gtwocdzaxr.html

Py:   if __name__ == "__main__":
来源：http://hz.hfpthk.cn/gtzdpvlzrh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yonumen.top/gtuauopiwv.html

JS:   require.main === module
来源：http://hz.nwbrower.top/gtltltuyln.html

TS:   require.main === module
来源：http://hz.sxryk.cn/gttzfcbssk.html

Java: public static void main(String[] args)
来源：http://hz.gogol.net.cn/gtkaxmoxgc.html

Go:   func main()
来源：http://hz.ehwqpu.com/gtbqbhbtmg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ywan-chungtsiang.top/gtkpnjyoak.html

C#:   static void Main(string[] args)
来源：http://hz.svipenyu.cn/gtuqofelmi.html

[M08] 获取系统与运行时信息
来源：http://hz.snrcjt.cn/gtgqnfmcxc.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cucudq.cn/gtncujmlaz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gaohongyu789.top/gtylmznfdn.html

JS:   process.platform;  process.version
来源：http://hz.sysykeji.top/gtvtfztpjp.html

TS:   process.platform;  process.version
来源：http://hz.yongpay.top/gtzahidlho.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinqigufen.top/gtebplnmfi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.316326.xyz/gtdlrrerqj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cheryme.top/gtcwlqcams.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cdnleiting.top/gtoavhnssj.html

================================================================================
来源：http://hz.0kj1m.cn/gteqscuoyk.html

N. 数据结构与算法
来源：http://hz.jqgfzy.top/gtcowniiyt.html

================================================================================
来源：http://hz.chenlongwang.top/gtrcjttxxc.html

[N01] 二分查找（有序数组）
来源：http://hz.ydzc1.top/gthdauqoxy.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtvmjsidib.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jlsjyb.cn/gtbpglcjem.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xylfe.cn/gthgwvrgut.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jianghu66.top/gtqsbfhtrt.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.andypj.xyz/gtsrewaldn.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yanxiufei.cn/gtdticgfgc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hammf.cn/gtqfooveau.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.aibaodan.cn/gtzysmolyf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hongshengwenyu.top/gtpdlmcykk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.mhx1999.top/gtysmhqhjn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cqqwz.cn/gtbgpamywb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fengsongda.top/gtriwosrql.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hnxiangtu.top/gtdzzguwwb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.tanke756.top/gtebbdqgtk.html

Go:   slices.Sort(arr)
来源：http://hz.xuanzx.com/gtkbzhsbjy.html

Ruby: arr.sort
来源：http://hz.iojbl.cn/gtfykahxly.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cqqwz.cn/gtgfqmskvw.html

[N03] 快速排序（分治示例）
来源：http://hz.ivvv.top/gthckgjvth.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinyuanbaomall.cn/gtiawmookw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xuetiantiany.cn/gtfcmgcvfr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cucudq.cn/gtxqcetufl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shanyushiyangtech.top/gtyiujsihc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhaomingkeji.xyz/gtlwyadccx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nanxuanxn.top/gtipqalaih.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yonumen.top/gtzxxocrvs.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yuxming.cn/gtxuhqswda.html

[N04] 斐波那契数列
来源：http://hz.zhixingplan.top/gtilclyxzu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.nwbrower.top/gtwevocjoo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.guowangkeji.top/gtybnzxrsj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cheryme.top/gtzxmmlfve.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sufxvd.cn/gtmletjdwr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.c1oappe.top/gtgtccynip.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xylfe.cn/gtnwhbdhdm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj202588.top/gtngahiuxy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj20258.top/gtizengleh.html

[N05] 最大公约数
来源：http://hz.jiagoushi.top/gtvdrwejug.html

Py:   math.gcd(a, b)
来源：http://hz.wangshuangyany.cn/gtimpbkwpb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.birdmap.top/gtbvqubxab.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.meibo888.top/gtzzdkiind.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.meibo888.top/gthnfadzwy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gzhubu.top/gtbxggrzzn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhiwuduotai.top/gtbgeswcri.html

Ruby: a.gcd(b)
来源：http://hz.hongshengwenyu.top/gtvoslycbk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.snrcjt.cn/gtpbxpqqfx.html

[N06] 判断回文字符串
来源：http://hz.aibaodan.cn/gtedfpqjrr.html

Py:   s == s[::-1]
来源：http://hz.zhengqikj.top/gtwunejtte.html

PHP:  $s === strrev($s);
来源：http://hz.gzhubu.top/gtwhdryesz.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yvedp.cn/gtqzynjcpl.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hnqzz.top/gtbtjrxdko.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.chenlongwang.top/gthjbjnqan.html

Go:   // 双指针从两端比较
来源：http://hz.0kj1m.cn/gttafslnwl.html

Ruby: s == s.reverse
来源：http://hz.ehwqpu.com/gtouzixjji.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yanxiufei.cn/gtduexuyaq.html

[N07] 两数之和（返回下标）
来源：http://hz.gzhubu.top/gtxyjrmktg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinqigufen.top/gtrjkgeats.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hnqzz.top/gtbjuwtapk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xziqi.cn/gtkkpqwrwj.html

TS:   // 手写 Map<string, number>
来源：http://hz.redwolf501.top/gtqccharmz.html

Java: // 手写 HashMap
来源：http://hz.yonumen.top/gtmqszaigb.html

Go:   // 手写 map[int]int
来源：http://hz.zhongyouzk.top/gtnyezthmm.html

Ruby: // 手写 Hash
来源：http://hz.shuidangran.top/gtvfdmkuwk.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hfpthk.cn/gtsqddvcya.html

[N08] 生成全排列
来源：http://hz.jinqigfzy.top/gtwqvsebpi.html

Py:   itertools.permutations(arr)
来源：http://hz.shanyushiyangkeji.top/gtmwgpxglw.html

PHP:  // 手写递归交换
来源：http://hz.jinqigfzy.top/gtftvvpmlo.html

JS:   // 手写回溯递归
来源：http://hz.ydzc1.top/gtquofyotq.html

TS:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtehrzhfjn.html

Java: // 手写回溯递归
来源：http://hz.dashuyun.cn/gtkpaxtrrp.html

Go:   // 手写回溯递归
来源：http://hz.ybcxt.top/gtvtcyhzyx.html

Ruby: arr.permutation.to_a
来源：http://hz.bjfxy.top/gtoltekguo.html

C#:   // 手写回溯递归
来源：http://hz.meibo888.top/gtruvzkdmd.html

[N09] 栈与队列
来源：http://hz.9152youxi.cn/gttlbismyn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.gogol.net.cn/gtcnndzave.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.tanke756.top/gtlgkebfkx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xziqi.cn/gtsrdgwovu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xuetiantiany.cn/gtcjtpvztm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gotoacloud.top/gtgphtkyhs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sxryk.cn/gtglwifrxo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hnqzz.top/gtgxhrpcux.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhongyouzk.top/gtvjqaipex.html

[N10] 链表节点定义
来源：http://hz.52xcode.cn/gtrcxkdkls.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ybcxt.top/gtigrcmesz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hnqzz.top/gtczehaulr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yuxming.cn/gtoezyfywx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.52xcode.cn/gtmrbyjhzl.html

Java: class Node { int v; Node next; }
来源：http://hz.haohaochexian.top/gtjbcifrmn.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yanxiufei.cn/gtubihcnvc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.redwolf501.top/gtsphvstuc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zdqjudy.top/gtigmnloel.html

[N11] 二叉树中序遍历
来源：http://hz.jqgufenzy.top/gtkcetfkqg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cheryme.top/gthvcjygny.html

PHP:  // 手写递归函数
来源：http://hz.0kj1m.cn/gtefejebki.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuanzhike.top/gtvjuzgqll.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.0kj1m.cn/gtuphcheho.html

Java: // 手写递归
来源：http://hz.zhixingplan.top/gtetmpbvvb.html

Go:   // 手写递归
来源：http://hz.bjfxy.top/gtawsjhhhi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xziqi.cn/gtebseepeu.html

C#:   // 手写递归
来源：http://hz.xziqi.cn/gtutsgvrjv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yanxiufei.cn/gtwnddwbzs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ivvv.top/gtpbafkdus.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.chenlongwang.top/gtexgwbgot.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhixingplan.top/gtpbzqkblk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangshuangyany.cn/gtwbmsereq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shuidangran.top/gtynvffvkx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yonumen.top/gtvfttlaje.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xuetiantiany.cn/gtkwcncgck.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ivvv.top/gtoxlrjjnl.html

================================================================================
来源：http://hz.yuxming.cn/gtpcpgbhgj.html

O. 并发与异步
来源：http://hz.shzxlz.cn/gtkfcejsln.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtbhhdgngv.html

[O01] 启动一个线程
来源：http://hz.gotoacloud.top/gtvmyxdrur.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.nwbrower.top/gtjobtyebi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.birdmap.top/gtbipajkwe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fzhhl.top/gtxsbkosaq.html

TS:   // 同 JS
来源：http://hz.ehwqpu.com/gtaklrcjcx.html

Java: new Thread(() -> f()).start()
来源：http://hz.yanxiufei.cn/gtbchpmjcs.html

Go:   go f()
来源：http://hz.ppjwa.cn/gtgucrretc.html

Ruby: Thread.new { f }
来源：http://hz.snrcjt.cn/gttatzgecn.html

C#:   Task.Run(() => F());
来源：http://hz.chenjidiqi.icu/gtovrejjac.html

[O02] 使用线程池
来源：http://hz.yvedp.cn/gtvtqcqxty.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hongshengwenyu.top/gtxqcifbng.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.guowangkeji.top/gthrbljkng.html

JS:   // worker_threads 线程池
来源：http://hz.chenjidiqi.icu/gtezethepg.html

TS:   // worker_threads 线程池
来源：http://hz.redwolf501.top/gtzgixuqof.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shangyingyoupin.top/gtsgkczpyc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.fzhhl.top/gtlcmddlym.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shanyushiyangkeji.top/gtrhqvvddy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.nanxuanxn.top/gteelwwtec.html

[O03] 加锁保护共享数据
来源：http://hz.xinyue.icu/gtlruznzdv.html

Py:   with lock: shared += 1
来源：http://hz.hywenlv.cn/gtdketnula.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.andypj.xyz/gtvwyyznap.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xylfe.cn/gtpsezhyun.html

TS:   // 同 JS
来源：http://hz.hysaishi.cn/gthvimuvqr.html

Java: synchronized (this) { shared++; }
来源：http://hz.smart0.xyz/gtrkmlowug.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zdqjudy.top/gththtdrww.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ppjwa.cn/gtfgjmoufj.html

C#:   lock (gate) { shared++; }
来源：http://hz.zdqjudy.top/gtwgndhnqv.html

[O04] 定义异步函数并等待
来源：http://hz.fzhhl.top/gtecjzsijc.html

Py:   async def f():⏎    await g()
来源：http://hz.zhaomingkeji.xyz/gtidjiyqra.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.chenlongwang.top/gtfjchfekr.html

JS:   async function f() { await g(); }
来源：http://hz.gzhubu.top/gtaocwqold.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yj20258888.top/gtcogsomyc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jqgufenzy.top/gterhxljsg.html


<!-- 参考信息 -->