代发 wailian999

Go:   encoding/gob
来源：http://hz.jinqigfzy.top/gtevrnvtow.html

Ruby: Marshal.dump(obj)
来源：http://hz.cucudq.cn/gtlrgcaalr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhongyouzk.top/gtnllcombr.html

================================================================================
来源：http://hz.shzxlz.cn/gtrjwfrlgd.html

L. 网络请求
来源：http://hz.wangshuangyany.cn/gtooyerqcr.html

================================================================================
来源：http://hz.xylfe.cn/gtzkbylkte.html

[L01] 发送 GET 请求
来源：http://hz.haohaochexian.top/gtxieseznj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.guannengcc.top/gtqkspqkpt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.redwolf501.top/gtretctgpj.html

JS:   await fetch(url)
来源：http://hz.jinqigufen.top/gtpsqflvwf.html

TS:   await fetch(url)
来源：http://hz.yj20258888.top/gtybqxbslf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jiagoushi.top/gthkvwzxwn.html

Go:   resp, err := http.Get(url)
来源：http://hz.vqdsnc.cn/gtsuilzqaf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yangfankeji.com/gtpqrkpvnd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.316326.xyz/gtcwfwvrlj.html

[L02] 发送 POST JSON
来源：http://hz.zhongyouzk.top/gtcmovvdlp.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xinyue.icu/gtizrgiroc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ivvv.top/gtwalzeoxs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.redwolf501.top/gtgvlhtyep.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhixingplan.top/gtjikbeksz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.guannengcc.top/gtdeonjitw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hnxiangtu.top/gtmmarmiwy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.guowangkeji.top/gtsogbafua.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.gogol.net.cn/gtwpgvjvsc.html

[L03] 设置自定义请求头
来源：http://hz.gotoacloud.top/gtcwdnvqfv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zycfv.cn/gtghgcgmmu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.c1oappe.top/gtgkndqxza.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aizwys.cn/gtadxubbdc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhixingplan.top/gthuorxxtu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hongshengwenyu.top/gtjeainqiy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhiwuduotai.top/gtbrpramet.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ydjk.org.cn/gtapsbrwmg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhixingplan.top/gtcyjvntnn.html

[L04] 设置超时
来源：http://hz.sufxvd.cn/gtrunrsftk.html

Py:   requests.get(url, timeout=5)
来源：http://hz.daxiang520.top/gtmaurvoek.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yonumen.top/gtwdimmdjh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.andypj.xyz/gtmmkcbklr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hongshengwenyu.top/gtmsueatnh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhiwuduotai.top/gtbciiairg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.birdmap.top/gtuvybfhdo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.9152youxi.cn/gtgwvbvcfl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.chenzaomai.com/gtuzkgkafc.html

[L05] 上传文件（multipart）
来源：http://hz.wangdashe.top/gtvpxxetov.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.guowangkeji.top/gtcxzmelyl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.daxiang520.top/gtlotgzqtw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xylfe.cn/gtddopztmu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinyuanbaomall.cn/gtkruvgwfv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sufxvd.cn/gtnljbcopu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yonumen.top/gtlbcmnhii.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yongpay.top/gttmrvsjfb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ivvv.top/gtpjyzinik.html

[L06] 解析响应为 JSON
来源：http://hz.fzhhl.top/gthdkmexup.html

Py:   resp.json()
来源：http://hz.yanxiufei.cn/gtvtajlfic.html

PHP:  json_decode($body, true);
来源：http://hz.yueranfly.top/gtwzmmjapp.html

JS:   await resp.json()
来源：http://hz.hnqzz.top/gtkqinwxmu.html

TS:   await resp.json()
来源：http://hz.cqqwz.cn/gtmlrioxpl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cqqwz.cn/gtyduzepox.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhoulong.xyz/gtnepdkwov.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jqgufenzy.top/gtkdyxgbro.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xylfe.cn/gtigguvrzx.html

[L07] 处理 HTTP 状态码
来源：http://hz.vqdsnc.cn/gtyxxmxweq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.fzhhl.top/gtofguxehs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.daria6918.cn/gtkwrjpbpn.html

JS:   resp.ok;  resp.status
来源：http://hz.fengsongda.top/gteseajdcs.html

TS:   resp.ok;  resp.status
来源：http://hz.aizwys.cn/gtbckhnzji.html

Java: resp.statusCode()
来源：http://hz.gogol.net.cn/gtnvhbmqxo.html

Go:   resp.StatusCode
来源：http://hz.yueranfly.top/gtjydwpevl.html

Ruby: resp.code.to_i
来源：http://hz.yuanzhike.top/gtoavaluqm.html

C#:   (int)resp.StatusCode
来源：http://hz.hnqzz.top/gtxuiylpot.html

[L08] 并发请求多个地址
来源：http://hz.wangdashe.top/gtodjzrymr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.guannengcc.top/gtygpffoeo.html

PHP:  curl_multi_init() 系列
来源：http://hz.guowangkeji.top/gtsxwsuhba.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ivvv.top/gtacjtcapk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fzhhl.top/gtawcqdcau.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.daria6918.cn/gtgbhosowp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.smart0.xyz/gtqdptosgw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ehwqpu.com/gtfotthgem.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.kuanghao11.cn/gtydusbzow.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtgjoczjmp.html

M. 命令行 / 进程 / 环境
来源：http://hz.shanyushiyangkeji.top/gtvwzvkdnk.html

================================================================================
来源：http://hz.gaohongyu789.top/gtmnpldlgl.html

[M01] 读取命令行参数
来源：http://hz.jinqigufen.top/gtfcpxphkd.html

Py:   sys.argv[1:]
来源：http://hz.daxiang520.top/gtnxecevat.html

PHP:  $argv;  $argc;
来源：http://hz.haohaochexian.top/gtnwknnnue.html

JS:   process.argv.slice(2)
来源：http://hz.zhixingplan.top/gtynoessdr.html

TS:   process.argv.slice(2)
来源：http://hz.sysykeji.top/gtssynzwlj.html

Java: args 数组（main 方法参数）
来源：http://hz.shanyushiyangkeji.top/gtkunbemyo.html

Go:   os.Args[1:]
来源：http://hz.jyoumei.cn/gtcqsvyurn.html

Ruby: ARGV
来源：http://hz.vqdsnc.cn/gtoamvrsyt.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shanyushiyangtech.top/gtwmqfkbxj.html

[M02] 读取环境变量
来源：http://hz.jinqigufen.top/gtsptrjhar.html

Py:   os.environ.get("HOME")
来源：http://hz.andypj.xyz/gtsarzqoii.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cqqwz.cn/gtoarvdlvs.html

JS:   process.env.HOME
来源：http://hz.xziqi.cn/gtqmsymulj.html

TS:   process.env.HOME
来源：http://hz.yanxiufei.cn/gtahhjbkhs.html

Java: System.getenv("HOME")
来源：http://hz.daxiang520.top/gtwrmfzmpe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.c1oappe.top/gteenfpplg.html

Ruby: ENV["HOME"]
来源：http://hz.zhoulong.xyz/gtvriqzoop.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.dashuyun.cn/gtirkttroi.html

[M03] 执行外部命令
来源：http://hz.tian-w.cn/gtjbxlvxsv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.smart0.xyz/gtlbtqtiii.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jqgfzy.top/gtopydyrum.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yongpay.top/gtupmldgyj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.nanxuanxn.top/gtxftjixyf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xuanzx.com/gtcbkvjcfe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jiagoushi.top/gtthptjpbk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.svipenyu.cn/gtniykjsdw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.meibo888.top/gtqqxkvhup.html

[M04] 获取当前工作目录
来源：http://hz.smart0.xyz/gtwkpwxmrj.html

Py:   os.getcwd()
来源：http://hz.iojbl.cn/gtdwciocne.html

PHP:  getcwd();
来源：http://hz.zhengqikj.top/gtllwlueiq.html

JS:   process.cwd()
来源：http://hz.cdnleiting.top/gtrtfmjyez.html

TS:   process.cwd()
来源：http://hz.zdqjudy.top/gtaigcqvtc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.chenjidiqi.icu/gtsbutvhli.html

Go:   os.Getwd()
来源：http://hz.shzxlz.cn/gtocpunzrp.html

Ruby: Dir.pwd
来源：http://hz.redwolf501.top/gtkkjsqcjd.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.andypj.xyz/gtooqgvkof.html

[M05] 设置退出码
来源：http://hz.jinghuilouyu.cn/gtzbixxroh.html

Py:   sys.exit(1)
来源：http://hz.0kj1m.cn/gtaypgjnpc.html

PHP:  exit(1);
来源：http://hz.hnqzz.top/gtabheidvw.html

JS:   process.exit(1)
来源：http://hz.pycfn.com/gthexdgnif.html

TS:   process.exit(1)
来源：http://hz.gaohongyu789.top/gthqnaaaxo.html

Java: System.exit(1)
来源：http://hz.xylfe.cn/gtakbfyzbk.html

Go:   os.Exit(1)
来源：http://hz.zhixingplan.top/gtxoyupbov.html

Ruby: exit 1
来源：http://hz.zhiwuduotai.top/gtdydczrtw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.daria6918.cn/gthkzltllh.html

[M06] 向标准错误输出
来源：http://hz.pengpengdd.cyou/gtwyxhqiji.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gogol.net.cn/gtocqjobgr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.bjfxy.top/gtofkwdzge.html

JS:   console.error("err")
来源：http://hz.cashguo.top/gtzhfuoipp.html

TS:   console.error("err")
来源：http://hz.cqqwz.cn/gthbqfnehr.html

Java: System.err.println("err")
来源：http://hz.svipenyu.cn/gtoyxxvfkl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ywan-chungtsiang.top/gtbphqikej.html

Ruby: warn "err"
来源：http://hz.fengsongda.top/gtdzrqmwvv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jinqigufen.top/gtwwmgzezp.html

[M07] 判断是否为主入口
来源：http://hz.havefunace.top/gtmbouqgch.html

Py:   if __name__ == "__main__":
来源：http://hz.zdqjudy.top/gtolzwyfik.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.iojbl.cn/gtfaeduwtc.html

JS:   require.main === module
来源：http://hz.redwolf501.top/gtndntkhhm.html

TS:   require.main === module
来源：http://hz.cheryme.top/gtjzwmrfxa.html

Java: public static void main(String[] args)
来源：http://hz.smart0.xyz/gtvrtdmobz.html

Go:   func main()
来源：http://hz.cqqwz.cn/gtyyopyizs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.chenlongwang.top/gtpuyiglpb.html

C#:   static void Main(string[] args)
来源：http://hz.vqdsnc.cn/gtwfbkzbbm.html

[M08] 获取系统与运行时信息
来源：http://hz.hysaishi.cn/gtszsqrlva.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hnqzz.top/gttsdbmorz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zdqjudy.top/gtkzbmtsox.html

JS:   process.platform;  process.version
来源：http://hz.aizwys.cn/gtokbkgohn.html

TS:   process.platform;  process.version
来源：http://hz.tianlin.xyz/gtpsvgfhyd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hongshengwenyu.top/gtdeblkfmt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhengqikj.top/gtahpkovpt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gaohongyu789.top/gtycfaxnah.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.316326.xyz/gtudhkslcd.html

================================================================================
来源：http://hz.xinyue.icu/gtgpxneeoz.html

N. 数据结构与算法
来源：http://hz.fzhhl.top/gtenvjobws.html

================================================================================
来源：http://hz.xuanzx.com/gtiomdbamw.html

[N01] 二分查找（有序数组）
来源：http://hz.wangdashe.top/gtphiqkebt.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ydjk.org.cn/gtvesajrwm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sweek.top/gtwuueqcfo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sweek.top/gthtmoawrs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxuanxn.top/gtoyqlztjl.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.havefunace.top/gtubdbegvr.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hfpthk.cn/gtpxzytvvv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.dashuyun.cn/gtvoszkpts.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nwbrower.top/gttmgusulo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.iojbl.cn/gtdaisxvyh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.aizwys.cn/gtsxhjnqja.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sweek.top/gtvomwlcgt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhiwuduotai.top/gtbchyerwn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.andypj.xyz/gtdychajoz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cqqwz.cn/gtjedkbxsc.html

Go:   slices.Sort(arr)
来源：http://hz.aizwys.cn/gtlnflpmpq.html

Ruby: arr.sort
来源：http://hz.xziqi.cn/gtxwlphtpc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shzxlz.cn/gthvhlmysc.html

[N03] 快速排序（分治示例）
来源：http://hz.xingfuxueyuan.xyz/gtcucuolvf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.tanke756.top/gtcyilepmu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.dashuyun.cn/gtfzvnjzrp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangdashe.top/gtcjudchic.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gtnirdjbzt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hfpthk.cn/gtgrsbiatl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jqgufenzy.top/gtvdtxflug.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.guowangkeji.top/gtjgdxqaee.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.smart0.xyz/gtgwtqvvii.html

[N04] 斐波那契数列
来源：http://hz.birdmap.top/gtmpbiemyw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.pycfn.com/gthqokemal.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinghuilouyu.cn/gtlpipncrz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xinyue.icu/gtmiavdlip.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sxryk.cn/gtmwwlmrzt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.fzhhl.top/gthqyyflav.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sxryk.cn/gtjiriroxf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yonumen.top/gttlrslbpt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhixingplan.top/gtpqutkjao.html

[N05] 最大公约数
来源：http://hz.jlsjyb.cn/gtsmytlbum.html

Py:   math.gcd(a, b)
来源：http://hz.ppjwa.cn/gtmrkniuhb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhijiandao.cn/gtifjsvtxn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgfzy.top/gtsyjnihaf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guannengcc.top/gtuwdorzvg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yueranfly.top/gtkwdnaoja.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.fengsongda.top/gtaalhdutw.html

Ruby: a.gcd(b)
来源：http://hz.jinqigfzy.top/gtshnrzgzx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jlsjyb.cn/gtqfvobyei.html

[N06] 判断回文字符串
来源：http://hz.mhx1999.top/gtplwjbdlb.html

Py:   s == s[::-1]
来源：http://hz.guowangkeji.top/gteuvirrhq.html

PHP:  $s === strrev($s);
来源：http://hz.snrcjt.cn/gtvmdaolrz.html

JS:   s === [...s].reverse().join("")
来源：http://hz.kuanghao11.cn/gtbxsvrjhx.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xylfe.cn/gtassvrvst.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.9152youxi.cn/gtipxunrdn.html

Go:   // 双指针从两端比较
来源：http://hz.xziqi.cn/gtnilhonln.html

Ruby: s == s.reverse
来源：http://hz.gzhubu.top/gtdtoyyndd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.nwbrower.top/gtozhhllrx.html

[N07] 两数之和（返回下标）
来源：http://hz.dianchejie.cn/gtisisdwbv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hnqzz.top/gtwznctpzn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sweek.top/gtgmfwdlgy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xinyue.icu/gtcjaqirlv.html

TS:   // 手写 Map<string, number>
来源：http://hz.hongshengwenyu.top/gtafcurkel.html

Java: // 手写 HashMap
来源：http://hz.hysaishi.cn/gtbjwlppin.html

Go:   // 手写 map[int]int
来源：http://hz.gzhubu.top/gtjemqjpqn.html

Ruby: // 手写 Hash
来源：http://hz.wangshuangyany.cn/gtobnrvncq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.chenzaomai.com/gtfjankrdu.html

[N08] 生成全排列
来源：http://hz.sxryk.cn/gtbsiklypj.html

Py:   itertools.permutations(arr)
来源：http://hz.9152youxi.cn/gtimkigoms.html

PHP:  // 手写递归交换
来源：http://hz.xuetiantiany.cn/gtqpyfuskp.html

JS:   // 手写回溯递归
来源：http://hz.wangdashe.top/gtpqnzpbjt.html

TS:   // 手写回溯递归
来源：http://hz.ppjwa.cn/gtwjvefrlt.html

Java: // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtxzydqnam.html

Go:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtzlspxupt.html

Ruby: arr.permutation.to_a
来源：http://hz.hnqzz.top/gtxkubyplx.html

C#:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtxbhtmpcp.html

[N09] 栈与队列
来源：http://hz.cqqwz.cn/gtoohhjmuz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.chenlongwang.top/gtykgwzfht.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.svipenyu.cn/gtuyavbjfg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xziqi.cn/gtxluuawvw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.316326.xyz/gtlkjpvmyo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zycfv.cn/gtoqknbpep.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hywenlv.cn/gtbbtmhmsu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.aibaodan.cn/gtunhpjjdl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hammf.cn/gtnkmfmigk.html

[N10] 链表节点定义
来源：http://hz.yonumen.top/gtnhgenjit.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.sysykeji.top/gtbzfutmgn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cashguo.top/gtmtdbiyox.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.feifeiyinyue.top/gtiizhrpap.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hnxiangtu.top/gtumuowdla.html

Java: class Node { int v; Node next; }
来源：http://hz.shzxlz.cn/gtbyapessg.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hywenlv.cn/gtojrvexed.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.guowangkeji.top/gthfirfxba.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shzxlz.cn/gtnuqemems.html

[N11] 二叉树中序遍历
来源：http://hz.shzxlz.cn/gtzbxdxmgg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinyuanbaomall.cn/gtbeytefcb.html

PHP:  // 手写递归函数
来源：http://hz.hongshengwenyu.top/gtteuixsgz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydzc1.top/gtmoakvvmd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cqqwz.cn/gtmxuzeuka.html

Java: // 手写递归
来源：http://hz.jyoumei.cn/gtawzxusym.html

Go:   // 手写递归
来源：http://hz.ivvv.top/gtrrcibywf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.wangdashe.top/gtheelseua.html

C#:   // 手写递归
来源：http://hz.yanxiufei.cn/gtzczcwcga.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jianghu66.top/gtpxbgtweo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jqgufenzy.top/gtwnhuccfy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hfpthk.cn/gtwuudzpwj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cashguo.top/gtgpdwxdoh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zdqjudy.top/gtmxwqkklv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zycfv.cn/gtpckxwfbx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.316326.xyz/gtnwtcxfay.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yvedp.cn/gtiucgmryf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhixingplan.top/gtpcxwvgum.html

================================================================================
来源：http://hz.cdnleiting.top/gtomiyynam.html

O. 并发与异步
来源：http://hz.iojbl.cn/gtqpfkqipa.html

================================================================================
来源：http://hz.yuanzhike.top/gtyhshgphr.html

[O01] 启动一个线程
来源：http://hz.vqdsnc.cn/gtbyysmoor.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xuanzx.com/gtgurjmetf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.daria6918.cn/gtapryzlag.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cdnleiting.top/gtzgvljdgx.html

TS:   // 同 JS
来源：http://hz.cheryme.top/gtiemptsrs.html

Java: new Thread(() -> f()).start()
来源：http://hz.yangfankeji.com/gtaxaebgyd.html

Go:   go f()
来源：http://hz.316326.xyz/gthclrthpb.html

Ruby: Thread.new { f }
来源：http://hz.xuetiantiany.cn/gtafdmtfmz.html

C#:   Task.Run(() => F());
来源：http://hz.jinqigufen.top/gtmdsjpuuy.html

[O02] 使用线程池
来源：http://hz.tianlin.xyz/gtkktebsfc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.chenzaomai.com/gtandkcfga.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sufxvd.cn/gtdvkgydkz.html

JS:   // worker_threads 线程池
来源：http://hz.kuanghao11.cn/gtvkfcganu.html

TS:   // worker_threads 线程池
来源：http://hz.sufxvd.cn/gtufjffsob.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jlsjyb.cn/gtaxvclhcf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.nwbrower.top/gtkbliajhz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.chenlongwang.top/gtiduzekjn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.wangshuangyany.cn/gtzvfkvtpt.html

[O03] 加锁保护共享数据
来源：http://hz.xinyue.icu/gtpzdmqmew.html

Py:   with lock: shared += 1
来源：http://hz.ybcxt.top/gtzzkyffvc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.snrcjt.cn/gtcvftlwgz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.tianlin.xyz/gtfgtkzxtk.html

TS:   // 同 JS
来源：http://hz.ydjk.org.cn/gtsgwvsoei.html

Java: synchronized (this) { shared++; }
来源：http://hz.ywan-chungtsiang.top/gtqxgwkgmx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ydzc1.top/gtsgwlzwpi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.quarkkingdee.top/gttlswlbbi.html

C#:   lock (gate) { shared++; }
来源：http://hz.xuanzx.com/gtskivxovh.html

[O04] 定义异步函数并等待
来源：http://hz.zhaomingkeji.xyz/gtarmleuzz.html

Py:   async def f():⏎    await g()
来源：http://hz.jiagoushi.top/gtjazbgbdm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.guowangkeji.top/gtgipkhnqb.html

JS:   async function f() { await g(); }
来源：http://hz.yuanzhike.top/gtikeehuru.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hysaishi.cn/gtsfvksfpd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shzxlz.cn/gtgeseilfz.html


<!-- 参考信息 -->