代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.guowangkeji.top/gtneervxrr.html

[L04] 设置超时
来源：http://hz.havefunace.top/gtjiuprujf.html

Py:   requests.get(url, timeout=5)
来源：http://hz.chenlongwang.top/gtqfwsdkbw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.andypj.xyz/gtlhcpxljy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xingfuxueyuan.xyz/gtdbqeyjcp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shzxlz.cn/gttxgcjelj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yuanzhike.top/gtrghwsdet.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.smart0.xyz/gthkkcjpmd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhengqikj.top/gtksnhzrkv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.andypj.xyz/gtzxbuzlnl.html

[L05] 上传文件（multipart）
来源：http://hz.yanxiufei.cn/gtddiyescf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cqqwz.cn/gtbwhebaih.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gaohongyu789.top/gtzoaooppx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cqqwz.cn/gtmkphoavj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.dashuyun.cn/gtxxkfxdbr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yanxiufei.cn/gtbcodfaqr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xuetiantiany.cn/gtdsuotgjl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shanyushiyangkeji.top/gtycqhxdyn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.guowangkeji.top/gtwyndjvan.html

[L06] 解析响应为 JSON
来源：http://hz.gaohongyu789.top/gtpagfwlww.html

Py:   resp.json()
来源：http://hz.yj202588.top/gttaamvipl.html

PHP:  json_decode($body, true);
来源：http://hz.jqgfzy.top/gthddpwwwh.html

JS:   await resp.json()
来源：http://hz.ivvv.top/gtveousvdv.html

TS:   await resp.json()
来源：http://hz.ppjwa.cn/gtolxuhffw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shzxlz.cn/gtbnmmfwnh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shanyushiyangtech.top/gtibtpzdpw.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ydjk.org.cn/gtngdzhieh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.andypj.xyz/gtegumvbio.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinyuanbaomall.cn/gthbberwur.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yongpay.top/gtqgngzukx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.daxiang520.top/gtkjwzdtri.html

JS:   resp.ok;  resp.status
来源：http://hz.pengpengdd.cyou/gtccmikjid.html

TS:   resp.ok;  resp.status
来源：http://hz.sweek.top/gthaekomzp.html

Java: resp.statusCode()
来源：http://hz.gaohongyu789.top/gtowndyccj.html

Go:   resp.StatusCode
来源：http://hz.tianlin.xyz/gtbobldbps.html

Ruby: resp.code.to_i
来源：http://hz.dashuyun.cn/gtzjfknhti.html

C#:   (int)resp.StatusCode
来源：http://hz.ivvv.top/gtlghfmjdm.html

[L08] 并发请求多个地址
来源：http://hz.tanke756.top/gtqwtholjh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.c1oappe.top/gtkvagizhv.html

PHP:  curl_multi_init() 系列
来源：http://hz.tian-w.cn/gtpulbvpcu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fzhhl.top/gtysvjsofo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ywan-chungtsiang.top/gtmssshvsd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.feifeiyinyue.top/gtmczwmspc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.guannengcc.top/gtnsrxajxj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.tianlin.xyz/gtxulpgiok.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zycfv.cn/gtzaesmyyp.html

================================================================================
来源：http://hz.vqdsnc.cn/gtgnfohjwx.html

M. 命令行 / 进程 / 环境
来源：http://hz.aizwys.cn/gtqmglfcwd.html

================================================================================
来源：http://hz.gzhubu.top/gtvrfpeejy.html

[M01] 读取命令行参数
来源：http://hz.nanxuanxn.top/gtoudngiae.html

Py:   sys.argv[1:]
来源：http://hz.zhixingplan.top/gteosimpgx.html

PHP:  $argv;  $argc;
来源：http://hz.xziqi.cn/gtzmsjrqgi.html

JS:   process.argv.slice(2)
来源：http://hz.smart0.xyz/gtgferpkfu.html

TS:   process.argv.slice(2)
来源：http://hz.zhaomingkeji.xyz/gtoseawheu.html

Java: args 数组（main 方法参数）
来源：http://hz.haohaochexian.top/gttyjphhfs.html

Go:   os.Args[1:]
来源：http://hz.fengsongda.top/gtywlsfbyw.html

Ruby: ARGV
来源：http://hz.yj20258.top/gtinchddvm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.svipenyu.cn/gtzbpkmcjg.html

[M02] 读取环境变量
来源：http://hz.hysaishi.cn/gteekgiclz.html

Py:   os.environ.get("HOME")
来源：http://hz.52xcode.cn/gtheqhnzop.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.wangshuangyany.cn/gtcslixhvl.html

JS:   process.env.HOME
来源：http://hz.nanxinkj.top/gtzyziqxpo.html

TS:   process.env.HOME
来源：http://hz.havefunace.top/gtvtmbhdhz.html

Java: System.getenv("HOME")
来源：http://hz.shzxlz.cn/gtdbkfqdmg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yj20258.top/gtafjxufhs.html

Ruby: ENV["HOME"]
来源：http://hz.aibaodan.cn/gtmwjoyfvs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jqgfzy.top/gtchxgpbpu.html

[M03] 执行外部命令
来源：http://hz.zhixingplan.top/gttojdtoou.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.wangdashe.top/gtuucqymiz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cheryme.top/gttmvdlzwx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhoulong.xyz/gtmjmkppkq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.52xcode.cn/gtbvcxwoss.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.shzxlz.cn/gtjlhkncpn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.fzhhl.top/gtkppqfyhv.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yanxiufei.cn/gtvvktaeno.html

C#:   Process.Start("ls", "-l");
来源：http://hz.tian-w.cn/gtotflbewc.html

[M04] 获取当前工作目录
来源：http://hz.zhengqikj.top/gtqbqvhtpa.html

Py:   os.getcwd()
来源：http://hz.ppjwa.cn/gteqnlrugk.html

PHP:  getcwd();
来源：http://hz.zhixingplan.top/gtwekaytyv.html

JS:   process.cwd()
来源：http://hz.shangyingyoupin.top/gtdkwfogws.html

TS:   process.cwd()
来源：http://hz.birdmap.top/gtkykvjhrf.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jlsjyb.cn/gtkkzdksrh.html

Go:   os.Getwd()
来源：http://hz.nanxinkj.top/gtywsmipgh.html

Ruby: Dir.pwd
来源：http://hz.tian-w.cn/gtkhtxdodj.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.nanxinkj.top/gtgoszheyw.html

[M05] 设置退出码
来源：http://hz.yj202588.top/gtdllecnxb.html

Py:   sys.exit(1)
来源：http://hz.jinqigfzy.top/gtfjceacta.html

PHP:  exit(1);
来源：http://hz.hysaishi.cn/gtnbokuutb.html

JS:   process.exit(1)
来源：http://hz.sysykeji.top/gtuzqwfvui.html

TS:   process.exit(1)
来源：http://hz.c1oappe.top/gttmljaagn.html

Java: System.exit(1)
来源：http://hz.feifeiyinyue.top/gtqyqovmmz.html

Go:   os.Exit(1)
来源：http://hz.hnqzz.top/gtejxesxmi.html

Ruby: exit 1
来源：http://hz.haohaochexian.top/gtrfgkllof.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ydzc1.top/gtmhfwzeyr.html

[M06] 向标准错误输出
来源：http://hz.hywenlv.cn/gtbolgwuiy.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xuanzx.com/gtoenwwngp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenlongwang.top/gtoywrtfig.html

JS:   console.error("err")
来源：http://hz.ybcxt.top/gtxshofomu.html

TS:   console.error("err")
来源：http://hz.chenjidiqi.icu/gtozmcteqh.html

Java: System.err.println("err")
来源：http://hz.jqgufenzy.top/gtokwqoihg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.dianchejie.cn/gtbkmtdzuy.html

Ruby: warn "err"
来源：http://hz.c1oappe.top/gtmitdlsbi.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.quarkkingdee.top/gtlrmgshay.html

[M07] 判断是否为主入口
来源：http://hz.yongpay.top/gtizfasgfx.html

Py:   if __name__ == "__main__":
来源：http://hz.sxryk.cn/gtfcvmzxan.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yongpay.top/gtggwikbgp.html

JS:   require.main === module
来源：http://hz.guannengcc.top/gtjmioenkq.html

TS:   require.main === module
来源：http://hz.daria6918.cn/gtwnwoccry.html

Java: public static void main(String[] args)
来源：http://hz.dashuyun.cn/gtnvheexwq.html

Go:   func main()
来源：http://hz.nwbrower.top/gtpeuphmop.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shzxlz.cn/gtrodwqwwx.html

C#:   static void Main(string[] args)
来源：http://hz.chenjidiqi.icu/gtmpyaruyh.html

[M08] 获取系统与运行时信息
来源：http://hz.yj202588.top/gtfrdzlyrn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.wangdashe.top/gtfijuacnp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yanxiufei.cn/gtqlgxfdwq.html

JS:   process.platform;  process.version
来源：http://hz.hfpthk.cn/gthjaztxah.html

TS:   process.platform;  process.version
来源：http://hz.jqgfzy.top/gtetdaodgh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sweek.top/gtykjedhaq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yongpay.top/gtwfuzcqno.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.tianlin.xyz/gtymqmdajb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.quarkkingdee.top/gtjudiyhps.html

================================================================================
来源：http://hz.yuxming.cn/gtzchbviun.html

N. 数据结构与算法
来源：http://hz.jqgufenzy.top/gtdwxgpwqh.html

================================================================================
来源：http://hz.daxiang520.top/gtbbmefxpy.html

[N01] 二分查找（有序数组）
来源：http://hz.aizwys.cn/gtypcbykyt.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.aizwys.cn/gtvrpgljml.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.dianchejie.cn/gtlrjbarlf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gotoacloud.top/gtmpqpbgnm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zycfv.cn/gtmjgqkoeh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gaohongyu789.top/gtvwuakcke.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cashguo.top/gtqnltekce.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sysykeji.top/gtxksymooh.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shuidangran.top/gtsogimrrx.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.vqdsnc.cn/gtqvbkphjl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shzxlz.cn/gtekbjcqzm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hnqzz.top/gtxbsmcyie.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258.top/gtdluaslyh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhoulong.xyz/gtgypajmdi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.aizwys.cn/gtbfgamtlz.html

Go:   slices.Sort(arr)
来源：http://hz.sweek.top/gtkxwbpcph.html

Ruby: arr.sort
来源：http://hz.yonumen.top/gttwjfzwvr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhoulong.xyz/gtavsfnfes.html

[N03] 快速排序（分治示例）
来源：http://hz.yj20258888.top/gtgtvorsfh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yongpay.top/gtoutcjxdb.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gotoacloud.top/gtyyqquqwy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gaohongyu789.top/gtuvucyjfh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cheryme.top/gtgehjbeep.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.kuanghao11.cn/gthnmhqtus.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ywan-chungtsiang.top/gtdvnvtwnp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shuidangran.top/gtoezdzjoy.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yj202588.top/gtbmanltaz.html

[N04] 斐波那契数列
来源：http://hz.316326.xyz/gtzndjgxoe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xylfe.cn/gtjlysizlv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yangfankeji.com/gtlvtlnyuv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ppjwa.cn/gthbfxefym.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxinkj.top/gtyujfmtjc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yuanzhike.top/gtyqopxgpo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xylfe.cn/gtrbihobwo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.smart0.xyz/gtmbokuhjk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhongyouzk.top/gtnbslktby.html

[N05] 最大公约数
来源：http://hz.smart0.xyz/gtiejlsdhv.html

Py:   math.gcd(a, b)
来源：http://hz.gzhubu.top/gtssyhswtv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xuanzx.com/gtbdrznlsa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj20258888.top/gtoejfepso.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.haohaochexian.top/gtzahbyddw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.iojbl.cn/gtesuchcax.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.guowangkeji.top/gtnbzffgxv.html

Ruby: a.gcd(b)
来源：http://hz.aibaodan.cn/gtfssrczel.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.chenzaomai.com/gtqbhjgnff.html

[N06] 判断回文字符串
来源：http://hz.ehwqpu.com/gtrphkkaxq.html

Py:   s == s[::-1]
来源：http://hz.yj202588.top/gtmsmmrkpt.html

PHP:  $s === strrev($s);
来源：http://hz.sxryk.cn/gtikyqkcws.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtvlbxxarv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.fzhhl.top/gthqmymrbc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cucudq.cn/gtqingrfmz.html

Go:   // 双指针从两端比较
来源：http://hz.wangdashe.top/gtzqfzcrzi.html

Ruby: s == s.reverse
来源：http://hz.cucudq.cn/gttrjrbnmy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.daria6918.cn/gtcjbadbef.html

[N07] 两数之和（返回下标）
来源：http://hz.tanke756.top/gtitccspbu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xingfuxueyuan.xyz/gththstwbb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.chenzaomai.com/gturtfahah.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jyoumei.cn/gtszknoweo.html

TS:   // 手写 Map<string, number>
来源：http://hz.nanxuanxn.top/gttprybnzn.html

Java: // 手写 HashMap
来源：http://hz.yonumen.top/gtnsvxogog.html

Go:   // 手写 map[int]int
来源：http://hz.ydjk.org.cn/gtxotgqucx.html

Ruby: // 手写 Hash
来源：http://hz.xuetiantiany.cn/gtfmnfkffg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.nanxinkj.top/gtlgipraag.html

[N08] 生成全排列
来源：http://hz.fengsongda.top/gtjojvytwk.html

Py:   itertools.permutations(arr)
来源：http://hz.hongshengwenyu.top/gtqohywzaf.html

PHP:  // 手写递归交换
来源：http://hz.snrcjt.cn/gtbfitjsqy.html

JS:   // 手写回溯递归
来源：http://hz.yongpay.top/gtdeujiagp.html

TS:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtxsbfgfpi.html

Java: // 手写回溯递归
来源：http://hz.yj20258888.top/gtnczkkqjz.html

Go:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtdbtfqtip.html

Ruby: arr.permutation.to_a
来源：http://hz.jinyuanbaomall.cn/gtafjysdab.html

C#:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtxtxbosvo.html

[N09] 栈与队列
来源：http://hz.cdnleiting.top/gtkdaysryk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ydjk.org.cn/gtdzucrswv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xuetiantiany.cn/gtbukndhus.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.dianchejie.cn/gtixeotikq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jqgufenzy.top/gtviqbhpun.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhixingplan.top/gtasmfpuaw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tian-w.cn/gtciavycri.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.0kj1m.cn/gtdlsrqdpt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.c1oappe.top/gtkmnzktuh.html

[N10] 链表节点定义
来源：http://hz.quarkkingdee.top/gtcznpvrya.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xziqi.cn/gtspigquqs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.c1oappe.top/gtnrnwssrh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xuanzx.com/gtzbpwehwy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhongyouzk.top/gtjaezyymu.html

Java: class Node { int v; Node next; }
来源：http://hz.xuetiantiany.cn/gtcrstofvw.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yvedp.cn/gttgkzqolf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhoulong.xyz/gtxuhkkbsw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xziqi.cn/gtrxptrnlk.html

[N11] 二叉树中序遍历
来源：http://hz.zycfv.cn/gtzreknlue.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.aizwys.cn/gtsqykeckq.html

PHP:  // 手写递归函数
来源：http://hz.pycfn.com/gtqtykbhtg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhaomingkeji.xyz/gtohkelhil.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cqqwz.cn/gtbpobqhjo.html

Java: // 手写递归
来源：http://hz.shangyingyoupin.top/gtboaapblt.html

Go:   // 手写递归
来源：http://hz.pengpengdd.cyou/gtipgaqwyo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yanxiufei.cn/gtyfzhveik.html

C#:   // 手写递归
来源：http://hz.jiagoushi.top/gtnrlirwze.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhiwuduotai.top/gtxjfwizgi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hfpthk.cn/gtkkbdklaf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ywan-chungtsiang.top/gtaqfwgptj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhaomingkeji.xyz/gtdvusnmrl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shangyingyoupin.top/gtedlqsznp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cashguo.top/gtklembadc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.c1oappe.top/gtvnmabffe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.havefunace.top/gthrbmropu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuanzx.com/gtfcvtvlal.html

================================================================================
来源：http://hz.cucudq.cn/gtzpnkdnyc.html

O. 并发与异步
来源：http://hz.daria6918.cn/gtkunxnzjc.html

================================================================================
来源：http://hz.havefunace.top/gttpudtulu.html

[O01] 启动一个线程
来源：http://hz.guannengcc.top/gtvstyfmqy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yuxming.cn/gtrvigftlk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yanxiufei.cn/gthwmsyrzb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yuanzhike.top/gtuwrjoxng.html

TS:   // 同 JS
来源：http://hz.aibaodan.cn/gtbxxnrqjn.html

Java: new Thread(() -> f()).start()
来源：http://hz.birdmap.top/gtfkouplrk.html

Go:   go f()
来源：http://hz.shuidangran.top/gtqaisucwq.html

Ruby: Thread.new { f }
来源：http://hz.havefunace.top/gtucjydzqh.html

C#:   Task.Run(() => F());
来源：http://hz.xuanzx.com/gtjbmdgnre.html

[O02] 使用线程池
来源：http://hz.gogol.net.cn/gtrqgaerbx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yueranfly.top/gtnvcyexxm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hysaishi.cn/gtdgjvghmq.html

JS:   // worker_threads 线程池
来源：http://hz.meibo888.top/gtwnvrldpq.html

TS:   // worker_threads 线程池
来源：http://hz.zhoulong.xyz/gtravbpbms.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.vqdsnc.cn/gtprbqblnn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.guowangkeji.top/gtdryqlhxr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cucudq.cn/gturhipuhf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ehwqpu.com/gtluyrkuub.html

[O03] 加锁保护共享数据
来源：http://hz.cdnleiting.top/gtloqrfqbu.html

Py:   with lock: shared += 1
来源：http://hz.zhiwuduotai.top/gtrweumdrw.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.smart0.xyz/gtoeiqfwzx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.tanke756.top/gtkbizacaz.html

TS:   // 同 JS
来源：http://hz.gaohongyu789.top/gtjrruwvbp.html

Java: synchronized (this) { shared++; }
来源：http://hz.yangfankeji.com/gtppmzueep.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.tian-w.cn/gtkdxpzras.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.kuanghao11.cn/gtwxguizmo.html

C#:   lock (gate) { shared++; }
来源：http://hz.wangshuangyany.cn/gtzlbljhne.html

[O04] 定义异步函数并等待
来源：http://hz.zhaomingkeji.xyz/gtvssmavng.html

Py:   async def f():⏎    await g()
来源：http://hz.jinghuilouyu.cn/gtbkexwxyf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gzhubu.top/gtbjhhozvr.html

JS:   async function f() { await g(); }
来源：http://hz.ybcxt.top/gtugfhlbiz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.c1oappe.top/gtegkktzjv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jqgufenzy.top/gtdkcvpmyc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jinghuilouyu.cn/gtiehwghmj.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.nwbrower.top/gtpechemka.html

C#:   async Task F() { await G(); }
来源：http://hz.hnxiangtu.top/gtnvtdxzfb.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj20258.top/gtuptlwbzw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jyoumei.cn/gtxpnximmv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.nanxinkj.top/gthgwjyrve.html

JS:   await Promise.all(tasks)
来源：http://hz.jyoumei.cn/gtpcosrhcw.html

TS:   await Promise.all(tasks)
来源：http://hz.bjfxy.top/gturmaytwr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.c1oappe.top/gtzqxvvhbu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.svipenyu.cn/gthkxvtirw.html

Ruby: threads.map(&:join)
来源：http://hz.hongshengwenyu.top/gtaydehynh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yonumen.top/gtkxqoltxf.html

[O06] 使用进程池
来源：http://hz.zhongyouzk.top/gtdeykxpjv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ywan-chungtsiang.top/gtqddyfigu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hywenlv.cn/gtfzmqxrbh.html

JS:   // child_process / cluster 模块
来源：http://hz.zhongyouzk.top/gttvqcetki.html

TS:   // child_process / cluster 模块
来源：http://hz.yuanzhike.top/gtuawubxdh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xuanzx.com/gtgknybete.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hfpthk.cn/gtheujdwrp.html

Ruby: // fork 块
来源：http://hz.zdqjudy.top/gtagebovfj.html

C#:   Parallel.For
来源：http://hz.316326.xyz/gtveoogexl.html

================================================================================
来源：http://hz.iojbl.cn/gttbjohmlo.html

P. 常用工具函数
来源：http://hz.dianchejie.cn/gtqytotiqj.html

================================================================================
来源：http://hz.ehwqpu.com/gtkbpnvbtv.html

[P01] 生成 UUID
来源：http://hz.zdqjudy.top/gtdigsbvse.html

Py:   str(uuid.uuid4())
来源：http://hz.nanxuanxn.top/gtrzzswnvl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hfpthk.cn/gtbndjmkrf.html

JS:   crypto.randomUUID()
来源：http://hz.shuidangran.top/gtnhqnaece.html

TS:   crypto.randomUUID()
来源：http://hz.pengpengdd.cyou/gthkqdbpqn.html

Java: UUID.randomUUID().toString()
来源：http://hz.wangshuangyany.cn/gtlstljpau.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shzxlz.cn/gtrgmgkcgd.html

Ruby: SecureRandom.uuid
来源：http://hz.aizwys.cn/gtwonqyqfz.html


<!-- 参考信息 -->