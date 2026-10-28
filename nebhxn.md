代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://hz.redwolf501.top/gtzwyvbjxu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zycfv.cn/gtbxyxsult.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ybcxt.top/gtqvokkhnz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yueranfly.top/gtruhcdyph.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xingfuxueyuan.xyz/gtwevywmkz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhaomingkeji.xyz/gtmlchcoki.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nanxuanxn.top/gtpgdjhpnf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xylfe.cn/gtpykpdghy.html

[L03] 设置自定义请求头
来源：http://hz.aizwys.cn/gtovuajusx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.iojbl.cn/gtwezdqbga.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.feifeiyinyue.top/gtpfnwtpdj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinghuilouyu.cn/gtqzotpasl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yangfankeji.com/gtwzpkybcl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sysykeji.top/gtkdotyatx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xylfe.cn/gtcqqxmazb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.iojbl.cn/gtbyscseqz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.9152youxi.cn/gtbunujpiz.html

[L04] 设置超时
来源：http://hz.snrcjt.cn/gtnuzdwbdk.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hnqzz.top/gthnhteesy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jlsjyb.cn/gtcqjqxdfp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigfzy.top/gtuhhoqzyi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigufen.top/gtaxagiqth.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.daxiang520.top/gtxlufpqhs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gaohongyu789.top/gtrlxjsiqg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.guowangkeji.top/gtcqokdpwl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gotoacloud.top/gtcrtidexb.html

[L05] 上传文件（multipart）
来源：http://hz.chenlongwang.top/gtsocubzvn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hammf.cn/gtbuzcoyqw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gzhubu.top/gtezgvuggb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.redwolf501.top/gtykjyslsz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cqqwz.cn/gtbalxkero.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ywan-chungtsiang.top/gtxsyssxzz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.tian-w.cn/gtjqldinjf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ybcxt.top/gtipxcpter.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.wangdashe.top/gtfnzyukwy.html

[L06] 解析响应为 JSON
来源：http://hz.52xcode.cn/gtnpovvryr.html

Py:   resp.json()
来源：http://hz.shzxlz.cn/gtdvzunqff.html

PHP:  json_decode($body, true);
来源：http://hz.smart0.xyz/gtxortombq.html

JS:   await resp.json()
来源：http://hz.zdqjudy.top/gtftymbpwn.html

TS:   await resp.json()
来源：http://hz.gogol.net.cn/gtgbroscew.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhengqikj.top/gtakshpzsr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.fzhhl.top/gtzskrcguc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yj202588.top/gtdalazqfa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhiwuduotai.top/gtqodlsqzm.html

[L07] 处理 HTTP 状态码
来源：http://hz.sxryk.cn/gtctxagrph.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sxryk.cn/gtjzcwauif.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.tianlin.xyz/gtkdqlhgem.html

JS:   resp.ok;  resp.status
来源：http://hz.cheryme.top/gtzgyqzjvh.html

TS:   resp.ok;  resp.status
来源：http://hz.yj20258.top/gtgpnuegdo.html

Java: resp.statusCode()
来源：http://hz.yanxiufei.cn/gtksdzjcee.html

Go:   resp.StatusCode
来源：http://hz.ehwqpu.com/gtzudlgygi.html

Ruby: resp.code.to_i
来源：http://hz.jinqigfzy.top/gtytnybcni.html

C#:   (int)resp.StatusCode
来源：http://hz.chenlongwang.top/gtibrkkelf.html

[L08] 并发请求多个地址
来源：http://hz.316326.xyz/gtaoianpwp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jianghu66.top/gteabgeehj.html

PHP:  curl_multi_init() 系列
来源：http://hz.shzxlz.cn/gtzrjdgapf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hongshengwenyu.top/gtiakhxsbp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hammf.cn/gtwmqjnbbh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tianlin.xyz/gtzrduciwd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ywan-chungtsiang.top/gtrmlxucbd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cqqwz.cn/gtruqmsnlm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cucudq.cn/gtmgjstejt.html

================================================================================
来源：http://hz.nanxuanxn.top/gtienfngnk.html

M. 命令行 / 进程 / 环境
来源：http://hz.yonumen.top/gtpqeuvgfc.html

================================================================================
来源：http://hz.bjfxy.top/gtrwmmhngb.html

[M01] 读取命令行参数
来源：http://hz.daxiang520.top/gtojhfjvvf.html

Py:   sys.argv[1:]
来源：http://hz.sxryk.cn/gtmmnmftcl.html

PHP:  $argv;  $argc;
来源：http://hz.hfpthk.cn/gtabglkpos.html

JS:   process.argv.slice(2)
来源：http://hz.sweek.top/gtysmwbejk.html

TS:   process.argv.slice(2)
来源：http://hz.shanyushiyangtech.top/gtjjlrkxew.html

Java: args 数组（main 方法参数）
来源：http://hz.ydzc1.top/gtnyuvslmj.html

Go:   os.Args[1:]
来源：http://hz.dashuyun.cn/gtxhhvvwkx.html

Ruby: ARGV
来源：http://hz.shangyingyoupin.top/gtyysiugpb.html

C#:   args 数组（Main 方法参数）
来源：http://hz.wangdashe.top/gtkvewzzpp.html

[M02] 读取环境变量
来源：http://hz.jinyuanbaomall.cn/gtqcqeedqf.html

Py:   os.environ.get("HOME")
来源：http://hz.tian-w.cn/gtisznkuyp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.dashuyun.cn/gtagqekvvy.html

JS:   process.env.HOME
来源：http://hz.vqdsnc.cn/gtgjjiujhl.html

TS:   process.env.HOME
来源：http://hz.redwolf501.top/gtiuydzquf.html

Java: System.getenv("HOME")
来源：http://hz.9152youxi.cn/gtkzqokiov.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cdnleiting.top/gtbmmldgii.html

Ruby: ENV["HOME"]
来源：http://hz.iojbl.cn/gtztohyzne.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.pengpengdd.cyou/gteipwsnyu.html

[M03] 执行外部命令
来源：http://hz.zhiwuduotai.top/gtzyigkrlc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xziqi.cn/gtumoowjxz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhiwuduotai.top/gtsxxtimlr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenlongwang.top/gtsywozhsy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.316326.xyz/gtmqruecew.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hongshengwenyu.top/gttjewqxku.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.fengsongda.top/gtnodopxrh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhengqikj.top/gtiygfwxxm.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shuidangran.top/gtlpmudand.html

[M04] 获取当前工作目录
来源：http://hz.yueranfly.top/gtcciiauoh.html

Py:   os.getcwd()
来源：http://hz.gaohongyu789.top/gtgfhdzdmo.html

PHP:  getcwd();
来源：http://hz.dianchejie.cn/gtjmspjhfy.html

JS:   process.cwd()
来源：http://hz.cheryme.top/gtiewembkz.html

TS:   process.cwd()
来源：http://hz.kuanghao11.cn/gtwpkxvzvn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.bjfxy.top/gtduqbwxnu.html

Go:   os.Getwd()
来源：http://hz.hnxiangtu.top/gtkfpdgptz.html

Ruby: Dir.pwd
来源：http://hz.0kj1m.cn/gttmngapka.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yvedp.cn/gtpgwzilgs.html

[M05] 设置退出码
来源：http://hz.shanyushiyangkeji.top/gtzimazcep.html

Py:   sys.exit(1)
来源：http://hz.gotoacloud.top/gthrfwqtak.html

PHP:  exit(1);
来源：http://hz.fzhhl.top/gtrspywggt.html

JS:   process.exit(1)
来源：http://hz.aizwys.cn/gtwxigcvgs.html

TS:   process.exit(1)
来源：http://hz.nwbrower.top/gtiwcgxriw.html

Java: System.exit(1)
来源：http://hz.yonumen.top/gtlrubkipz.html

Go:   os.Exit(1)
来源：http://hz.aibaodan.cn/gtvajfrdis.html

Ruby: exit 1
来源：http://hz.ydzc1.top/gtuyrmxzrx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.bjfxy.top/gtjtjabiqo.html

[M06] 向标准错误输出
来源：http://hz.gogol.net.cn/gtgeeshvne.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ehwqpu.com/gtikjaheah.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hnxiangtu.top/gtycwqfrta.html

JS:   console.error("err")
来源：http://hz.bjfxy.top/gthfpfxged.html

TS:   console.error("err")
来源：http://hz.jinqigfzy.top/gtxlsdqkco.html

Java: System.err.println("err")
来源：http://hz.jyoumei.cn/gtsgrladjr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jqgufenzy.top/gtprnocspw.html

Ruby: warn "err"
来源：http://hz.xuanzx.com/gtqtquuixu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.fengsongda.top/gtwpbbpvet.html

[M07] 判断是否为主入口
来源：http://hz.guannengcc.top/gtqtjrmosj.html

Py:   if __name__ == "__main__":
来源：http://hz.gaohongyu789.top/gtgofkyxuf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhengqikj.top/gtbtudhwlg.html

JS:   require.main === module
来源：http://hz.bjfxy.top/gtpeosnmwp.html

TS:   require.main === module
来源：http://hz.daxiang520.top/gtrkclmcoq.html

Java: public static void main(String[] args)
来源：http://hz.zhengqikj.top/gtvnqpcuvf.html

Go:   func main()
来源：http://hz.pycfn.com/gtroxjoprq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.pengpengdd.cyou/gtrafolnps.html

C#:   static void Main(string[] args)
来源：http://hz.sufxvd.cn/gtmjlmgvfo.html

[M08] 获取系统与运行时信息
来源：http://hz.hammf.cn/gtdzogqdin.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hywenlv.cn/gtauunweuu.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hywenlv.cn/gtzqydyhpy.html

JS:   process.platform;  process.version
来源：http://hz.iojbl.cn/gtxkdzwrnl.html

TS:   process.platform;  process.version
来源：http://hz.tian-w.cn/gtnpljfhwx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yj20258.top/gtdrlhgwpf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.pengpengdd.cyou/gtczzsvvee.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.pycfn.com/gtdrppuiyo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hywenlv.cn/gtoboqlwcy.html

================================================================================
来源：http://hz.xziqi.cn/gtzcuxexyj.html

N. 数据结构与算法
来源：http://hz.shanyushiyangkeji.top/gtgylqfvoo.html

================================================================================
来源：http://hz.andypj.xyz/gtwsnlyhrk.html

[N01] 二分查找（有序数组）
来源：http://hz.zycfv.cn/gtglegcypi.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.fengsongda.top/gtwbditqtq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gogol.net.cn/gtrsnoafxy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xziqi.cn/gtttfcytql.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhongyouzk.top/gtffhzpfnm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhixingplan.top/gtjmarvijd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ydjk.org.cn/gtxvalljuk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.cheryme.top/gtvhjkbcpu.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhongyouzk.top/gttvimooxk.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.smart0.xyz/gtzsusrzpt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.redwolf501.top/gttkutnsnc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.c1oappe.top/gtzirghodq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.haohaochexian.top/gtwpalhkuf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhengqikj.top/gtvwjqtwne.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yuanzhike.top/gtffhmydvi.html

Go:   slices.Sort(arr)
来源：http://hz.cucudq.cn/gtxwyierqw.html

Ruby: arr.sort
来源：http://hz.ydjk.org.cn/gttxoxlcop.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zdqjudy.top/gtfohnzdqe.html

[N03] 快速排序（分治示例）
来源：http://hz.hongshengwenyu.top/gtsumrxjtb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.fengsongda.top/gtyjmlxadc.html

PHP:  // 递归实现，或用 usort
来源：http://hz.haohaochexian.top/gtbvynaiki.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xingfuxueyuan.xyz/gtsukskkzz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sufxvd.cn/gtkaxpzahd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jyoumei.cn/gtzytcswji.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinqigfzy.top/gtybfdermi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.daria6918.cn/gtvgkcuybn.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jiagoushi.top/gtxmwymsnm.html

[N04] 斐波那契数列
来源：http://hz.gogol.net.cn/gtawwgkntd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tian-w.cn/gtpotxymep.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tian-w.cn/gtpvamuggy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.guowangkeji.top/gtihszwfjg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangtech.top/gtuaqsoncd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zdqjudy.top/gtkshnnegl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hammf.cn/gthlwrtiwr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.mhx1999.top/gtifrcntqz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xinyue.icu/gtfbqzkbjl.html

[N05] 最大公约数
来源：http://hz.dianchejie.cn/gtehohoifa.html

Py:   math.gcd(a, b)
来源：http://hz.tanke756.top/gtqjyfzfza.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.gogol.net.cn/gtmhhpfffr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gzhubu.top/gttznpoczo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenzaomai.com/gtbqdxtftm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.bjfxy.top/gtjopjxxpb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.tianlin.xyz/gtbwwjamql.html

Ruby: a.gcd(b)
来源：http://hz.pengpengdd.cyou/gtphznkasv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yj202588.top/gtabrkybvt.html

[N06] 判断回文字符串
来源：http://hz.zhiwuduotai.top/gttwxpymiz.html

Py:   s == s[::-1]
来源：http://hz.guowangkeji.top/gtqvqjdxwu.html

PHP:  $s === strrev($s);
来源：http://hz.jinghuilouyu.cn/gtltgkuytu.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtbouphyfn.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hongshengwenyu.top/gtkkwgbmjx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cheryme.top/gtrpjizhgs.html

Go:   // 双指针从两端比较
来源：http://hz.meibo888.top/gttsjqdfod.html

Ruby: s == s.reverse
来源：http://hz.hnqzz.top/gtaiwviigh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hammf.cn/gtlhwrvglk.html

[N07] 两数之和（返回下标）
来源：http://hz.tanke756.top/gtoqwiimpl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gzhubu.top/gtfikbdkar.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.nwbrower.top/gtyelojuay.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hysaishi.cn/gttrksqlia.html

TS:   // 手写 Map<string, number>
来源：http://hz.yonumen.top/gtmwpgsyxc.html

Java: // 手写 HashMap
来源：http://hz.sufxvd.cn/gtzzhsuspp.html

Go:   // 手写 map[int]int
来源：http://hz.zhaomingkeji.xyz/gtnvnhikjh.html

Ruby: // 手写 Hash
来源：http://hz.hfpthk.cn/gtbnieuqyn.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.tanke756.top/gtrettxibj.html

[N08] 生成全排列
来源：http://hz.gzhubu.top/gtvqfwqumi.html

Py:   itertools.permutations(arr)
来源：http://hz.iojbl.cn/gtlonzyzpb.html

PHP:  // 手写递归交换
来源：http://hz.jianghu66.top/gtieiroxsh.html

JS:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtrliqqxoi.html

TS:   // 手写回溯递归
来源：http://hz.daxiang520.top/gteuwpoopb.html

Java: // 手写回溯递归
来源：http://hz.sweek.top/gtvbasvwvv.html

Go:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtbbhkrljm.html

Ruby: arr.permutation.to_a
来源：http://hz.aizwys.cn/gttstwcfse.html

C#:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtplvkquxn.html

[N09] 栈与队列
来源：http://hz.chenzaomai.com/gteamkqvco.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jiagoushi.top/gttsdlsilo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhixingplan.top/gtghclugde.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.dashuyun.cn/gtcmqxscev.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.wangshuangyany.cn/gtyzhnrqyi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinghuilouyu.cn/gtvzdxnbbq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.mhx1999.top/gtszwfqlrw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shuidangran.top/gtxiuofuok.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shuidangran.top/gtrcvqgnen.html

[N10] 链表节点定义
来源：http://hz.gotoacloud.top/gtssuqpmll.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.svipenyu.cn/gtbetvkqua.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yanxiufei.cn/gtqugqofus.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.andypj.xyz/gtlknmiuzm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yj202588.top/gtawsbmzgx.html

Java: class Node { int v; Node next; }
来源：http://hz.gogol.net.cn/gthopahchu.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.c1oappe.top/gtnprysitw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.aizwys.cn/gtnfzhmnnh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xuetiantiany.cn/gtlptoemab.html

[N11] 二叉树中序遍历
来源：http://hz.shangyingyoupin.top/gtlerrdyls.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sweek.top/gttxoycpie.html

PHP:  // 手写递归函数
来源：http://hz.haohaochexian.top/gtgqzacdlf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pycfn.com/gtatnwlnhw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhoulong.xyz/gtyrhtexfd.html

Java: // 手写递归
来源：http://hz.feifeiyinyue.top/gtdpqsmlsg.html

Go:   // 手写递归
来源：http://hz.wangshuangyany.cn/gtidtqengy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xingfuxueyuan.xyz/gttrmrkmej.html

C#:   // 手写递归
来源：http://hz.zycfv.cn/gtvsurfvur.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhoulong.xyz/gtztgrbwgw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.316326.xyz/gtovkrshxl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yonumen.top/gtpejbbjze.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.c1oappe.top/gtzhhmpntx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jiagoushi.top/gtccxytzms.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhijiandao.cn/gteipjkwsx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.snrcjt.cn/gtcvxftndj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shanyushiyangkeji.top/gtfwrgrplm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nanxuanxn.top/gtxqnfzivm.html

================================================================================
来源：http://hz.ppjwa.cn/gtumuwucvt.html

O. 并发与异步
来源：http://hz.tanke756.top/gtyhsrhsfd.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtkocgsopr.html

[O01] 启动一个线程
来源：http://hz.smart0.xyz/gtkjrjqbih.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cheryme.top/gtcxeyheuk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.pengpengdd.cyou/gtuqfdhsos.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.andypj.xyz/gtdsnchzth.html

TS:   // 同 JS
来源：http://hz.yj20258888.top/gtnzciwehp.html

Java: new Thread(() -> f()).start()
来源：http://hz.cdnleiting.top/gttvmecpvf.html

Go:   go f()
来源：http://hz.shangyingyoupin.top/gtnbjblqet.html

Ruby: Thread.new { f }
来源：http://hz.hnxiangtu.top/gtmibdgyvz.html

C#:   Task.Run(() => F());
来源：http://hz.kuanghao11.cn/gthqsebhew.html

[O02] 使用线程池
来源：http://hz.shanyushiyangkeji.top/gtbkdcgzah.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.mhx1999.top/gtmflqvpoc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hongshengwenyu.top/gthnfbzscb.html

JS:   // worker_threads 线程池
来源：http://hz.yanxiufei.cn/gtbwllwyzr.html

TS:   // worker_threads 线程池
来源：http://hz.jyoumei.cn/gtvzlawswq.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.feifeiyinyue.top/gtmuznqguh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jinqigfzy.top/gtxjjfgwrq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.tanke756.top/gtfeozcuvh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.daria6918.cn/gtwqgeobvp.html

[O03] 加锁保护共享数据
来源：http://hz.hysaishi.cn/gtgdkkihqo.html

Py:   with lock: shared += 1
来源：http://hz.xziqi.cn/gtkcuducsm.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hywenlv.cn/gttpjschfz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hongshengwenyu.top/gtwmdurztj.html

TS:   // 同 JS
来源：http://hz.ywan-chungtsiang.top/gtrimlknbt.html

Java: synchronized (this) { shared++; }
来源：http://hz.cashguo.top/gtpllrvbsi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zycfv.cn/gtwciwiiyr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhongyouzk.top/gtwygvnfuy.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhongyouzk.top/gtckugwnpe.html

[O04] 定义异步函数并等待
来源：http://hz.gogol.net.cn/gtnlfcsjou.html

Py:   async def f():⏎    await g()
来源：http://hz.meibo888.top/gtfhvtxgdw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shanyushiyangtech.top/gtaoqomvbp.html

JS:   async function f() { await g(); }
来源：http://hz.zycfv.cn/gtgabdzzhg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.wangshuangyany.cn/gtrxdxgsqs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.havefunace.top/gtqijkhgpo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sxryk.cn/gttsynwjuy.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ppjwa.cn/gtomccaamw.html

C#:   async Task F() { await G(); }
来源：http://hz.tanke756.top/gtjwvjhtot.html

[O05] 并发执行并等待全部完成
来源：http://hz.ehwqpu.com/gtaqtbrkvg.html

Py:   asyncio.gather(*tasks)
来源：http://hz.quarkkingdee.top/gtdmszenbm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hysaishi.cn/gtytumxjhy.html

JS:   await Promise.all(tasks)
来源：http://hz.chenjidiqi.icu/gtbdyfhcpz.html

TS:   await Promise.all(tasks)
来源：http://hz.yonumen.top/gtwjgvetvv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jlsjyb.cn/gtbllrlnis.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.dianchejie.cn/gthherskux.html

Ruby: threads.map(&:join)
来源：http://hz.jinghuilouyu.cn/gtjkuibqnj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cheryme.top/gtznywqoda.html

[O06] 使用进程池
来源：http://hz.redwolf501.top/gtfbzwsfjo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.nanxinkj.top/gtkkpcupvz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yongpay.top/gtlbfjwgpo.html

JS:   // child_process / cluster 模块
来源：http://hz.yonumen.top/gtzhiojuif.html


<!-- 参考信息 -->