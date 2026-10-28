代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.havefunace.top/gtwbxygvta.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cdnleiting.top/gtjyyaruin.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hfpthk.cn/gtnawnmolz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.redwolf501.top/gtvslrexkh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.redwolf501.top/gtzlmtrrjq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yj20258888.top/gtgrbgvxkx.html

[L05] 上传文件（multipart）
来源：http://hz.sweek.top/gteirmohij.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.quarkkingdee.top/gthmbvmieo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.meibo888.top/gtndyciarc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.tanke756.top/gttndzvaqb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yongpay.top/gtlbuopiyt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jqgufenzy.top/gtxkxaedbg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.dianchejie.cn/gtnjxltwxe.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jqgufenzy.top/gtwifwbvjp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhengqikj.top/gtkndwbyij.html

[L06] 解析响应为 JSON
来源：http://hz.birdmap.top/gtkuimmpvq.html

Py:   resp.json()
来源：http://hz.andypj.xyz/gtceavkuas.html

PHP:  json_decode($body, true);
来源：http://hz.shuidangran.top/gtjlgkkpgw.html

JS:   await resp.json()
来源：http://hz.jqgfzy.top/gtxzadxwqa.html

TS:   await resp.json()
来源：http://hz.tanke756.top/gthbemrynu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shzxlz.cn/gtoaneewwt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.316326.xyz/gtszctkhpu.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cheryme.top/gtvhykityz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.wangdashe.top/gtqacqnsdp.html

[L07] 处理 HTTP 状态码
来源：http://hz.snrcjt.cn/gtbpfkcyjv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.52xcode.cn/gtjcaxmsdl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.smart0.xyz/gtjzcemvtd.html

JS:   resp.ok;  resp.status
来源：http://hz.316326.xyz/gtapfvpyig.html

TS:   resp.ok;  resp.status
来源：http://hz.ppjwa.cn/gtoycosqsw.html

Java: resp.statusCode()
来源：http://hz.ydjk.org.cn/gtbyvlyelc.html

Go:   resp.StatusCode
来源：http://hz.hywenlv.cn/gtsxsbisqg.html

Ruby: resp.code.to_i
来源：http://hz.yanxiufei.cn/gtmswtblwm.html

C#:   (int)resp.StatusCode
来源：http://hz.hammf.cn/gtwfvritpj.html

[L08] 并发请求多个地址
来源：http://hz.sysykeji.top/gtuyisgfcg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gogol.net.cn/gtlpqutmzg.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhiwuduotai.top/gtdnobanqv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.feifeiyinyue.top/gtpdgcfezo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nwbrower.top/gtdkfbjjhu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cheryme.top/gtibnyorew.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.nwbrower.top/gtqgtuqesu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.9152youxi.cn/gtblncigcf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yangfankeji.com/gtctxuifhh.html

================================================================================
来源：http://hz.mhx1999.top/gtyedluxcx.html

M. 命令行 / 进程 / 环境
来源：http://hz.jyoumei.cn/gtdnyaqxki.html

================================================================================
来源：http://hz.hammf.cn/gtlgfrlhsc.html

[M01] 读取命令行参数
来源：http://hz.ydzc1.top/gtguzmwkmm.html

Py:   sys.argv[1:]
来源：http://hz.nanxinkj.top/gtbrbbjolj.html

PHP:  $argv;  $argc;
来源：http://hz.chenzaomai.com/gtcpuxytqb.html

JS:   process.argv.slice(2)
来源：http://hz.snrcjt.cn/gtjlxpoozy.html

TS:   process.argv.slice(2)
来源：http://hz.sxryk.cn/gtzgvddkww.html

Java: args 数组（main 方法参数）
来源：http://hz.chenlongwang.top/gttbsjwvcw.html

Go:   os.Args[1:]
来源：http://hz.kuanghao11.cn/gttbgszmzd.html

Ruby: ARGV
来源：http://hz.guowangkeji.top/gtedyygqqv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sweek.top/gtqusdxbsl.html

[M02] 读取环境变量
来源：http://hz.cheryme.top/gtkvdhcggz.html

Py:   os.environ.get("HOME")
来源：http://hz.ydjk.org.cn/gtafazhkov.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shuidangran.top/gtxkkidgmu.html

JS:   process.env.HOME
来源：http://hz.redwolf501.top/gtxrpcfuep.html

TS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtajarzmxq.html

Java: System.getenv("HOME")
来源：http://hz.316326.xyz/gtvcozyhxb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hysaishi.cn/gthhjqliww.html

Ruby: ENV["HOME"]
来源：http://hz.meibo888.top/gtfdhtkkre.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.daria6918.cn/gtqfbyqjck.html

[M03] 执行外部命令
来源：http://hz.birdmap.top/gtbubdpkzn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zdqjudy.top/gtaavrugsi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.guannengcc.top/gthvrcaeal.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenjidiqi.icu/gtppsunjdu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yangfankeji.com/gtjgsrcidv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.c1oappe.top/gtcgdabekz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.andypj.xyz/gtmyavbzkf.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gaohongyu789.top/gtevlnnaio.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhongyouzk.top/gtuexwyrbg.html

[M04] 获取当前工作目录
来源：http://hz.zhoulong.xyz/gtzaoeaxgs.html

Py:   os.getcwd()
来源：http://hz.snrcjt.cn/gtyqrciqjy.html

PHP:  getcwd();
来源：http://hz.zhijiandao.cn/gtvbrzskjt.html

JS:   process.cwd()
来源：http://hz.xuetiantiany.cn/gtbemnbrde.html

TS:   process.cwd()
来源：http://hz.jiagoushi.top/gtsyctzcqx.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tianlin.xyz/gtgbibpigg.html

Go:   os.Getwd()
来源：http://hz.sxryk.cn/gthbafnote.html

Ruby: Dir.pwd
来源：http://hz.guannengcc.top/gtesuspfly.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.316326.xyz/gtqttobzrc.html

[M05] 设置退出码
来源：http://hz.ywan-chungtsiang.top/gtjtkpyuhh.html

Py:   sys.exit(1)
来源：http://hz.nwbrower.top/gtkrukcczu.html

PHP:  exit(1);
来源：http://hz.hongshengwenyu.top/gtdftqeimg.html

JS:   process.exit(1)
来源：http://hz.gotoacloud.top/gtmkxdaqtp.html

TS:   process.exit(1)
来源：http://hz.gzhubu.top/gtzcovhzjr.html

Java: System.exit(1)
来源：http://hz.zhongyouzk.top/gthvgkorlg.html

Go:   os.Exit(1)
来源：http://hz.hongshengwenyu.top/gtaksbxshl.html

Ruby: exit 1
来源：http://hz.sweek.top/gtojnovdyx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhaomingkeji.xyz/gtqcrpvkfu.html

[M06] 向标准错误输出
来源：http://hz.xziqi.cn/gtgqevxkxs.html

Py:   print("err", file=sys.stderr)
来源：http://hz.bjfxy.top/gtnzhkegrj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.daxiang520.top/gtfgirxjks.html

JS:   console.error("err")
来源：http://hz.yangfankeji.com/gtqzqrokzr.html

TS:   console.error("err")
来源：http://hz.zhengqikj.top/gtijqmjahp.html

Java: System.err.println("err")
来源：http://hz.haohaochexian.top/gtciannuha.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hnxiangtu.top/gtarykqhlo.html

Ruby: warn "err"
来源：http://hz.daria6918.cn/gtjwvjzabc.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.nanxuanxn.top/gthsusadml.html

[M07] 判断是否为主入口
来源：http://hz.nanxuanxn.top/gtxjfepryk.html

Py:   if __name__ == "__main__":
来源：http://hz.hfpthk.cn/gtiofjyfud.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.feifeiyinyue.top/gtyjgiihfl.html

JS:   require.main === module
来源：http://hz.jlsjyb.cn/gtxoqwqxkc.html

TS:   require.main === module
来源：http://hz.zhixingplan.top/gtcnoksvtj.html

Java: public static void main(String[] args)
来源：http://hz.ywan-chungtsiang.top/gtfqlviige.html

Go:   func main()
来源：http://hz.jinqigfzy.top/gtylrhjvpe.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinqigufen.top/gtwtnnthiz.html

C#:   static void Main(string[] args)
来源：http://hz.chenlongwang.top/gtamehpuoq.html

[M08] 获取系统与运行时信息
来源：http://hz.pycfn.com/gthhzxjrfx.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gotoacloud.top/gtjvxvqyjn.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tianlin.xyz/gttrzjcyoo.html

JS:   process.platform;  process.version
来源：http://hz.redwolf501.top/gtqgviluec.html

TS:   process.platform;  process.version
来源：http://hz.tanke756.top/gtekbvhisy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhongyouzk.top/gtgudxuvqh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jyoumei.cn/gtxckkilbl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.tanke756.top/gtjojwgusk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.52xcode.cn/gtthuzzqdk.html

================================================================================
来源：http://hz.kuanghao11.cn/gtjjmrjxni.html

N. 数据结构与算法
来源：http://hz.mhx1999.top/gtwhflqmmh.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtgbpnqdqv.html

[N01] 二分查找（有序数组）
来源：http://hz.cdnleiting.top/gtgktmgkax.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.dianchejie.cn/gtqjeqvxhb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.feifeiyinyue.top/gtgjnhfmli.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sxryk.cn/gtclaitahw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258888.top/gtwpkokagd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.dianchejie.cn/gtkfbwbncg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ppjwa.cn/gtbknloqzp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hammf.cn/gtlrhmvumt.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.havefunace.top/gtjedclkhs.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yuxming.cn/gtatrdgixx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xziqi.cn/gtiomemogn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shuidangran.top/gtorhsgwms.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ehwqpu.com/gtwclhaefr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sxryk.cn/gtojfdtzms.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhoulong.xyz/gtkxfsynlw.html

Go:   slices.Sort(arr)
来源：http://hz.meibo888.top/gtqcsycmeg.html

Ruby: arr.sort
来源：http://hz.dashuyun.cn/gtynfndkfd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yj20258.top/gtsswmmtjo.html

[N03] 快速排序（分治示例）
来源：http://hz.xingfuxueyuan.xyz/gtoqmljmsp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.nwbrower.top/gtzeijvzhb.html

PHP:  // 递归实现，或用 usort
来源：http://hz.snrcjt.cn/gtscvunsme.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cashguo.top/gtasysmwya.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenzaomai.com/gteuqinvbu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ybcxt.top/gtbvqspxsi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xuanzx.com/gtdjkqsdpv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.andypj.xyz/gthnvxqluu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jyoumei.cn/gtpwbolujk.html

[N04] 斐波那契数列
来源：http://hz.havefunace.top/gtbyignrdz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tian-w.cn/gtinmtiext.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cheryme.top/gtbrjniwnf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.haohaochexian.top/gtzmsyefrc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sysykeji.top/gturcijmrx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.birdmap.top/gtqmopvsfz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ehwqpu.com/gtfpottluv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.daria6918.cn/gtwotxuiog.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.fzhhl.top/gtivlwlhdu.html

[N05] 最大公约数
来源：http://hz.gotoacloud.top/gtpvoscfey.html

Py:   math.gcd(a, b)
来源：http://hz.gaohongyu789.top/gtszfviiuq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shzxlz.cn/gtyxvkutpk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dianchejie.cn/gtjacixgiq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jlsjyb.cn/gtskmiduew.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cdnleiting.top/gtclcvqigs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xziqi.cn/gtrqyxaglw.html

Ruby: a.gcd(b)
来源：http://hz.guannengcc.top/gtjuhqafut.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinghuilouyu.cn/gterehbdbe.html

[N06] 判断回文字符串
来源：http://hz.yuxming.cn/gtuhjxywxq.html

Py:   s == s[::-1]
来源：http://hz.jqgufenzy.top/gttnxvcwne.html

PHP:  $s === strrev($s);
来源：http://hz.zhijiandao.cn/gtxrkbvwpq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cashguo.top/gtidplhlyr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gturipbzmr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zycfv.cn/gtgcfdbdpc.html

Go:   // 双指针从两端比较
来源：http://hz.pengpengdd.cyou/gtsiqbougl.html

Ruby: s == s.reverse
来源：http://hz.dianchejie.cn/gtaozpxqwp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jianghu66.top/gtgrfbyuny.html

[N07] 两数之和（返回下标）
来源：http://hz.feifeiyinyue.top/gtfygatjlz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shuidangran.top/gtiwxkrqda.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yueranfly.top/gtzvuqyoym.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.meibo888.top/gtuamivnsv.html

TS:   // 手写 Map<string, number>
来源：http://hz.tianlin.xyz/gtonbvwrdl.html

Java: // 手写 HashMap
来源：http://hz.iojbl.cn/gtvsekizig.html

Go:   // 手写 map[int]int
来源：http://hz.hongshengwenyu.top/gtjuwptrlw.html

Ruby: // 手写 Hash
来源：http://hz.dianchejie.cn/gtuqqtkuom.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.wangdashe.top/gtknhebozk.html

[N08] 生成全排列
来源：http://hz.zhongyouzk.top/gtgihhhthj.html

Py:   itertools.permutations(arr)
来源：http://hz.wangshuangyany.cn/gtslbsbwvl.html

PHP:  // 手写递归交换
来源：http://hz.xziqi.cn/gtfbfbcgju.html

JS:   // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gtohpvhjhq.html

TS:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtogrbxgql.html

Java: // 手写回溯递归
来源：http://hz.tian-w.cn/gtkdjawekb.html

Go:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtklvrusws.html

Ruby: arr.permutation.to_a
来源：http://hz.yuanzhike.top/gtwsysxrlm.html

C#:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtnpfphinf.html

[N09] 栈与队列
来源：http://hz.hnxiangtu.top/gtcecajufe.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xingfuxueyuan.xyz/gtfwhvimtm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.feifeiyinyue.top/gtmkbaqknf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.chenlongwang.top/gtqytbtrxa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shuidangran.top/gtqwezepvk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.haohaochexian.top/gthhvyizrb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ywan-chungtsiang.top/gtqnnuvxhg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.mhx1999.top/gtyolyxmnw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ybcxt.top/gtuwwivexd.html

[N10] 链表节点定义
来源：http://hz.jinqigufen.top/gtxyfuyopj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xuanzx.com/gtjumhxuwt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sxryk.cn/gthpojyoft.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.quarkkingdee.top/gtodazsgcr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sufxvd.cn/gtpnpwwwlr.html

Java: class Node { int v; Node next; }
来源：http://hz.ivvv.top/gtqtcgcfab.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ydjk.org.cn/gtygsinkgv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.guowangkeji.top/gtnonbfgcm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jlsjyb.cn/gtmhnemdkz.html

[N11] 二叉树中序遍历
来源：http://hz.yj20258.top/gtanlwemik.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cdnleiting.top/gtwygynqsi.html

PHP:  // 手写递归函数
来源：http://hz.yanxiufei.cn/gtutwbhbdo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jyoumei.cn/gtvskuhdqs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj20258888.top/gtrmpstkrp.html

Java: // 手写递归
来源：http://hz.cqqwz.cn/gtlbjvtkis.html

Go:   // 手写递归
来源：http://hz.ydzc1.top/gtpnqxskhy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hammf.cn/gtrmbugpcm.html

C#:   // 手写递归
来源：http://hz.hfpthk.cn/gtklgneqqc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.daria6918.cn/gtpzxslgnn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tian-w.cn/gtffxllfzk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sweek.top/gtoddqnkzo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinyuanbaomall.cn/gtnmcwoawf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tianlin.xyz/gtvwzjihnl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.snrcjt.cn/gtlcysqdrs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.redwolf501.top/gtvqpzojnb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jianghu66.top/gteneiucza.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xziqi.cn/gtwddqvfcr.html

================================================================================
来源：http://hz.yueranfly.top/gtjduqmjph.html

O. 并发与异步
来源：http://hz.yj20258888.top/gtvcxqundk.html

================================================================================
来源：http://hz.kuanghao11.cn/gtvhevxsip.html

[O01] 启动一个线程
来源：http://hz.aizwys.cn/gtnxhboqks.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sxryk.cn/gtvayuhomb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.redwolf501.top/gtugyxctdv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.9152youxi.cn/gtfaxrohut.html

TS:   // 同 JS
来源：http://hz.zhoulong.xyz/gtdlxtspkp.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinyuanbaomall.cn/gtmtszpkkw.html

Go:   go f()
来源：http://hz.birdmap.top/gthmgqnnbm.html

Ruby: Thread.new { f }
来源：http://hz.cdnleiting.top/gtusytayba.html

C#:   Task.Run(() => F());
来源：http://hz.meibo888.top/gtpwspzozv.html

[O02] 使用线程池
来源：http://hz.feifeiyinyue.top/gtruicdqbi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hnqzz.top/gtcfrmxidq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.aizwys.cn/gtcigasjby.html

JS:   // worker_threads 线程池
来源：http://hz.jyoumei.cn/gtlctlitaz.html

TS:   // worker_threads 线程池
来源：http://hz.hongshengwenyu.top/gtntrdqqdp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yuxming.cn/gtizcmdiue.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.andypj.xyz/gtybncbnkb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ppjwa.cn/gtnsvethxa.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.nwbrower.top/gtjtrzzajx.html

[O03] 加锁保护共享数据
来源：http://hz.ppjwa.cn/gtpdiuakqx.html

Py:   with lock: shared += 1
来源：http://hz.tanke756.top/gtyivyblki.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.haohaochexian.top/gtachmoisg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhijiandao.cn/gtfwbxhznt.html

TS:   // 同 JS
来源：http://hz.jinqigfzy.top/gtfxhmnzjp.html

Java: synchronized (this) { shared++; }
来源：http://hz.birdmap.top/gtiikjzeci.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gaohongyu789.top/gtoqoyigyu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.feifeiyinyue.top/gtfhscnxqq.html

C#:   lock (gate) { shared++; }
来源：http://hz.ydjk.org.cn/gtvwuceneu.html

[O04] 定义异步函数并等待
来源：http://hz.ydjk.org.cn/gtslulnmgf.html

Py:   async def f():⏎    await g()
来源：http://hz.sweek.top/gtacmyhfyd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jqgufenzy.top/gtrwojfxtm.html

JS:   async function f() { await g(); }
来源：http://hz.aizwys.cn/gthqycdqbp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.chenjidiqi.icu/gthjlxodex.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.guowangkeji.top/gtqvwylyuf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.316326.xyz/gtmabfglly.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yanxiufei.cn/gtukfzkyit.html

C#:   async Task F() { await G(); }
来源：http://hz.yvedp.cn/gtadvccfgv.html

[O05] 并发执行并等待全部完成
来源：http://hz.xziqi.cn/gtemanzpxj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ybcxt.top/gtdheuwjgo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xingfuxueyuan.xyz/gthxjxforj.html

JS:   await Promise.all(tasks)
来源：http://hz.jinqigfzy.top/gtbsyazkkc.html

TS:   await Promise.all(tasks)
来源：http://hz.mhx1999.top/gtfirunjnz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.dashuyun.cn/gtxihgpzkc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhijiandao.cn/gthbinxkvq.html

Ruby: threads.map(&:join)
来源：http://hz.yj20258.top/gtvcxehsvj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yj20258888.top/gtmoylzvmw.html

[O06] 使用进程池
来源：http://hz.jinghuilouyu.cn/gtzuglmbun.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ydjk.org.cn/gtwcoooexl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zdqjudy.top/gtpgczhjwj.html

JS:   // child_process / cluster 模块
来源：http://hz.sxryk.cn/gtwhqedzkw.html

TS:   // child_process / cluster 模块
来源：http://hz.jyoumei.cn/gtvqavnkhv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.havefunace.top/gtudxjhdcs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.chenzaomai.com/gtvfvuhlmp.html

Ruby: // fork 块
来源：http://hz.nanxinkj.top/gtpiewuvim.html

C#:   Parallel.For
来源：http://hz.nanxuanxn.top/gtgkcbwvfa.html

================================================================================
来源：http://hz.sysykeji.top/gtmawytqgf.html

P. 常用工具函数
来源：http://hz.nanxuanxn.top/gtxpqeksck.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtyemnrxex.html

[P01] 生成 UUID
来源：http://hz.aibaodan.cn/gtoubxbhiy.html

Py:   str(uuid.uuid4())
来源：http://hz.zhijiandao.cn/gtadmsxshf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ywan-chungtsiang.top/gtipglhexy.html

JS:   crypto.randomUUID()
来源：http://hz.hywenlv.cn/gtzxajsuxz.html

TS:   crypto.randomUUID()
来源：http://hz.meibo888.top/gtycyxcoup.html

Java: UUID.randomUUID().toString()
来源：http://hz.nwbrower.top/gtxkhldwby.html

Go:   // 用 github.com/google/uuid
来源：http://hz.wangshuangyany.cn/gtlowxyxqd.html

Ruby: SecureRandom.uuid
来源：http://hz.zycfv.cn/gtuitdfrlr.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenlongwang.top/gtigcbhsjk.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yuanzhike.top/gtkmdxadwt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cqqwz.cn/gttowzbgku.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ppjwa.cn/gtxnlnzqgu.html


<!-- 参考信息 -->