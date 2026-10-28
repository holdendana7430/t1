代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yj20258.top/gtsmanweio.html

[L04] 设置超时
来源：http://hz.c1oappe.top/gtzoydhnle.html

Py:   requests.get(url, timeout=5)
来源：http://hz.52xcode.cn/gtmhbczmib.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sysykeji.top/gtnmaxfvvf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ydjk.org.cn/gtihmstefm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hywenlv.cn/gtkiprlxgc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.nanxuanxn.top/gtfyknfpfv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj20258888.top/gtgnymtkke.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.quarkkingdee.top/gttpbgovup.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.andypj.xyz/gteejnzkjt.html

[L05] 上传文件（multipart）
来源：http://hz.hnqzz.top/gtrxhelhkc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yanxiufei.cn/gtgqefajit.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinyuanbaomall.cn/gtxumvlxxi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yongpay.top/gtjfuntesj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.316326.xyz/gtadajschf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.birdmap.top/gtkqeitixm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yj20258888.top/gtrvnliqqa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinqigfzy.top/gtatxzjzdi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhaomingkeji.xyz/gtixchhmoi.html

[L06] 解析响应为 JSON
来源：http://hz.mhx1999.top/gtmimypwpu.html

Py:   resp.json()
来源：http://hz.0kj1m.cn/gtgkuumjxg.html

PHP:  json_decode($body, true);
来源：http://hz.nanxuanxn.top/gtepvnuiyv.html

JS:   await resp.json()
来源：http://hz.fengsongda.top/gtttvylzmg.html

TS:   await resp.json()
来源：http://hz.zhijiandao.cn/gtpjgixath.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.wangshuangyany.cn/gtrgsyuocl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.guowangkeji.top/gtjmeaemsj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinqigufen.top/gtuctcjctk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhoulong.xyz/gtkhzzwdnl.html

[L07] 处理 HTTP 状态码
来源：http://hz.hongshengwenyu.top/gtmifgoiyj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.redwolf501.top/gtmxnrnvgb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.0kj1m.cn/gtidcyaxxe.html

JS:   resp.ok;  resp.status
来源：http://hz.ivvv.top/gttzrtjiit.html

TS:   resp.ok;  resp.status
来源：http://hz.ivvv.top/gtgopztkhb.html

Java: resp.statusCode()
来源：http://hz.yongpay.top/gtovrtnrxh.html

Go:   resp.StatusCode
来源：http://hz.svipenyu.cn/gtqpibgool.html

Ruby: resp.code.to_i
来源：http://hz.mhx1999.top/gtodjaymso.html

C#:   (int)resp.StatusCode
来源：http://hz.zdqjudy.top/gtomeyruws.html

[L08] 并发请求多个地址
来源：http://hz.aizwys.cn/gtjrihfjkn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.nanxuanxn.top/gtsrymutjz.html

PHP:  curl_multi_init() 系列
来源：http://hz.hammf.cn/gttbiqmovx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sxryk.cn/gtioswtguw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.birdmap.top/gtlqpdpeuc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhiwuduotai.top/gtqeugtcih.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hywenlv.cn/gtgnlekqcg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shuidangran.top/gtorcbzmvm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinghuilouyu.cn/gtmibsorsr.html

================================================================================
来源：http://hz.sysykeji.top/gteqggbisw.html

M. 命令行 / 进程 / 环境
来源：http://hz.yangfankeji.com/gtcdkqclwk.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtgvumfzgq.html

[M01] 读取命令行参数
来源：http://hz.aibaodan.cn/gtcvrpzuch.html

Py:   sys.argv[1:]
来源：http://hz.jyoumei.cn/gtcbueomow.html

PHP:  $argv;  $argc;
来源：http://hz.kuanghao11.cn/gtwffjcvtr.html

JS:   process.argv.slice(2)
来源：http://hz.hnxiangtu.top/gtkrltmyds.html

TS:   process.argv.slice(2)
来源：http://hz.yj202588.top/gtbvqooqqy.html

Java: args 数组（main 方法参数）
来源：http://hz.bjfxy.top/gtzucokktx.html

Go:   os.Args[1:]
来源：http://hz.zdqjudy.top/gtidovwqyh.html

Ruby: ARGV
来源：http://hz.yongpay.top/gtlwobhjac.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jlsjyb.cn/gtmdjbfygu.html

[M02] 读取环境变量
来源：http://hz.jinqigfzy.top/gthjqakyqu.html

Py:   os.environ.get("HOME")
来源：http://hz.xuetiantiany.cn/gtaysotmyb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sysykeji.top/gtyknltiio.html

JS:   process.env.HOME
来源：http://hz.zhijiandao.cn/gtxndmfutu.html

TS:   process.env.HOME
来源：http://hz.zhaomingkeji.xyz/gtaznffssv.html

Java: System.getenv("HOME")
来源：http://hz.aizwys.cn/gtnsrinnoz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cashguo.top/gtkmoksjkm.html

Ruby: ENV["HOME"]
来源：http://hz.quarkkingdee.top/gtndnatjks.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.0kj1m.cn/gtkflgncub.html

[M03] 执行外部命令
来源：http://hz.jiagoushi.top/gtzieodqwa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shuidangran.top/gtkylfjled.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.guowangkeji.top/gteyacltll.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenlongwang.top/gtokbzinvg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.0kj1m.cn/gtjabkalbc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.iojbl.cn/gtrmsczhja.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.gogol.net.cn/gtftnlzprr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.tian-w.cn/gtpimsudyj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhoulong.xyz/gtcztyspfh.html

[M04] 获取当前工作目录
来源：http://hz.aibaodan.cn/gtijdhoztk.html

Py:   os.getcwd()
来源：http://hz.aibaodan.cn/gtgyufacmr.html

PHP:  getcwd();
来源：http://hz.yj20258.top/gtubkhoayh.html

JS:   process.cwd()
来源：http://hz.feifeiyinyue.top/gtwhkeinoo.html

TS:   process.cwd()
来源：http://hz.gaohongyu789.top/gtahaprher.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.havefunace.top/gtseuqwzjc.html

Go:   os.Getwd()
来源：http://hz.sufxvd.cn/gtctbafhga.html

Ruby: Dir.pwd
来源：http://hz.gaohongyu789.top/gtoayoltaz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cdnleiting.top/gtnjgkdudv.html

[M05] 设置退出码
来源：http://hz.shanyushiyangtech.top/gtaxlbdflz.html

Py:   sys.exit(1)
来源：http://hz.xinyue.icu/gthpdmvihm.html

PHP:  exit(1);
来源：http://hz.cashguo.top/gttowzbcob.html

JS:   process.exit(1)
来源：http://hz.chenjidiqi.icu/gtusqbzful.html

TS:   process.exit(1)
来源：http://hz.chenzaomai.com/gtlflkznba.html

Java: System.exit(1)
来源：http://hz.jlsjyb.cn/gtnuvendua.html

Go:   os.Exit(1)
来源：http://hz.xuanzx.com/gtbpsaeutx.html

Ruby: exit 1
来源：http://hz.tanke756.top/gtievfdxru.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhiwuduotai.top/gthvpsfjpq.html

[M06] 向标准错误输出
来源：http://hz.smart0.xyz/gtlqvpsmkt.html

Py:   print("err", file=sys.stderr)
来源：http://hz.vqdsnc.cn/gtlpunksyi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.wangdashe.top/gtwfgqttml.html

JS:   console.error("err")
来源：http://hz.hammf.cn/gtvfersavp.html

TS:   console.error("err")
来源：http://hz.daxiang520.top/gtbxuareap.html

Java: System.err.println("err")
来源：http://hz.316326.xyz/gttezqnmfn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jiagoushi.top/gtoiedtrth.html

Ruby: warn "err"
来源：http://hz.mhx1999.top/gtpnvjgteo.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.sxryk.cn/gtizfrbfqi.html

[M07] 判断是否为主入口
来源：http://hz.vqdsnc.cn/gtjaldbvyi.html

Py:   if __name__ == "__main__":
来源：http://hz.guannengcc.top/gtdhrfvdjq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhongyouzk.top/gtubnqtwyg.html

JS:   require.main === module
来源：http://hz.hongshengwenyu.top/gtckbzioxi.html

TS:   require.main === module
来源：http://hz.pengpengdd.cyou/gtniotpqkx.html

Java: public static void main(String[] args)
来源：http://hz.zhixingplan.top/gtkurazufo.html

Go:   func main()
来源：http://hz.fzhhl.top/gtbmsclxbv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhijiandao.cn/gtamlfnjvx.html

C#:   static void Main(string[] args)
来源：http://hz.feifeiyinyue.top/gtzyxklsoe.html

[M08] 获取系统与运行时信息
来源：http://hz.cheryme.top/gtvxxjwpme.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yuxming.cn/gtqidoigmp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.meibo888.top/gthyaezdqr.html

JS:   process.platform;  process.version
来源：http://hz.shuidangran.top/gttzioylaj.html

TS:   process.platform;  process.version
来源：http://hz.guowangkeji.top/gtpnjtwfvr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhoulong.xyz/gttrqlrtga.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.kuanghao11.cn/gtbobradxy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jyoumei.cn/gtnmnzwplf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.smart0.xyz/gtapenuxse.html

================================================================================
来源：http://hz.yueranfly.top/gtuyspwtpq.html

N. 数据结构与算法
来源：http://hz.hnqzz.top/gtucgzskoo.html

================================================================================
来源：http://hz.zycfv.cn/gtlsczyjgd.html

[N01] 二分查找（有序数组）
来源：http://hz.jlsjyb.cn/gtfcmduigt.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gteylmrqbb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.wangdashe.top/gttbqlymzm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.guowangkeji.top/gtrmuorrek.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tian-w.cn/gtnivyuvxd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.0kj1m.cn/gtcpmsizai.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.haohaochexian.top/gtulhfplps.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ydjk.org.cn/gtxomniwci.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.dashuyun.cn/gtihftmted.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.daxiang520.top/gtkqvrnjmv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhengqikj.top/gtzmtlsmnu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.aizwys.cn/gtjjigdngf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yvedp.cn/gtgzflbrae.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aizwys.cn/gtixsdaoha.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xylfe.cn/gticxwwfzg.html

Go:   slices.Sort(arr)
来源：http://hz.tanke756.top/gtxyqsjeus.html

Ruby: arr.sort
来源：http://hz.c1oappe.top/gtlguclxnf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ydzc1.top/gtrkexvgqj.html

[N03] 快速排序（分治示例）
来源：http://hz.guowangkeji.top/gtufprkymf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jqgufenzy.top/gtodvbxnsn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jyoumei.cn/gtgqbbhavg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gotoacloud.top/gtcjocpgmz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gotoacloud.top/gtpsmvzlhg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shangyingyoupin.top/gtsulbaboh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shanyushiyangkeji.top/gtqkvzxofp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sweek.top/gtfpfsbdbx.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yj20258.top/gtetobiwup.html

[N04] 斐波那契数列
来源：http://hz.chenzaomai.com/gtncjdqubm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xuanzx.com/gthtyuxzch.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shanyushiyangkeji.top/gtwfekuwlx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aibaodan.cn/gtyqwhbqqr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhiwuduotai.top/gtbjocnbki.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jyoumei.cn/gtoyadmqje.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.fzhhl.top/gtmbsveddb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gaohongyu789.top/gteqivxmlz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xuetiantiany.cn/gtmhfegthi.html

[N05] 最大公约数
来源：http://hz.shuidangran.top/gtvasbnvvl.html

Py:   math.gcd(a, b)
来源：http://hz.xuetiantiany.cn/gtmughxybc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinghuilouyu.cn/gtkkowrupt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jyoumei.cn/gttfkecriv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.mhx1999.top/gtubmyrhdj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.snrcjt.cn/gtpzjvclvb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.meibo888.top/gtzycsdgtk.html

Ruby: a.gcd(b)
来源：http://hz.gogol.net.cn/gtmzljwglp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shangyingyoupin.top/gtusrqyaiu.html

[N06] 判断回文字符串
来源：http://hz.0kj1m.cn/gtcqgpmiia.html

Py:   s == s[::-1]
来源：http://hz.c1oappe.top/gtkuukxrrw.html

PHP:  $s === strrev($s);
来源：http://hz.sxryk.cn/gtyasoxmjo.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cheryme.top/gtvkkdgtga.html

TS:   s === [...s].reverse().join("")
来源：http://hz.chenjidiqi.icu/gtggbvtnnp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sufxvd.cn/gtpgiuygmt.html

Go:   // 双指针从两端比较
来源：http://hz.zycfv.cn/gtyfverkzc.html

Ruby: s == s.reverse
来源：http://hz.yj20258.top/gtoujwroqr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ydjk.org.cn/gtbcwbgybt.html

[N07] 两数之和（返回下标）
来源：http://hz.cdnleiting.top/gtubfrmphp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.tian-w.cn/gtkhwhdifq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xingfuxueyuan.xyz/gtxpbtvayf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.wangshuangyany.cn/gtxcdbrdef.html

TS:   // 手写 Map<string, number>
来源：http://hz.gzhubu.top/gtoblvuufi.html

Java: // 手写 HashMap
来源：http://hz.shzxlz.cn/gtglpiggpg.html

Go:   // 手写 map[int]int
来源：http://hz.vqdsnc.cn/gtrsuyzaxt.html

Ruby: // 手写 Hash
来源：http://hz.fzhhl.top/gtlagpuorg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hnxiangtu.top/gtmbxgrcnx.html

[N08] 生成全排列
来源：http://hz.xziqi.cn/gtoblmdliw.html

Py:   itertools.permutations(arr)
来源：http://hz.zhijiandao.cn/gthpjdmuir.html

PHP:  // 手写递归交换
来源：http://hz.cashguo.top/gtdvraqefq.html

JS:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtcmctezka.html

TS:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtvdkerzge.html

Java: // 手写回溯递归
来源：http://hz.chenlongwang.top/gtlcgzfpez.html

Go:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtdmjnldne.html

Ruby: arr.permutation.to_a
来源：http://hz.ybcxt.top/gtbmeicazr.html

C#:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtkwscmppg.html

[N09] 栈与队列
来源：http://hz.ybcxt.top/gtefuwiznp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.aizwys.cn/gtxyqwcbwb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ydjk.org.cn/gtyfhdxbhr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jqgfzy.top/gtdamembhw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.aibaodan.cn/gtitywdlqd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.svipenyu.cn/gtzocvecoh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhongyouzk.top/gtghkdotsb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.nanxinkj.top/gtqjmwrpzl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hfpthk.cn/gtnvwmydbl.html

[N10] 链表节点定义
来源：http://hz.guannengcc.top/gtzxzjpupa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.haohaochexian.top/gtwjkysidn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shanyushiyangtech.top/gtvrbvfdvn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gzhubu.top/gtgudlosva.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenjidiqi.icu/gtxydowrbl.html

Java: class Node { int v; Node next; }
来源：http://hz.ybcxt.top/gtctkqptal.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.wangshuangyany.cn/gttmbpqvvn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.guowangkeji.top/gtbplkzcrb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.52xcode.cn/gtqkkjguox.html

[N11] 二叉树中序遍历
来源：http://hz.iojbl.cn/gtkaqfgzrz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.c1oappe.top/gtkfpyxoeq.html

PHP:  // 手写递归函数
来源：http://hz.haohaochexian.top/gtczvosmix.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenzaomai.com/gtjgcrdhyx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jianghu66.top/gtllaiyaqe.html

Java: // 手写递归
来源：http://hz.dashuyun.cn/gtzyhtwqjg.html

Go:   // 手写递归
来源：http://hz.guannengcc.top/gtoyhytzdj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhiwuduotai.top/gtgvhywxeh.html

C#:   // 手写递归
来源：http://hz.ydzc1.top/gtbrvcmvqg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hongshengwenyu.top/gtrldsmizb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hnxiangtu.top/gtjpwculqf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.wangshuangyany.cn/gtoepjnmnc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zycfv.cn/gtkgolcrtj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hongshengwenyu.top/gtpifppnfl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pengpengdd.cyou/gtnpdigwru.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zdqjudy.top/gtwkmmgqbl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hammf.cn/gtylvgqfqk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgfzy.top/gtmmehwwmv.html

================================================================================
来源：http://hz.haohaochexian.top/gtmetcksgc.html

O. 并发与异步
来源：http://hz.nanxinkj.top/gtvhlekejy.html

================================================================================
来源：http://hz.zdqjudy.top/gtwpifyihj.html

[O01] 启动一个线程
来源：http://hz.aibaodan.cn/gttftifgeo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ybcxt.top/gtelwgwcom.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yuanzhike.top/gthohefpgt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.smart0.xyz/gtaybtflci.html

TS:   // 同 JS
来源：http://hz.52xcode.cn/gtrgbrwdit.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinyuanbaomall.cn/gttnqasvvi.html

Go:   go f()
来源：http://hz.shanyushiyangtech.top/gtpfxngruo.html

Ruby: Thread.new { f }
来源：http://hz.shuidangran.top/gtzqndbiew.html

C#:   Task.Run(() => F());
来源：http://hz.quarkkingdee.top/gtsfpxsmcd.html

[O02] 使用线程池
来源：http://hz.ehwqpu.com/gtvvlzuysz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhaomingkeji.xyz/gtgwfseiun.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.9152youxi.cn/gtbfprjbps.html

JS:   // worker_threads 线程池
来源：http://hz.pengpengdd.cyou/gtbzbttisp.html

TS:   // worker_threads 线程池
来源：http://hz.cheryme.top/gthtiluohh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yangfankeji.com/gthyszjyqa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.sweek.top/gtskvgyvte.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.tanke756.top/gtiiigrlgl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.chenzaomai.com/gtrlrbpnkb.html

[O03] 加锁保护共享数据
来源：http://hz.cdnleiting.top/gtcramgwio.html

Py:   with lock: shared += 1
来源：http://hz.yanxiufei.cn/gtjukteblg.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.vqdsnc.cn/gtergojwbl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.havefunace.top/gtlesqshmy.html

TS:   // 同 JS
来源：http://hz.ivvv.top/gtxjmklcqr.html

Java: synchronized (this) { shared++; }
来源：http://hz.jiagoushi.top/gtrbykhbgu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.smart0.xyz/gtmsxpvsku.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.haohaochexian.top/gtpgqhsded.html

C#:   lock (gate) { shared++; }
来源：http://hz.shzxlz.cn/gtbzqibynq.html

[O04] 定义异步函数并等待
来源：http://hz.pengpengdd.cyou/gtieavnlcy.html

Py:   async def f():⏎    await g()
来源：http://hz.hfpthk.cn/gttzvdjosp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.iojbl.cn/gtdireidcg.html

JS:   async function f() { await g(); }
来源：http://hz.hysaishi.cn/gtazimsssh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.andypj.xyz/gtmrpjlkrc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yanxiufei.cn/gtsugjabln.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shangyingyoupin.top/gtnfwfzqdx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xuetiantiany.cn/gtfhipfkad.html

C#:   async Task F() { await G(); }
来源：http://hz.jiagoushi.top/gtmewpholg.html

[O05] 并发执行并等待全部完成
来源：http://hz.dianchejie.cn/gtctezugii.html

Py:   asyncio.gather(*tasks)
来源：http://hz.mhx1999.top/gtfejwstym.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cucudq.cn/gtlwcaagrr.html

JS:   await Promise.all(tasks)
来源：http://hz.nanxuanxn.top/gtldnwynqw.html

TS:   await Promise.all(tasks)
来源：http://hz.sweek.top/gtwyfgthfk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.nanxuanxn.top/gtfzwujdns.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hongshengwenyu.top/gttzskachb.html

Ruby: threads.map(&:join)
来源：http://hz.zhoulong.xyz/gtfjhbyrqf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.aizwys.cn/gtwtkfvzta.html

[O06] 使用进程池
来源：http://hz.hongshengwenyu.top/gtozznpoky.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.sxryk.cn/gtguxzuwmy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jyoumei.cn/gtgkjyntwb.html

JS:   // child_process / cluster 模块
来源：http://hz.dianchejie.cn/gtxecneyti.html

TS:   // child_process / cluster 模块
来源：http://hz.zhixingplan.top/gtoqhnwxer.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.shzxlz.cn/gtfqblevle.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.smart0.xyz/gtvebvevps.html

Ruby: // fork 块
来源：http://hz.hnxiangtu.top/gtgeewlrzn.html

C#:   Parallel.For
来源：http://hz.gaohongyu789.top/gtwvszatpk.html

================================================================================
来源：http://hz.birdmap.top/gtlcgsnjdt.html

P. 常用工具函数
来源：http://hz.mhx1999.top/gtqxctqbsq.html

================================================================================
来源：http://hz.shzxlz.cn/gtiaptaarl.html

[P01] 生成 UUID
来源：http://hz.daria6918.cn/gtqrpjtiwi.html

Py:   str(uuid.uuid4())
来源：http://hz.gotoacloud.top/gtfajcxdqe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sysykeji.top/gtwagqjzae.html

JS:   crypto.randomUUID()
来源：http://hz.guannengcc.top/gtktaimlii.html

TS:   crypto.randomUUID()
来源：http://hz.hongshengwenyu.top/gtidjkkyjk.html

Java: UUID.randomUUID().toString()
来源：http://hz.dianchejie.cn/gtpdykgfgl.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cheryme.top/gtyjynfwax.html

Ruby: SecureRandom.uuid
来源：http://hz.gotoacloud.top/gttjmxfpsn.html


<!-- 参考信息 -->