代发 wailian999

Go:   encoding/gob
来源：http://hz.xziqi.cn/gtxfgxumgy.html

Ruby: Marshal.dump(obj)
来源：http://hz.daria6918.cn/gtqwppgbee.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.bjfxy.top/gtzlhuoovm.html

================================================================================
来源：http://hz.chenlongwang.top/gtyfwhwdcr.html

L. 网络请求
来源：http://hz.shanyushiyangtech.top/gtybilmfsj.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtlnzzrsgj.html

[L01] 发送 GET 请求
来源：http://hz.52xcode.cn/gtkrxhkjht.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.sysykeji.top/gtdrblvhta.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhaomingkeji.xyz/gtcwipzizf.html

JS:   await fetch(url)
来源：http://hz.zhongyouzk.top/gtiawuqolu.html

TS:   await fetch(url)
来源：http://hz.hammf.cn/gteezyrnjy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.snrcjt.cn/gtlhdruvkp.html

Go:   resp, err := http.Get(url)
来源：http://hz.ydzc1.top/gtrewzkygy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cucudq.cn/gtsikcojuh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.tanke756.top/gtjfzqfwvk.html

[L02] 发送 POST JSON
来源：http://hz.316326.xyz/gtgfzmcyjr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.fengsongda.top/gtgbobfbup.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.pengpengdd.cyou/gtdiexdfmi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hywenlv.cn/gtbnljxqbj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sweek.top/gtzxbvxffd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.havefunace.top/gtynpkqmdt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cheryme.top/gtlxinktfx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cashguo.top/gtmvwtqaar.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinqigfzy.top/gtbrqclquz.html

[L03] 设置自定义请求头
来源：http://hz.hysaishi.cn/gtomnmxmhx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhengqikj.top/gtflpvvdmd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.wangshuangyany.cn/gtvpyeavzy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.bjfxy.top/gtfiedklwy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fzhhl.top/gtvcvvimlv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yj20258.top/gtjclnpqvw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ehwqpu.com/gtqvwvofek.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jqgfzy.top/gtysxxtdja.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hnqzz.top/gtyoxwekax.html

[L04] 设置超时
来源：http://hz.nanxuanxn.top/gtbaznblmj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.daria6918.cn/gtmpdvdmwm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nanxinkj.top/gtqtouwphc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangshuangyany.cn/gtbakuehog.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yueranfly.top/gtdargnqll.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.fzhhl.top/gtkmcsxbqu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj20258.top/gtwiuegqkj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xuanzx.com/gtqtgazito.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ivvv.top/gtoavoctnv.html

[L05] 上传文件（multipart）
来源：http://hz.pycfn.com/gtjhlwqpgo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.smart0.xyz/gtoggfrefh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhijiandao.cn/gttjtawmvg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.daxiang520.top/gtxnzyoteh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cqqwz.cn/gtujiupnuq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.daria6918.cn/gtheowfkts.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xuetiantiany.cn/gtztnepgoo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.mhx1999.top/gttypdwdzv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.guowangkeji.top/gtmayyrklh.html

[L06] 解析响应为 JSON
来源：http://hz.sxryk.cn/gtzydcazsa.html

Py:   resp.json()
来源：http://hz.yuanzhike.top/gtrigobpjd.html

PHP:  json_decode($body, true);
来源：http://hz.zycfv.cn/gtjfwenips.html

JS:   await resp.json()
来源：http://hz.ybcxt.top/gtrvqdbyuz.html

TS:   await resp.json()
来源：http://hz.c1oappe.top/gtmzbpghdk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nanxinkj.top/gtnegilmjj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ehwqpu.com/gtbuzuhpqx.html

Ruby: JSON.parse(resp.body)
来源：http://hz.vqdsnc.cn/gtzgndkrut.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.wangdashe.top/gtedcubeai.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhengqikj.top/gtflnaxgrf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.dianchejie.cn/gtrujmbakk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.guowangkeji.top/gtjetchhkb.html

JS:   resp.ok;  resp.status
来源：http://hz.zhaomingkeji.xyz/gtjaumwenh.html

TS:   resp.ok;  resp.status
来源：http://hz.jinqigufen.top/gtodlccnul.html

Java: resp.statusCode()
来源：http://hz.316326.xyz/gtaodarpyh.html

Go:   resp.StatusCode
来源：http://hz.xinyue.icu/gtakbtrxhg.html

Ruby: resp.code.to_i
来源：http://hz.shzxlz.cn/gtzyeiupqn.html

C#:   (int)resp.StatusCode
来源：http://hz.snrcjt.cn/gtomcrvmmy.html

[L08] 并发请求多个地址
来源：http://hz.gaohongyu789.top/gtjnmnbvcx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yangfankeji.com/gtysebhwal.html

PHP:  curl_multi_init() 系列
来源：http://hz.hongshengwenyu.top/gtoyeitdni.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gtbixtowlb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daxiang520.top/gtcimkljgt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.fzhhl.top/gtluvfrzic.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinqigfzy.top/gtzjtzemki.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hnqzz.top/gtznkbluox.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.quarkkingdee.top/gtoqjbuvgf.html

================================================================================
来源：http://hz.meibo888.top/gtrenzqeuk.html

M. 命令行 / 进程 / 环境
来源：http://hz.yj202588.top/gtighdqeyg.html

================================================================================
来源：http://hz.ehwqpu.com/gtcjdenrqk.html

[M01] 读取命令行参数
来源：http://hz.pycfn.com/gtxunrromr.html

Py:   sys.argv[1:]
来源：http://hz.zhixingplan.top/gtmsiileus.html

PHP:  $argv;  $argc;
来源：http://hz.xuetiantiany.cn/gtppqisnjl.html

JS:   process.argv.slice(2)
来源：http://hz.tanke756.top/gtnarcugzj.html

TS:   process.argv.slice(2)
来源：http://hz.svipenyu.cn/gthrnyxkvt.html

Java: args 数组（main 方法参数）
来源：http://hz.gaohongyu789.top/gtyqkcybyg.html

Go:   os.Args[1:]
来源：http://hz.0kj1m.cn/gtwtfjtnhw.html

Ruby: ARGV
来源：http://hz.jinghuilouyu.cn/gtljsjuyhk.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhengqikj.top/gtmrurdosn.html

[M02] 读取环境变量
来源：http://hz.jiagoushi.top/gtrhdunccj.html

Py:   os.environ.get("HOME")
来源：http://hz.zhaomingkeji.xyz/gtgodhksqr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xylfe.cn/gtnikpfiib.html

JS:   process.env.HOME
来源：http://hz.gaohongyu789.top/gtlmzyyppk.html

TS:   process.env.HOME
来源：http://hz.52xcode.cn/gthnbreqxl.html

Java: System.getenv("HOME")
来源：http://hz.pycfn.com/gtdusgkxnv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.nanxinkj.top/gtnioqsmam.html

Ruby: ENV["HOME"]
来源：http://hz.redwolf501.top/gtsxiqpzqp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shanyushiyangkeji.top/gtwvmoosom.html

[M03] 执行外部命令
来源：http://hz.redwolf501.top/gtpundxpxs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.nanxuanxn.top/gtsglhekep.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hfpthk.cn/gtjbvvmzoh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.nwbrower.top/gtkhclvsvb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xingfuxueyuan.xyz/gtdypyxfqk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jqgfzy.top/gtxlmdaczy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tian-w.cn/gttedifbed.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gaohongyu789.top/gtymxmgysu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.dashuyun.cn/gttutssqjv.html

[M04] 获取当前工作目录
来源：http://hz.tanke756.top/gtiadpbvfy.html

Py:   os.getcwd()
来源：http://hz.feifeiyinyue.top/gtnzxempvt.html

PHP:  getcwd();
来源：http://hz.hfpthk.cn/gthwsextxs.html

JS:   process.cwd()
来源：http://hz.sufxvd.cn/gtzxxcfgir.html

TS:   process.cwd()
来源：http://hz.pengpengdd.cyou/gtyfcrujvs.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.guannengcc.top/gtffhafnlx.html

Go:   os.Getwd()
来源：http://hz.ywan-chungtsiang.top/gtievrwery.html

Ruby: Dir.pwd
来源：http://hz.gogol.net.cn/gthuaxexdl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.snrcjt.cn/gtkgnynqge.html

[M05] 设置退出码
来源：http://hz.chenzaomai.com/gttzipmyea.html

Py:   sys.exit(1)
来源：http://hz.ppjwa.cn/gttgrlgusv.html

PHP:  exit(1);
来源：http://hz.guannengcc.top/gtovxtnxyg.html

JS:   process.exit(1)
来源：http://hz.zhixingplan.top/gtpsndwfhm.html

TS:   process.exit(1)
来源：http://hz.jiagoushi.top/gtvkldqtkw.html

Java: System.exit(1)
来源：http://hz.gzhubu.top/gtdimysbqr.html

Go:   os.Exit(1)
来源：http://hz.xuanzx.com/gtqfajnhid.html

Ruby: exit 1
来源：http://hz.yj20258888.top/gtaferxikp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ydzc1.top/gtnhvkcpjn.html

[M06] 向标准错误输出
来源：http://hz.yuanzhike.top/gtvyuhdfer.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinyuanbaomall.cn/gtxeztorbg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.316326.xyz/gtgqdzsovc.html

JS:   console.error("err")
来源：http://hz.zhijiandao.cn/gtrmfplahs.html

TS:   console.error("err")
来源：http://hz.jinyuanbaomall.cn/gtilqcssxh.html

Java: System.err.println("err")
来源：http://hz.xuetiantiany.cn/gtnjqlsobs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhijiandao.cn/gtoidttllv.html

Ruby: warn "err"
来源：http://hz.xziqi.cn/gtgsbpomac.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.sxryk.cn/gtqngqojjc.html

[M07] 判断是否为主入口
来源：http://hz.jiagoushi.top/gtzmurofxy.html

Py:   if __name__ == "__main__":
来源：http://hz.jinyuanbaomall.cn/gtieysptbc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ehwqpu.com/gtehwqdeyj.html

JS:   require.main === module
来源：http://hz.yvedp.cn/gtjbnyfyle.html

TS:   require.main === module
来源：http://hz.fengsongda.top/gtrebwsqqv.html

Java: public static void main(String[] args)
来源：http://hz.sweek.top/gtqwqxqeon.html

Go:   func main()
来源：http://hz.shanyushiyangkeji.top/gtildynxyo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhoulong.xyz/gttriukwiv.html

C#:   static void Main(string[] args)
来源：http://hz.yueranfly.top/gtxnqdmkgm.html

[M08] 获取系统与运行时信息
来源：http://hz.zhixingplan.top/gtwyludhls.html

Py:   platform.system();  platform.python_version()
来源：http://hz.haohaochexian.top/gtukoqbemn.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ybcxt.top/gtqnbgusui.html

JS:   process.platform;  process.version
来源：http://hz.vqdsnc.cn/gtufmbeqvb.html

TS:   process.platform;  process.version
来源：http://hz.xziqi.cn/gtjhijoqzp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cashguo.top/gtmoquxnej.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.dashuyun.cn/gthneqaelb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yj20258888.top/gtpdbeyseh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhongyouzk.top/gtkryhifjx.html

================================================================================
来源：http://hz.shzxlz.cn/gtdzjeqgap.html

N. 数据结构与算法
来源：http://hz.tanke756.top/gtipdtoeet.html

================================================================================
来源：http://hz.hammf.cn/gtkoqxjhix.html

[N01] 二分查找（有序数组）
来源：http://hz.yueranfly.top/gtyfthlomw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nanxinkj.top/gtbecujqmj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yongpay.top/gtwghxcfbl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgfzy.top/gtqwvzfwce.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258.top/gtimwgvafi.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shanyushiyangtech.top/gthzusseyo.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtnopyejwt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ywan-chungtsiang.top/gtvstateah.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yuanzhike.top/gtzhxizbbr.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jiagoushi.top/gtizzzgqmg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.svipenyu.cn/gtyplbdnrr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ywan-chungtsiang.top/gtwlmeiobb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258888.top/gtxfsnuvhu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nwbrower.top/gtduokedxx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.wangshuangyany.cn/gtonbmrnin.html

Go:   slices.Sort(arr)
来源：http://hz.hysaishi.cn/gttgypcdlr.html

Ruby: arr.sort
来源：http://hz.birdmap.top/gtrcvvfjyh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hammf.cn/gtrmklzfge.html

[N03] 快速排序（分治示例）
来源：http://hz.vqdsnc.cn/gtezondjpr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.chenzaomai.com/gtyfzpulkz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.daxiang520.top/gtneymyymq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tianlin.xyz/gtgveekzjg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuetiantiany.cn/gtuhzgxhpz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.bjfxy.top/gtldvfuvvs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xingfuxueyuan.xyz/gtmrdxxbmk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.fzhhl.top/gtedvseeqj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.c1oappe.top/gtzcpqtkod.html

[N04] 斐波那契数列
来源：http://hz.cdnleiting.top/gtffnluhff.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hongshengwenyu.top/gtwtufzztk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.wangdashe.top/gtcdajzkil.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jyoumei.cn/gtrifkmjve.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aibaodan.cn/gtamqendzy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.birdmap.top/gtahofzhum.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zdqjudy.top/gtchfnuata.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.iojbl.cn/gtvkgmhifa.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhaomingkeji.xyz/gtlhvgzsgx.html

[N05] 最大公约数
来源：http://hz.birdmap.top/gtdjzgbfxt.html

Py:   math.gcd(a, b)
来源：http://hz.gotoacloud.top/gtdlqxwenv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yuxming.cn/gtcuzzjhqd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangshuangyany.cn/gtsaovfehm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daxiang520.top/gtbjbisvfe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hysaishi.cn/gtrzfmooxk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinghuilouyu.cn/gtbuvdgyem.html

Ruby: a.gcd(b)
来源：http://hz.yvedp.cn/gtpbtxqizs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.52xcode.cn/gtifctoagu.html

[N06] 判断回文字符串
来源：http://hz.redwolf501.top/gtchcctvil.html

Py:   s == s[::-1]
来源：http://hz.aizwys.cn/gtguplgrpb.html

PHP:  $s === strrev($s);
来源：http://hz.shanyushiyangkeji.top/gtvbloncia.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hfpthk.cn/gthehgtznd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.nwbrower.top/gtujliqztu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yonumen.top/gtvawokwyc.html

Go:   // 双指针从两端比较
来源：http://hz.feifeiyinyue.top/gtuxsuoypv.html

Ruby: s == s.reverse
来源：http://hz.cdnleiting.top/gtfgzjtmvl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jqgufenzy.top/gtarqwmqfk.html

[N07] 两数之和（返回下标）
来源：http://hz.tian-w.cn/gtyhcghojo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.aizwys.cn/gtmfxrlrva.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.meibo888.top/gtgqpgegrd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.wangdashe.top/gtpzpvoxwh.html

TS:   // 手写 Map<string, number>
来源：http://hz.guannengcc.top/gtwmtfklvw.html

Java: // 手写 HashMap
来源：http://hz.cheryme.top/gthjbcazlv.html

Go:   // 手写 map[int]int
来源：http://hz.zhongyouzk.top/gttmbtqhao.html

Ruby: // 手写 Hash
来源：http://hz.zhaomingkeji.xyz/gthfawbpos.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.nwbrower.top/gtpnmuhnda.html

[N08] 生成全排列
来源：http://hz.meibo888.top/gtxezqejaa.html

Py:   itertools.permutations(arr)
来源：http://hz.iojbl.cn/gtduldrbfe.html

PHP:  // 手写递归交换
来源：http://hz.aizwys.cn/gtfvhbruuh.html

JS:   // 手写回溯递归
来源：http://hz.hysaishi.cn/gteprtzidk.html

TS:   // 手写回溯递归
来源：http://hz.redwolf501.top/gtboeoqbss.html

Java: // 手写回溯递归
来源：http://hz.zhixingplan.top/gtbtwfwsac.html

Go:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtiisgyyob.html

Ruby: arr.permutation.to_a
来源：http://hz.ywan-chungtsiang.top/gthdwvrvst.html

C#:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtdzkaeaaa.html

[N09] 栈与队列
来源：http://hz.zhoulong.xyz/gtsbfywyqk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ydjk.org.cn/gtzghaxthq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.svipenyu.cn/gtlazsycnb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yj20258.top/gtzvrcknos.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hongshengwenyu.top/gtbeqdfinz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.birdmap.top/gtzjsmjrdy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xinyue.icu/gtnodbemze.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhixingplan.top/gtvovcessl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.dianchejie.cn/gtlkkdwdnu.html

[N10] 链表节点定义
来源：http://hz.chenjidiqi.icu/gtkhkhfggz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.haohaochexian.top/gtyvnnoimu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zycfv.cn/gtqwnyxgsw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.wangdashe.top/gtenqbbelx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xylfe.cn/gttorifgwf.html

Java: class Node { int v; Node next; }
来源：http://hz.havefunace.top/gtgngslmmq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.9152youxi.cn/gttiqjnejd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cucudq.cn/gtzzjjikhp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cdnleiting.top/gtdxprsjts.html

[N11] 二叉树中序遍历
来源：http://hz.tianlin.xyz/gtsnvhjcyj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yj202588.top/gtpnclcjwb.html

PHP:  // 手写递归函数
来源：http://hz.xylfe.cn/gttmumwttg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guowangkeji.top/gtfouvwioy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.birdmap.top/gtzorwstrt.html

Java: // 手写递归
来源：http://hz.cqqwz.cn/gtyyoxxpcu.html

Go:   // 手写递归
来源：http://hz.nwbrower.top/gtmtphrmfz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jianghu66.top/gtcbmdfekh.html

C#:   // 手写递归
来源：http://hz.daria6918.cn/gtewtuviys.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gaohongyu789.top/gtxebzqyuq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.haohaochexian.top/gttmxjikzc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.redwolf501.top/gtpmrslqhv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xingfuxueyuan.xyz/gtucrbbqks.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.bjfxy.top/gtvikpjudw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cqqwz.cn/gtqeallijj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.havefunace.top/gtulsilspl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jianghu66.top/gtvvpinsgq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nwbrower.top/gtissowvbd.html

================================================================================
来源：http://hz.cucudq.cn/gtxdkmgyar.html

O. 并发与异步
来源：http://hz.0kj1m.cn/gtsyiylfma.html

================================================================================
来源：http://hz.chenzaomai.com/gtpasstpzc.html

[O01] 启动一个线程
来源：http://hz.yj20258.top/gtrrcbxlra.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.chenlongwang.top/gtfegqitea.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.dashuyun.cn/gtrjaumsik.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yuxming.cn/gtxligiixx.html

TS:   // 同 JS
来源：http://hz.kuanghao11.cn/gtidotctty.html

Java: new Thread(() -> f()).start()
来源：http://hz.hywenlv.cn/gteukycwdy.html

Go:   go f()
来源：http://hz.gogol.net.cn/gtjllteqdb.html

Ruby: Thread.new { f }
来源：http://hz.snrcjt.cn/gtlyejkyyh.html

C#:   Task.Run(() => F());
来源：http://hz.ppjwa.cn/gtarqjngzf.html

[O02] 使用线程池
来源：http://hz.jinqigufen.top/gtayucgvhc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.aizwys.cn/gtfoazfwki.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.snrcjt.cn/gtttwktwde.html

JS:   // worker_threads 线程池
来源：http://hz.yonumen.top/gtiuxurgvo.html

TS:   // worker_threads 线程池
来源：http://hz.dianchejie.cn/gtctdijbzw.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.mhx1999.top/gtgoamlxea.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.tanke756.top/gtduqzikms.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ivvv.top/gtarbvmzux.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.sysykeji.top/gtvxtcvxlh.html

[O03] 加锁保护共享数据
来源：http://hz.cucudq.cn/gtxhrlawmi.html

Py:   with lock: shared += 1
来源：http://hz.tanke756.top/gtrelmllfy.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhijiandao.cn/gtzosxnkgq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yonumen.top/gtfklbmwfv.html

TS:   // 同 JS
来源：http://hz.cucudq.cn/gtsfusbfgx.html

Java: synchronized (this) { shared++; }
来源：http://hz.havefunace.top/gtrvsgjjfa.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hywenlv.cn/gtlrnsioek.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.sysykeji.top/gtcecdoogi.html

C#:   lock (gate) { shared++; }
来源：http://hz.pycfn.com/gtornzgxkp.html

[O04] 定义异步函数并等待
来源：http://hz.nwbrower.top/gtqycdtbok.html

Py:   async def f():⏎    await g()
来源：http://hz.chenjidiqi.icu/gtpfnccweb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cashguo.top/gtyrclxqyd.html

JS:   async function f() { await g(); }
来源：http://hz.xylfe.cn/gtvtiyawta.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.wangshuangyany.cn/gtstxvrrsm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shangyingyoupin.top/gtwqcflbjw.html


<!-- 参考信息 -->