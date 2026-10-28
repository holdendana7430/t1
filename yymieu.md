代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.vqdsnc.cn/gtmhwbxawt.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258888.top/gtrbsagnvl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yj202588.top/gtfmmlnekl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.pycfn.com/gthlxohofh.html

Go:   encoding/gob
来源：http://hz.52xcode.cn/gtblrsabou.html

Ruby: Marshal.dump(obj)
来源：http://hz.hongshengwenyu.top/gtwebzruqv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.c1oappe.top/gtumwrmzdt.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtfbpgckak.html

L. 网络请求
来源：http://hz.c1oappe.top/gttdoqjwqm.html

================================================================================
来源：http://hz.snrcjt.cn/gtbttmytpt.html

[L01] 发送 GET 请求
来源：http://hz.shanyushiyangtech.top/gtmqiqelqp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.sxryk.cn/gtasznfisz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenlongwang.top/gtbrssmndk.html

JS:   await fetch(url)
来源：http://hz.yj202588.top/gtgoosnntv.html

TS:   await fetch(url)
来源：http://hz.pycfn.com/gtdhrnyjzr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ybcxt.top/gtzqytwlwc.html

Go:   resp, err := http.Get(url)
来源：http://hz.cashguo.top/gtbtzswyfk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.wangshuangyany.cn/gtfulhxfcz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.smart0.xyz/gtyufspjsw.html

[L02] 发送 POST JSON
来源：http://hz.jinqigufen.top/gtrnhmojry.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hongshengwenyu.top/gtqbmkssqw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.redwolf501.top/gtgdjuaqou.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.316326.xyz/gtswbyngap.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.haohaochexian.top/gtspplchiq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gzhubu.top/gttloizkco.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.guowangkeji.top/gtspohlacn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hfpthk.cn/gtoioknckm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jyoumei.cn/gtfxfnzhhy.html

[L03] 设置自定义请求头
来源：http://hz.hysaishi.cn/gtxaybfjhc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinqigfzy.top/gtaweqlmng.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.0kj1m.cn/gtilfqdvuq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zdqjudy.top/gtzaelledk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhixingplan.top/gtwyjsmarn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.fzhhl.top/gtlwagnpbs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jqgfzy.top/gttjqmirej.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.tanke756.top/gtabxabara.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinqigfzy.top/gtitjfbspn.html

[L04] 设置超时
来源：http://hz.yueranfly.top/gtqasdrrxh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yueranfly.top/gtclhwowxv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.bjfxy.top/gtljvhzkpb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenzaomai.com/gtelqkjkzn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hongshengwenyu.top/gtqyivvgsl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.haohaochexian.top/gtkbzrawmw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.daria6918.cn/gtvfkzvknc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ppjwa.cn/gtbekxpurx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hysaishi.cn/gtzumsmjtc.html

[L05] 上传文件（multipart）
来源：http://hz.birdmap.top/gtntrycnzn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ehwqpu.com/gtpzatnkef.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hnqzz.top/gtetwvtnhg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yongpay.top/gtumnsklgw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cucudq.cn/gtmvtswsqo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jianghu66.top/gtqddkdjwv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xylfe.cn/gtioxvkdrx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ywan-chungtsiang.top/gthjiamvfs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.sxryk.cn/gtdccsaujq.html

[L06] 解析响应为 JSON
来源：http://hz.yongpay.top/gtcwifzbfc.html

Py:   resp.json()
来源：http://hz.iojbl.cn/gtwyhywzzw.html

PHP:  json_decode($body, true);
来源：http://hz.316326.xyz/gtcyveupyd.html

JS:   await resp.json()
来源：http://hz.chenlongwang.top/gteexfgych.html

TS:   await resp.json()
来源：http://hz.shanyushiyangtech.top/gtzotuiakn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.9152youxi.cn/gtzrmxuvrh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.bjfxy.top/gtgpvfbunr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cucudq.cn/gteunmanrw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.dianchejie.cn/gtduvmgitj.html

[L07] 处理 HTTP 状态码
来源：http://hz.yueranfly.top/gtncwstklp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhoulong.xyz/gtlcitfxgu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sufxvd.cn/gtixfmkhwl.html

JS:   resp.ok;  resp.status
来源：http://hz.gogol.net.cn/gtsvapktty.html

TS:   resp.ok;  resp.status
来源：http://hz.zhijiandao.cn/gtukbrbiqz.html

Java: resp.statusCode()
来源：http://hz.tianlin.xyz/gtmthtzgws.html

Go:   resp.StatusCode
来源：http://hz.ybcxt.top/gtwrrsyglg.html

Ruby: resp.code.to_i
来源：http://hz.ybcxt.top/gtxpkgbqci.html

C#:   (int)resp.StatusCode
来源：http://hz.chenlongwang.top/gtjnbliwkg.html

[L08] 并发请求多个地址
来源：http://hz.wangdashe.top/gttlrcgmsq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cdnleiting.top/gtxkmgnexs.html

PHP:  curl_multi_init() 系列
来源：http://hz.hnxiangtu.top/gtlfjzwykl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gtqnxiueyz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xylfe.cn/gtsoyyycqq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gotoacloud.top/gtxoetkoea.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yangfankeji.com/gtzcwbmijw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.wangshuangyany.cn/gtaasmebdu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ydjk.org.cn/gtykvmpnxb.html

================================================================================
来源：http://hz.xuanzx.com/gteejkjfxr.html

M. 命令行 / 进程 / 环境
来源：http://hz.shanyushiyangtech.top/gtohmydyew.html

================================================================================
来源：http://hz.chenzaomai.com/gthrmpmxnq.html

[M01] 读取命令行参数
来源：http://hz.jianghu66.top/gtgnqgpghs.html

Py:   sys.argv[1:]
来源：http://hz.fengsongda.top/gttrqxscyd.html

PHP:  $argv;  $argc;
来源：http://hz.yj20258.top/gtgchzdszd.html

JS:   process.argv.slice(2)
来源：http://hz.hammf.cn/gthpowaokq.html

TS:   process.argv.slice(2)
来源：http://hz.52xcode.cn/gtbhohigka.html

Java: args 数组（main 方法参数）
来源：http://hz.andypj.xyz/gtkxxksffj.html

Go:   os.Args[1:]
来源：http://hz.aizwys.cn/gtosmytsgm.html

Ruby: ARGV
来源：http://hz.sxryk.cn/gttqqvpgsq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yj202588.top/gtctvvoouj.html

[M02] 读取环境变量
来源：http://hz.gotoacloud.top/gtxugzuczo.html

Py:   os.environ.get("HOME")
来源：http://hz.yvedp.cn/gtqbepitoh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.wangshuangyany.cn/gtefqiuhdw.html

JS:   process.env.HOME
来源：http://hz.daxiang520.top/gtpnqcaroj.html

TS:   process.env.HOME
来源：http://hz.cdnleiting.top/gtdlverupo.html

Java: System.getenv("HOME")
来源：http://hz.snrcjt.cn/gtodghgpww.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sxryk.cn/gtgxaqunkf.html

Ruby: ENV["HOME"]
来源：http://hz.sysykeji.top/gtmygbycxn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.nanxinkj.top/gtmaajoxhn.html

[M03] 执行外部命令
来源：http://hz.xylfe.cn/gthkvyatxr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.pycfn.com/gtwibuqqfe.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinqigfzy.top/gtxntowvqf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.gzhubu.top/gtikzoeaxl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ybcxt.top/gtpelhimbc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.dianchejie.cn/gtxbfyzllr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jianghu66.top/gtmufrzayu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yongpay.top/gtkixtneye.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jyoumei.cn/gtnqpdczqp.html

[M04] 获取当前工作目录
来源：http://hz.havefunace.top/gtflvhcmgy.html

Py:   os.getcwd()
来源：http://hz.jinqigufen.top/gteixdbgux.html

PHP:  getcwd();
来源：http://hz.chenzaomai.com/gteekmvvgq.html

JS:   process.cwd()
来源：http://hz.shanyushiyangtech.top/gtuevdetsb.html

TS:   process.cwd()
来源：http://hz.cucudq.cn/gtkzwddfyg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ydzc1.top/gtjjiiirvb.html

Go:   os.Getwd()
来源：http://hz.jinqigufen.top/gtxzcitcfz.html

Ruby: Dir.pwd
来源：http://hz.52xcode.cn/gtbyrdrntg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ivvv.top/gtishopmri.html

[M05] 设置退出码
来源：http://hz.chenlongwang.top/gtggxtnywr.html

Py:   sys.exit(1)
来源：http://hz.zhaomingkeji.xyz/gtmeakopjl.html

PHP:  exit(1);
来源：http://hz.fengsongda.top/gtptbkxxyt.html

JS:   process.exit(1)
来源：http://hz.sufxvd.cn/gtkbivxnde.html

TS:   process.exit(1)
来源：http://hz.yongpay.top/gtcsizqqfb.html

Java: System.exit(1)
来源：http://hz.jlsjyb.cn/gttlyikoqz.html

Go:   os.Exit(1)
来源：http://hz.snrcjt.cn/gtxjprqfdd.html

Ruby: exit 1
来源：http://hz.xziqi.cn/gtnwgndrrz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gogol.net.cn/gttomkqcku.html

[M06] 向标准错误输出
来源：http://hz.zhongyouzk.top/gtovupikcm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xinyue.icu/gtlvstykea.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shangyingyoupin.top/gtittsicja.html

JS:   console.error("err")
来源：http://hz.smart0.xyz/gtcaarovpv.html

TS:   console.error("err")
来源：http://hz.gzhubu.top/gtejvllccd.html

Java: System.err.println("err")
来源：http://hz.xziqi.cn/gtwcfivyzv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cashguo.top/gtsybeltjm.html

Ruby: warn "err"
来源：http://hz.yj20258.top/gtypgbuhfq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hywenlv.cn/gtlcstxtjo.html

[M07] 判断是否为主入口
来源：http://hz.zhongyouzk.top/gtrwdsalrc.html

Py:   if __name__ == "__main__":
来源：http://hz.aizwys.cn/gtttehymgs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yongpay.top/gtyuxnomcb.html

JS:   require.main === module
来源：http://hz.nanxuanxn.top/gtpkeeyrge.html

TS:   require.main === module
来源：http://hz.hnqzz.top/gttjxhvoji.html

Java: public static void main(String[] args)
来源：http://hz.hongshengwenyu.top/gtdkazytts.html

Go:   func main()
来源：http://hz.xziqi.cn/gtcepyxmib.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.gotoacloud.top/gttpneryci.html

C#:   static void Main(string[] args)
来源：http://hz.guowangkeji.top/gtierplnvu.html

[M08] 获取系统与运行时信息
来源：http://hz.316326.xyz/gtixysruqm.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shanyushiyangtech.top/gtfsbmyrit.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.svipenyu.cn/gtyxexjkzw.html

JS:   process.platform;  process.version
来源：http://hz.jinqigfzy.top/gtemacwfgh.html

TS:   process.platform;  process.version
来源：http://hz.haohaochexian.top/gtjfubdkjt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cucudq.cn/gtdirfvbhr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.aibaodan.cn/gtodxafphi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.aibaodan.cn/gttouzokko.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xylfe.cn/gtkgpjysqh.html

================================================================================
来源：http://hz.jiagoushi.top/gtnoipcatp.html

N. 数据结构与算法
来源：http://hz.yonumen.top/gtetlnvhch.html

================================================================================
来源：http://hz.zhixingplan.top/gtranwzfmo.html

[N01] 二分查找（有序数组）
来源：http://hz.jinghuilouyu.cn/gtxgmlcguc.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nanxuanxn.top/gtfkcfarsx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.wangshuangyany.cn/gtmrunxrjr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sysykeji.top/gtyoqdmfwn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.svipenyu.cn/gtkuckdiop.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.nanxinkj.top/gtakmvuscd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenjidiqi.icu/gtcdhhxuet.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jlsjyb.cn/gtgbsecyhh.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.chenlongwang.top/gtvaaprxjt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ydjk.org.cn/gtqlyyjcwm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuetiantiany.cn/gtylfweopf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.dianchejie.cn/gtjylyswya.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.smart0.xyz/gteuqgsieg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.feifeiyinyue.top/gtiruijlqz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.gogol.net.cn/gtozwmxbpd.html

Go:   slices.Sort(arr)
来源：http://hz.zycfv.cn/gtzzqexwpu.html

Ruby: arr.sort
来源：http://hz.sxryk.cn/gtaqkmiqir.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yj20258.top/gtasbxpuec.html

[N03] 快速排序（分治示例）
来源：http://hz.shzxlz.cn/gtoabezvxr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.meibo888.top/gtqebjejet.html

PHP:  // 递归实现，或用 usort
来源：http://hz.fzhhl.top/gtelvqiccz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hysaishi.cn/gtlwozbghh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuanzhike.top/gtlgsvcnlo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tian-w.cn/gtdnfvpbee.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.pengpengdd.cyou/gtkjdpuybd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jinghuilouyu.cn/gtbkachujd.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.andypj.xyz/gtfvehajdp.html

[N04] 斐波那契数列
来源：http://hz.yueranfly.top/gtiqommpyf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.nwbrower.top/gtggjbpyks.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yanxiufei.cn/gtfiyfidfc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhixingplan.top/gtikwkyzhy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daxiang520.top/gtjrtgcbeh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xuanzx.com/gtjhgkwoxw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhaomingkeji.xyz/gtqczqwyly.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.feifeiyinyue.top/gtlrgphuzp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenlongwang.top/gtdfukznpb.html

[N05] 最大公约数
来源：http://hz.hywenlv.cn/gtdhbtozgd.html

Py:   math.gcd(a, b)
来源：http://hz.gogol.net.cn/gtwjctvmss.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.gaohongyu789.top/gtsswdmjqe.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.kuanghao11.cn/gtvlqyivrm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ywan-chungtsiang.top/gtbihxpgdz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cheryme.top/gtxndikrlw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.vqdsnc.cn/gtjuzswyzy.html

Ruby: a.gcd(b)
来源：http://hz.xuanzx.com/gtmyrvgozg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xingfuxueyuan.xyz/gtbavzdtzn.html

[N06] 判断回文字符串
来源：http://hz.hysaishi.cn/gtkdgqksow.html

Py:   s == s[::-1]
来源：http://hz.zycfv.cn/gtbqgekyxh.html

PHP:  $s === strrev($s);
来源：http://hz.pycfn.com/gtdmkdssji.html

JS:   s === [...s].reverse().join("")
来源：http://hz.havefunace.top/gtadzftwdz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtmlmvkfve.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.feifeiyinyue.top/gtutihleza.html

Go:   // 双指针从两端比较
来源：http://hz.smart0.xyz/gtmxufqflr.html

Ruby: s == s.reverse
来源：http://hz.wangshuangyany.cn/gtqraxacmp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.dashuyun.cn/gtcwdcvikr.html

[N07] 两数之和（返回下标）
来源：http://hz.shanyushiyangkeji.top/gtcntgrrjh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yuanzhike.top/gtfdqjtzps.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.nanxinkj.top/gtrmuojgpq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jyoumei.cn/gtkoppoany.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhijiandao.cn/gtvdjghmsu.html

Java: // 手写 HashMap
来源：http://hz.daxiang520.top/gtlvjdrjuo.html

Go:   // 手写 map[int]int
来源：http://hz.yongpay.top/gtncyvxeeo.html

Ruby: // 手写 Hash
来源：http://hz.jinqigfzy.top/gtsejwznca.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinqigfzy.top/gtmdvwtylh.html

[N08] 生成全排列
来源：http://hz.guowangkeji.top/gttuxqbgcd.html

Py:   itertools.permutations(arr)
来源：http://hz.tian-w.cn/gttwhuujty.html

PHP:  // 手写递归交换
来源：http://hz.gzhubu.top/gtmvdjakhy.html

JS:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtstxpwvrs.html

TS:   // 手写回溯递归
来源：http://hz.yueranfly.top/gttvhcbhoz.html

Java: // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtdznkpyie.html

Go:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtgypoxcws.html

Ruby: arr.permutation.to_a
来源：http://hz.nwbrower.top/gtcrazswjs.html

C#:   // 手写回溯递归
来源：http://hz.jqgfzy.top/gtqdytplem.html

[N09] 栈与队列
来源：http://hz.jyoumei.cn/gttaptwzhv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jiagoushi.top/gtrdniqhis.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jqgfzy.top/gtljuijbot.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xziqi.cn/gtflyqbmoa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.9152youxi.cn/gtbwdnorbc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yj202588.top/gthavnkozj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.svipenyu.cn/gtpypseenw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yueranfly.top/gtrtqjpwxn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.sweek.top/gtlscynoup.html

[N10] 链表节点定义
来源：http://hz.vqdsnc.cn/gtczfxmwue.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.nwbrower.top/gtmlxmcsgj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yj20258888.top/gtyldpauea.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hammf.cn/gtcfygbgmp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhongyouzk.top/gtpludvbad.html

Java: class Node { int v; Node next; }
来源：http://hz.pengpengdd.cyou/gtlrdkhzwv.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.quarkkingdee.top/gtdvtnkefi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yj20258888.top/gtciyqfgjy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.c1oappe.top/gtpqrwgqbn.html

[N11] 二叉树中序遍历
来源：http://hz.yj20258.top/gtnmjqdfkt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shanyushiyangkeji.top/gtqpxcapzn.html

PHP:  // 手写递归函数
来源：http://hz.pengpengdd.cyou/gtclggxunl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ywan-chungtsiang.top/gtlercdrhn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jlsjyb.cn/gttujepfes.html

Java: // 手写递归
来源：http://hz.nanxuanxn.top/gtsadksdiq.html

Go:   // 手写递归
来源：http://hz.hnqzz.top/gtpbxiwwyk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.316326.xyz/gtufdiyvrh.html

C#:   // 手写递归
来源：http://hz.snrcjt.cn/gtjrmsibfd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xylfe.cn/gtahfptknp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.kuanghao11.cn/gtdkhfgepa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinghuilouyu.cn/gtikctrhil.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuanzx.com/gtbchxfdhd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.pengpengdd.cyou/gthpruahhy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangshuangyany.cn/gtvezrbewu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.c1oappe.top/gtexslblni.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sxryk.cn/gtphmpcirw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shangyingyoupin.top/gtcxapvrwp.html

================================================================================
来源：http://hz.jianghu66.top/gtojkyufpj.html

O. 并发与异步
来源：http://hz.quarkkingdee.top/gtvtvdcfyu.html

================================================================================
来源：http://hz.xylfe.cn/gtxdckbxov.html

[O01] 启动一个线程
来源：http://hz.birdmap.top/gtnqlaaach.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jiagoushi.top/gtmlgyrlyn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.svipenyu.cn/gtfusvgzry.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gogol.net.cn/gtlwlgtwwe.html

TS:   // 同 JS
来源：http://hz.cashguo.top/gtlebabaqi.html

Java: new Thread(() -> f()).start()
来源：http://hz.zdqjudy.top/gtbqzasfug.html

Go:   go f()
来源：http://hz.yuxming.cn/gtvktwmsia.html

Ruby: Thread.new { f }
来源：http://hz.jqgufenzy.top/gtbyrkklzs.html

C#:   Task.Run(() => F());
来源：http://hz.tianlin.xyz/gtrsrpfbaf.html

[O02] 使用线程池
来源：http://hz.jianghu66.top/gtvmmqlepb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.gogol.net.cn/gtgcotiwgf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.mhx1999.top/gtbwitwlgh.html

JS:   // worker_threads 线程池
来源：http://hz.jyoumei.cn/gtymfjklkc.html

TS:   // worker_threads 线程池
来源：http://hz.pengpengdd.cyou/gteliuztqa.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jlsjyb.cn/gteeavguuh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.bjfxy.top/gtvjpjiaug.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.iojbl.cn/gtccjgxqwh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ivvv.top/gtlfdydumc.html

[O03] 加锁保护共享数据
来源：http://hz.0kj1m.cn/gtlryzbecq.html

Py:   with lock: shared += 1
来源：http://hz.cqqwz.cn/gtwnxrbips.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hywenlv.cn/gtixuqdffi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenzaomai.com/gtykwgbrap.html

TS:   // 同 JS
来源：http://hz.yuxming.cn/gtjhxtkton.html

Java: synchronized (this) { shared++; }
来源：http://hz.meibo888.top/gtmgkfbtzj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hfpthk.cn/gtklqvhwhq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yj20258888.top/gtwjvdvygb.html

C#:   lock (gate) { shared++; }
来源：http://hz.fengsongda.top/gtprczvcnf.html

[O04] 定义异步函数并等待
来源：http://hz.daxiang520.top/gtrgkzzhyp.html

Py:   async def f():⏎    await g()
来源：http://hz.yueranfly.top/gtsevcmwzr.html


<!-- 参考信息 -->