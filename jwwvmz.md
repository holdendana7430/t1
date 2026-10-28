代发 wailian999

L. 网络请求
来源：http://hz.xingfuxueyuan.xyz/gtfwfxanmt.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtllrwqgqw.html

[L01] 发送 GET 请求
来源：http://hz.ywan-chungtsiang.top/gtyhjogkvy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinqigfzy.top/gtwfmzlzne.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenlongwang.top/gtnstqzvzm.html

JS:   await fetch(url)
来源：http://hz.yongpay.top/gtpqxfoblk.html

TS:   await fetch(url)
来源：http://hz.fengsongda.top/gtengtzpzi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yangfankeji.com/gtfsnrgwid.html

Go:   resp, err := http.Get(url)
来源：http://hz.jqgufenzy.top/gtanxefslu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ywan-chungtsiang.top/gtmlrzanxw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yuxming.cn/gtqvzxupkv.html

[L02] 发送 POST JSON
来源：http://hz.birdmap.top/gtiqjrmgaa.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ydjk.org.cn/gtzkxrngsv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhixingplan.top/gtscavubbj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenzaomai.com/gtxczrltka.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenlongwang.top/gtriilxczz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.havefunace.top/gtrigtuvap.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.pycfn.com/gtomjdwwaz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jqgfzy.top/gtcjkvryut.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hongshengwenyu.top/gtejjcvnpg.html

[L03] 设置自定义请求头
来源：http://hz.haohaochexian.top/gtejsmvcqj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.52xcode.cn/gtskjwdcyr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.vqdsnc.cn/gtuivalfja.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guowangkeji.top/gtkyoequpe.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jianghu66.top/gtzgrxsehn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shanyushiyangkeji.top/gtpjgbuobe.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.daxiang520.top/gtmjzoirwv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.nanxuanxn.top/gthbfianpf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.redwolf501.top/gtkhozebhg.html

[L04] 设置超时
来源：http://hz.havefunace.top/gtsrggaawj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jyoumei.cn/gtquwtipki.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shzxlz.cn/gtvoswmxhj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ehwqpu.com/gtevrdttym.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhiwuduotai.top/gtbowqhgvz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.wangshuangyany.cn/gtmnauftno.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.52xcode.cn/gtyxookpri.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shanyushiyangkeji.top/gtdcjpfquf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.guowangkeji.top/gtiixwlszj.html

[L05] 上传文件（multipart）
来源：http://hz.jinyuanbaomall.cn/gtgqecefbt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj20258.top/gtejzwfogf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shanyushiyangtech.top/gtjhuvevcm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cheryme.top/gtspxinxbi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yongpay.top/gtywnmmfkk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ydjk.org.cn/gtdxnyronx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yuanzhike.top/gtnsfuklkb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.chenjidiqi.icu/gtesxufpar.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.pycfn.com/gtlexqonff.html

[L06] 解析响应为 JSON
来源：http://hz.zhiwuduotai.top/gtgujwmbte.html

Py:   resp.json()
来源：http://hz.xziqi.cn/gtmsssatlz.html

PHP:  json_decode($body, true);
来源：http://hz.shangyingyoupin.top/gtpsltucvy.html

JS:   await resp.json()
来源：http://hz.jinqigufen.top/gtaztyjuml.html

TS:   await resp.json()
来源：http://hz.jinqigfzy.top/gtfibssrzz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.smart0.xyz/gtkegwphyw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yj202588.top/gtxcetyqcr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenzaomai.com/gtgmdsiakn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.gotoacloud.top/gtkslubzto.html

[L07] 处理 HTTP 状态码
来源：http://hz.cucudq.cn/gtpbhtwhdi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jqgfzy.top/gtrzqonnnj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.daxiang520.top/gtskuvvair.html

JS:   resp.ok;  resp.status
来源：http://hz.ehwqpu.com/gtislkxykv.html

TS:   resp.ok;  resp.status
来源：http://hz.ybcxt.top/gtwevovalw.html

Java: resp.statusCode()
来源：http://hz.xylfe.cn/gtrglhvzix.html

Go:   resp.StatusCode
来源：http://hz.yj202588.top/gtayhguaba.html

Ruby: resp.code.to_i
来源：http://hz.hfpthk.cn/gtpfhslwui.html

C#:   (int)resp.StatusCode
来源：http://hz.cheryme.top/gttfyunoei.html

[L08] 并发请求多个地址
来源：http://hz.shanyushiyangkeji.top/gtlfmblayy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.havefunace.top/gtxqfywsdp.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj202588.top/gtpgacwsul.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cdnleiting.top/gtdphjtcge.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinghuilouyu.cn/gtydkaibar.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shanyushiyangtech.top/gtvivcfdox.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hnxiangtu.top/gtvyqaejkh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhongyouzk.top/gtjnqstnba.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shzxlz.cn/gttirnyyhz.html

================================================================================
来源：http://hz.bjfxy.top/gtmwqimack.html

M. 命令行 / 进程 / 环境
来源：http://hz.tanke756.top/gtqdxglfsg.html

================================================================================
来源：http://hz.yuxming.cn/gtidoedbeq.html

[M01] 读取命令行参数
来源：http://hz.aibaodan.cn/gtbhivzjyu.html

Py:   sys.argv[1:]
来源：http://hz.0kj1m.cn/gtqvevrehq.html

PHP:  $argv;  $argc;
来源：http://hz.vqdsnc.cn/gtlbknoylq.html

JS:   process.argv.slice(2)
来源：http://hz.xingfuxueyuan.xyz/gtxugkwtob.html

TS:   process.argv.slice(2)
来源：http://hz.shzxlz.cn/gtzvunzbek.html

Java: args 数组（main 方法参数）
来源：http://hz.hammf.cn/gtggzkespv.html

Go:   os.Args[1:]
来源：http://hz.tianlin.xyz/gtljlyohsd.html

Ruby: ARGV
来源：http://hz.hysaishi.cn/gttdvmsfgl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xuetiantiany.cn/gtwcdfdtxl.html

[M02] 读取环境变量
来源：http://hz.bjfxy.top/gtkbtwrcmm.html

Py:   os.environ.get("HOME")
来源：http://hz.mhx1999.top/gtjkczvrnk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ybcxt.top/gtvdjtunqv.html

JS:   process.env.HOME
来源：http://hz.ppjwa.cn/gtkfskcbug.html

TS:   process.env.HOME
来源：http://hz.quarkkingdee.top/gtnypnndhu.html

Java: System.getenv("HOME")
来源：http://hz.ybcxt.top/gtwqlpzckc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xinyue.icu/gtzlvlwmtr.html

Ruby: ENV["HOME"]
来源：http://hz.jinqigfzy.top/gtpgupejgs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.feifeiyinyue.top/gtorlzknfa.html

[M03] 执行外部命令
来源：http://hz.smart0.xyz/gtlrzswlrz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhoulong.xyz/gtyquouwdd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.316326.xyz/gtsixyqpmg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhoulong.xyz/gteqvqmdom.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ehwqpu.com/gtycqovglx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xziqi.cn/gtnkmoskfc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.gotoacloud.top/gtwqawodfh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hnxiangtu.top/gtaqzberfa.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jiagoushi.top/gtxwnywvup.html

[M04] 获取当前工作目录
来源：http://hz.iojbl.cn/gtuqarrryw.html

Py:   os.getcwd()
来源：http://hz.meibo888.top/gtmzpmunur.html

PHP:  getcwd();
来源：http://hz.yuxming.cn/gtvtytwgfa.html

JS:   process.cwd()
来源：http://hz.yj20258888.top/gtiknjuiml.html

TS:   process.cwd()
来源：http://hz.316326.xyz/gtpsrirsqd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.snrcjt.cn/gtajaxzyzz.html

Go:   os.Getwd()
来源：http://hz.quarkkingdee.top/gtdkvyjovf.html

Ruby: Dir.pwd
来源：http://hz.hfpthk.cn/gtbzotbxtt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhiwuduotai.top/gtceuklbzt.html

[M05] 设置退出码
来源：http://hz.shuidangran.top/gtxdxhvzok.html

Py:   sys.exit(1)
来源：http://hz.jinqigfzy.top/gtyvlyrxrt.html

PHP:  exit(1);
来源：http://hz.ybcxt.top/gtmpwwmvee.html

JS:   process.exit(1)
来源：http://hz.zhoulong.xyz/gtcmjbscvp.html

TS:   process.exit(1)
来源：http://hz.zhoulong.xyz/gtlmahiuxr.html

Java: System.exit(1)
来源：http://hz.xylfe.cn/gtqejixguu.html

Go:   os.Exit(1)
来源：http://hz.zdqjudy.top/gthwwybhwg.html

Ruby: exit 1
来源：http://hz.hysaishi.cn/gttfyhhncm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ybcxt.top/gtqqghhiid.html

[M06] 向标准错误输出
来源：http://hz.gaohongyu789.top/gtzdotozvv.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hnxiangtu.top/gtsnkfviey.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cqqwz.cn/gtaseorzhf.html

JS:   console.error("err")
来源：http://hz.xylfe.cn/gtiwmvrmeb.html

TS:   console.error("err")
来源：http://hz.tanke756.top/gtyxilusnc.html

Java: System.err.println("err")
来源：http://hz.jyoumei.cn/gtvbujsnif.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yj20258888.top/gtupqmtrgo.html

Ruby: warn "err"
来源：http://hz.andypj.xyz/gtkbezalhq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yuxming.cn/gtgiyccxgj.html

[M07] 判断是否为主入口
来源：http://hz.quarkkingdee.top/gtybafvtoa.html

Py:   if __name__ == "__main__":
来源：http://hz.aibaodan.cn/gtlxrmibzn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.sufxvd.cn/gtjgloekyt.html

JS:   require.main === module
来源：http://hz.guannengcc.top/gtsodcnocs.html

TS:   require.main === module
来源：http://hz.jqgufenzy.top/gtejdgdtpp.html

Java: public static void main(String[] args)
来源：http://hz.sysykeji.top/gttqvejljo.html

Go:   func main()
来源：http://hz.havefunace.top/gtxtymchna.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.haohaochexian.top/gtsujiqvka.html

C#:   static void Main(string[] args)
来源：http://hz.zhijiandao.cn/gtcpbkgajs.html

[M08] 获取系统与运行时信息
来源：http://hz.guowangkeji.top/gttmkjhoem.html

Py:   platform.system();  platform.python_version()
来源：http://hz.0kj1m.cn/gtgbiweraq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hnxiangtu.top/gtekvowumk.html

JS:   process.platform;  process.version
来源：http://hz.meibo888.top/gtvdkksdmd.html

TS:   process.platform;  process.version
来源：http://hz.jyoumei.cn/gtodflsbgc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tanke756.top/gtvtoawehp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhiwuduotai.top/gtolbufngj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ywan-chungtsiang.top/gtfwrgrrcw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yueranfly.top/gtmnxgujcj.html

================================================================================
来源：http://hz.cucudq.cn/gtnkkaqofm.html

N. 数据结构与算法
来源：http://hz.birdmap.top/gtrksjzxwl.html

================================================================================
来源：http://hz.shzxlz.cn/gtkzhsshav.html

[N01] 二分查找（有序数组）
来源：http://hz.andypj.xyz/gtcldzyvxb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhoulong.xyz/gtodjpegul.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cqqwz.cn/gtupjtceas.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.9152youxi.cn/gtxcndxefn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yuanzhike.top/gtyupdazuq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.tianlin.xyz/gtbhcgbvto.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jqgufenzy.top/gtkdhbvdtk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.chenjidiqi.icu/gtibgbiccx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.smart0.xyz/gtjctdfqwx.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ydzc1.top/gtyolsutxz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydjk.org.cn/gtoazftqgq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nwbrower.top/gthxbhsfkh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sxryk.cn/gtwcyaweks.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.meibo888.top/gtsyekiysi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ydzc1.top/gtraqobple.html

Go:   slices.Sort(arr)
来源：http://hz.zhengqikj.top/gtrkahfyfg.html

Ruby: arr.sort
来源：http://hz.jianghu66.top/gtfdlghpfl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.vqdsnc.cn/gtobdlygth.html

[N03] 快速排序（分治示例）
来源：http://hz.pycfn.com/gtcmargrwn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hysaishi.cn/gtdubwhqrm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.fzhhl.top/gtlogncvee.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.c1oappe.top/gtskvaxaan.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gotoacloud.top/gtxtuyhalt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhengqikj.top/gtfotlrkhu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nwbrower.top/gtjmgdcmvo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yuxming.cn/gtjcjyopwf.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.smart0.xyz/gtcsgjxsya.html

[N04] 斐波那契数列
来源：http://hz.yangfankeji.com/gtkukdnfqf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jqgfzy.top/gtlshokisn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ehwqpu.com/gtibmvvupt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.meibo888.top/gtqjtnvprh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ivvv.top/gtralzoizo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.guannengcc.top/gtgjopwabe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhongyouzk.top/gtqnlzcbpi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.iojbl.cn/gtpabkwuot.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.aizwys.cn/gtzkzjutjd.html

[N05] 最大公约数
来源：http://hz.cdnleiting.top/gtykjkovup.html

Py:   math.gcd(a, b)
来源：http://hz.ywan-chungtsiang.top/gtywcbbpxn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sysykeji.top/gtmpgymgqd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj202588.top/gtjozfwuxq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nanxinkj.top/gtqfbbiqaq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.svipenyu.cn/gtgmdfxypx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jqgfzy.top/gtvbvzkkfx.html

Ruby: a.gcd(b)
来源：http://hz.yonumen.top/gtfsgustnz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jqgufenzy.top/gttorwyxss.html

[N06] 判断回文字符串
来源：http://hz.shanyushiyangtech.top/gtjcqvfsxy.html

Py:   s == s[::-1]
来源：http://hz.redwolf501.top/gteckbavyw.html

PHP:  $s === strrev($s);
来源：http://hz.yj20258888.top/gtbznmwewn.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jinqigufen.top/gtbeusucrd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtbhskqbxy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.0kj1m.cn/gtccmhaaue.html

Go:   // 双指针从两端比较
来源：http://hz.pengpengdd.cyou/gtjthvnhyn.html

Ruby: s == s.reverse
来源：http://hz.gaohongyu789.top/gthulpxmsq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.guannengcc.top/gtkxkekcmj.html

[N07] 两数之和（返回下标）
来源：http://hz.tanke756.top/gtkmpqrspq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shangyingyoupin.top/gtysqihpgh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.guowangkeji.top/gtxsfatbvj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sxryk.cn/gtoruoshnw.html

TS:   // 手写 Map<string, number>
来源：http://hz.jiagoushi.top/gtvknktjqu.html

Java: // 手写 HashMap
来源：http://hz.yj20258888.top/gtkjkzowrt.html

Go:   // 手写 map[int]int
来源：http://hz.yvedp.cn/gteuwreuzs.html

Ruby: // 手写 Hash
来源：http://hz.hfpthk.cn/gtednijjnj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.havefunace.top/gtxnurppgm.html

[N08] 生成全排列
来源：http://hz.zhiwuduotai.top/gtmzmgsvso.html

Py:   itertools.permutations(arr)
来源：http://hz.jqgfzy.top/gtlwmofaud.html

PHP:  // 手写递归交换
来源：http://hz.shzxlz.cn/gtltpqjamx.html

JS:   // 手写回溯递归
来源：http://hz.birdmap.top/gtpwwsydmi.html

TS:   // 手写回溯递归
来源：http://hz.daxiang520.top/gtaaznrpkw.html

Java: // 手写回溯递归
来源：http://hz.xziqi.cn/gtqnqoqnst.html

Go:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gthwreebuu.html

Ruby: arr.permutation.to_a
来源：http://hz.xuetiantiany.cn/gtdamzihgs.html

C#:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtwetnseil.html

[N09] 栈与队列
来源：http://hz.gogol.net.cn/gtbceezykp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sufxvd.cn/gtujdybsyd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yj20258.top/gtghsmcutz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xylfe.cn/gttplpqbxh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.redwolf501.top/gtrsquiplb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xziqi.cn/gtguedrurs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yvedp.cn/gtcoytllmp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.redwolf501.top/gtdyvsvvel.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinqigufen.top/gtmeytdxvd.html

[N10] 链表节点定义
来源：http://hz.0kj1m.cn/gtujemmcxf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhijiandao.cn/gtacealazj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.dashuyun.cn/gtkfbzxnaq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.feifeiyinyue.top/gtutjbyhis.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zdqjudy.top/gtptjzdvkp.html

Java: class Node { int v; Node next; }
来源：http://hz.guannengcc.top/gtrcmbwzcp.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shzxlz.cn/gtmsrinupm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jqgfzy.top/gtfototqli.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.dashuyun.cn/gtsebsousj.html

[N11] 二叉树中序遍历
来源：http://hz.zdqjudy.top/gtezdyoruq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hnxiangtu.top/gtzzndouja.html

PHP:  // 手写递归函数
来源：http://hz.shangyingyoupin.top/gtmcijaltb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj20258.top/gtyghppepb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuanzhike.top/gtglmpxewc.html

Java: // 手写递归
来源：http://hz.feifeiyinyue.top/gtprefkuqr.html

Go:   // 手写递归
来源：http://hz.birdmap.top/gtzyxmciwd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cdnleiting.top/gtzwjlwvpv.html

C#:   // 手写递归
来源：http://hz.guannengcc.top/gtljhyniwu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jqgufenzy.top/gtiiupudgx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zycfv.cn/gtameqajky.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhoulong.xyz/gthjnzxihu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangkeji.top/gtejbwszqp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinqigfzy.top/gtglzrghyb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hnqzz.top/gtpbbfayqn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.mhx1999.top/gtapgkszra.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhixingplan.top/gttkhfmzmx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hnqzz.top/gtiamiwzil.html

================================================================================
来源：http://hz.guannengcc.top/gtdbrlgukb.html

O. 并发与异步
来源：http://hz.yj20258.top/gtwjehadgu.html

================================================================================
来源：http://hz.gogol.net.cn/gtforewkao.html

[O01] 启动一个线程
来源：http://hz.yangfankeji.com/gtzbubtlec.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.guannengcc.top/gtvjqyhwsm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.wangshuangyany.cn/gtjkgclkos.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.quarkkingdee.top/gtrksihsqi.html

TS:   // 同 JS
来源：http://hz.pycfn.com/gtrfdooqth.html

Java: new Thread(() -> f()).start()
来源：http://hz.yuanzhike.top/gtflpcrrof.html

Go:   go f()
来源：http://hz.pycfn.com/gtdenldacd.html

Ruby: Thread.new { f }
来源：http://hz.shanyushiyangkeji.top/gtcdxycciz.html

C#:   Task.Run(() => F());
来源：http://hz.zhixingplan.top/gtusokbtqe.html

[O02] 使用线程池
来源：http://hz.cqqwz.cn/gtenhazfft.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yanxiufei.cn/gtnxlrbpcn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yj20258.top/gtxcwbdngk.html

JS:   // worker_threads 线程池
来源：http://hz.ehwqpu.com/gtmapsiljd.html

TS:   // worker_threads 线程池
来源：http://hz.xuetiantiany.cn/gtimpdrseo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.iojbl.cn/gtcxkxtexr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.pengpengdd.cyou/gtlvksjoih.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.fengsongda.top/gtezcdmuex.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.tianlin.xyz/gtuchacxmg.html

[O03] 加锁保护共享数据
来源：http://hz.gzhubu.top/gthutjprka.html

Py:   with lock: shared += 1
来源：http://hz.0kj1m.cn/gtuzmcbafm.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jlsjyb.cn/gtcmqiajzb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gotoacloud.top/gtzqkjerpj.html

TS:   // 同 JS
来源：http://hz.hysaishi.cn/gtxmxasmxk.html

Java: synchronized (this) { shared++; }
来源：http://hz.yuanzhike.top/gtvdtlovmo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.tanke756.top/gtmzurldnc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.sufxvd.cn/gtocdhpklq.html

C#:   lock (gate) { shared++; }
来源：http://hz.0kj1m.cn/gtmjephhnc.html

[O04] 定义异步函数并等待
来源：http://hz.meibo888.top/gtnipbphub.html

Py:   async def f():⏎    await g()
来源：http://hz.jinghuilouyu.cn/gtrdzxdubz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.316326.xyz/gthqglzxyz.html

JS:   async function f() { await g(); }
来源：http://hz.hywenlv.cn/gtextkcyxh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yongpay.top/gttcsjhgkv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ydjk.org.cn/gthbeiyuct.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.mhx1999.top/gtrscnfoos.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.mhx1999.top/gtknmxwlrb.html

C#:   async Task F() { await G(); }
来源：http://hz.gogol.net.cn/gtjjxwfyrp.html

[O05] 并发执行并等待全部完成
来源：http://hz.sufxvd.cn/gtydqgbuar.html


<!-- 参考信息 -->