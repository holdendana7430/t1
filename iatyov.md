代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhiwuduotai.top/gtagecxsas.html

[L04] 设置超时
来源：http://hz.vqdsnc.cn/gtgqxnkmoc.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xylfe.cn/gtbbopyifs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yangfankeji.com/gtqkrociyc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hysaishi.cn/gtrgajowzk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.snrcjt.cn/gtwwgkmtjn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cheryme.top/gtfrytvioo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ydzc1.top/gtsuragugw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sweek.top/gtfobxbfbp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shanyushiyangtech.top/gtlvvhzetv.html

[L05] 上传文件（multipart）
来源：http://hz.guowangkeji.top/gteadbtziy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.svipenyu.cn/gtyxutpami.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.aizwys.cn/gtlekwslqa.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hysaishi.cn/gtlktuxitl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jyoumei.cn/gtcrzlrsog.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hongshengwenyu.top/gtxpqwrlyl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nanxinkj.top/gtrrizdlzm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.meibo888.top/gtuccyezic.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinghuilouyu.cn/gtguifnmnf.html

[L06] 解析响应为 JSON
来源：http://hz.meibo888.top/gtozchmcpf.html

Py:   resp.json()
来源：http://hz.zhaomingkeji.xyz/gtrngcytze.html

PHP:  json_decode($body, true);
来源：http://hz.tanke756.top/gtjgtjjloa.html

JS:   await resp.json()
来源：http://hz.gogol.net.cn/gtfkflxqzf.html

TS:   await resp.json()
来源：http://hz.jqgfzy.top/gtupiatdok.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.dianchejie.cn/gtbsecknwa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hnxiangtu.top/gtcajaxhlz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yanxiufei.cn/gtwqnfeawr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.316326.xyz/gtcignsemn.html

[L07] 处理 HTTP 状态码
来源：http://hz.birdmap.top/gtcibqrhyr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sweek.top/gtgyxistsq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinyuanbaomall.cn/gtciohuwdv.html

JS:   resp.ok;  resp.status
来源：http://hz.tanke756.top/gtxfxenxsa.html

TS:   resp.ok;  resp.status
来源：http://hz.hysaishi.cn/gtbvglaxwr.html

Java: resp.statusCode()
来源：http://hz.zhiwuduotai.top/gtmwupnvhc.html

Go:   resp.StatusCode
来源：http://hz.tianlin.xyz/gtcifltjgj.html

Ruby: resp.code.to_i
来源：http://hz.guowangkeji.top/gtvulrdckc.html

C#:   (int)resp.StatusCode
来源：http://hz.nanxinkj.top/gtdxrdnwkd.html

[L08] 并发请求多个地址
来源：http://hz.bjfxy.top/gtzfwgvizm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zdqjudy.top/gtacwjrvuz.html

PHP:  curl_multi_init() 系列
来源：http://hz.pycfn.com/gtbbqykuao.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhijiandao.cn/gtlsteyqsy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.birdmap.top/gtzyqtrlwl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ywan-chungtsiang.top/gtotokachb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hnxiangtu.top/gtdgpnwfof.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.sxryk.cn/gtjdebyfvk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhixingplan.top/gtssgsjwkr.html

================================================================================
来源：http://hz.zhoulong.xyz/gtndtrlzaq.html

M. 命令行 / 进程 / 环境
来源：http://hz.haohaochexian.top/gtfjakpxst.html

================================================================================
来源：http://hz.xuanzx.com/gtqstphoyk.html

[M01] 读取命令行参数
来源：http://hz.nanxinkj.top/gtpejddvrt.html

Py:   sys.argv[1:]
来源：http://hz.yanxiufei.cn/gtfdeerotl.html

PHP:  $argv;  $argc;
来源：http://hz.hnxiangtu.top/gtzwcxdpmd.html

JS:   process.argv.slice(2)
来源：http://hz.zhoulong.xyz/gtxbiaxuxs.html

TS:   process.argv.slice(2)
来源：http://hz.cdnleiting.top/gtzzgbeqpz.html

Java: args 数组（main 方法参数）
来源：http://hz.jianghu66.top/gttqtozqhg.html

Go:   os.Args[1:]
来源：http://hz.jqgufenzy.top/gtkbzatrba.html

Ruby: ARGV
来源：http://hz.haohaochexian.top/gtlxqgjlpf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yvedp.cn/gtqmwpzxtu.html

[M02] 读取环境变量
来源：http://hz.0kj1m.cn/gthdlqvymr.html

Py:   os.environ.get("HOME")
来源：http://hz.hywenlv.cn/gtitwlzxdi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shanyushiyangkeji.top/gtzhbkgehn.html

JS:   process.env.HOME
来源：http://hz.shangyingyoupin.top/gtmrgmysfq.html

TS:   process.env.HOME
来源：http://hz.jinqigufen.top/gtbyonusuf.html

Java: System.getenv("HOME")
来源：http://hz.zhaomingkeji.xyz/gtvuuxfamd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.tianlin.xyz/gtkseeouri.html

Ruby: ENV["HOME"]
来源：http://hz.hongshengwenyu.top/gtlgnlyfde.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cheryme.top/gtsgggwgkt.html

[M03] 执行外部命令
来源：http://hz.wangshuangyany.cn/gtnzlumwuj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jyoumei.cn/gtqmcoqxne.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yueranfly.top/gtjqlcoxcn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shuidangran.top/gtmkqxnbyn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangshuangyany.cn/gtcobmzclh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj20258.top/gtxnjzekpb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhengqikj.top/gtprtydpqm.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yangfankeji.com/gtpselprtn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shuidangran.top/gtbvscznlt.html

[M04] 获取当前工作目录
来源：http://hz.bjfxy.top/gtlgybaqjv.html

Py:   os.getcwd()
来源：http://hz.hfpthk.cn/gtiygosaiz.html

PHP:  getcwd();
来源：http://hz.zhaomingkeji.xyz/gtnanrtnfd.html

JS:   process.cwd()
来源：http://hz.cashguo.top/gteohwlvbw.html

TS:   process.cwd()
来源：http://hz.hnxiangtu.top/gtmpjgipqo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cashguo.top/gtqxlmpkrz.html

Go:   os.Getwd()
来源：http://hz.wangdashe.top/gtcckmatzl.html

Ruby: Dir.pwd
来源：http://hz.hnqzz.top/gtjcxbzlsb.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ivvv.top/gtemyyefpl.html

[M05] 设置退出码
来源：http://hz.yuanzhike.top/gtzabtkmqq.html

Py:   sys.exit(1)
来源：http://hz.52xcode.cn/gtlksbjqrw.html

PHP:  exit(1);
来源：http://hz.wangdashe.top/gtsxvpzevw.html

JS:   process.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtniqkubdt.html

TS:   process.exit(1)
来源：http://hz.svipenyu.cn/gtdkiooges.html

Java: System.exit(1)
来源：http://hz.ydzc1.top/gtyahjkvxt.html

Go:   os.Exit(1)
来源：http://hz.shanyushiyangkeji.top/gtfsvpbeiu.html

Ruby: exit 1
来源：http://hz.bjfxy.top/gtuagsdbal.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nanxuanxn.top/gtazykxamb.html

[M06] 向标准错误输出
来源：http://hz.zhijiandao.cn/gtumprsoen.html

Py:   print("err", file=sys.stderr)
来源：http://hz.mhx1999.top/gtcukcunja.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.iojbl.cn/gtgoyubahz.html

JS:   console.error("err")
来源：http://hz.ywan-chungtsiang.top/gtookkajsk.html

TS:   console.error("err")
来源：http://hz.nanxinkj.top/gtodtqdroi.html

Java: System.err.println("err")
来源：http://hz.aibaodan.cn/gtirwhcwwy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zdqjudy.top/gtwevfdsvw.html

Ruby: warn "err"
来源：http://hz.quarkkingdee.top/gtqwpicnwv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jlsjyb.cn/gtybipvsry.html

[M07] 判断是否为主入口
来源：http://hz.cdnleiting.top/gttsxcolxc.html

Py:   if __name__ == "__main__":
来源：http://hz.zhaomingkeji.xyz/gtpnyeydqd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zycfv.cn/gtysyxlpni.html

JS:   require.main === module
来源：http://hz.yongpay.top/gtcrwzrpxb.html

TS:   require.main === module
来源：http://hz.jlsjyb.cn/gtakdqstne.html

Java: public static void main(String[] args)
来源：http://hz.ybcxt.top/gtpgpyaeji.html

Go:   func main()
来源：http://hz.gaohongyu789.top/gtaosdttiy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ehwqpu.com/gtbialtoue.html

C#:   static void Main(string[] args)
来源：http://hz.hywenlv.cn/gtymerdhsf.html

[M08] 获取系统与运行时信息
来源：http://hz.zhixingplan.top/gtdatlkaej.html

Py:   platform.system();  platform.python_version()
来源：http://hz.pengpengdd.cyou/gthkoadtcr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yongpay.top/gtydrklnlz.html

JS:   process.platform;  process.version
来源：http://hz.dashuyun.cn/gtvspwwpjg.html

TS:   process.platform;  process.version
来源：http://hz.yongpay.top/gtyjqiawek.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.nanxuanxn.top/gthmizspzb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xylfe.cn/gtcawbhonw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.wangdashe.top/gtxavlyvwk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.mhx1999.top/gtgqdtaydg.html

================================================================================
来源：http://hz.xinyue.icu/gtpjcemouo.html

N. 数据结构与算法
来源：http://hz.zhaomingkeji.xyz/gtpzjikboe.html

================================================================================
来源：http://hz.hywenlv.cn/gttsojtihh.html

[N01] 二分查找（有序数组）
来源：http://hz.hywenlv.cn/gtgyblrhjs.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sweek.top/gtnxgwxxra.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cdnleiting.top/gtiwnjktzo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dianchejie.cn/gtixppobfw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ybcxt.top/gtsiuuhixf.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hnxiangtu.top/gtngjgratz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yvedp.cn/gtwwkyrces.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shanyushiyangtech.top/gtzbydwohu.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.fengsongda.top/gtnkaadaui.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhiwuduotai.top/gteqrcsslh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.0kj1m.cn/gtnvlwfdqo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hywenlv.cn/gtfjjjovpj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sysykeji.top/gtrrjgwlfo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.mhx1999.top/gtzzaqzohd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hfpthk.cn/gtviuwvzqb.html

Go:   slices.Sort(arr)
来源：http://hz.shanyushiyangkeji.top/gtpsnvtzry.html

Ruby: arr.sort
来源：http://hz.yanxiufei.cn/gtrdzizwfk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.fengsongda.top/gtfwfrxvil.html

[N03] 快速排序（分治示例）
来源：http://hz.ehwqpu.com/gtmipwjnbw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhixingplan.top/gtxnaxsbik.html

PHP:  // 递归实现，或用 usort
来源：http://hz.c1oappe.top/gtfuflfaym.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aibaodan.cn/gtgodxqnds.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yanxiufei.cn/gtcmmhzcmh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinqigufen.top/gtymgsxjiz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yuxming.cn/gtuhfldyzc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jinqigfzy.top/gtqnmdkzaw.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.dashuyun.cn/gtshstrglf.html

[N04] 斐波那契数列
来源：http://hz.guannengcc.top/gtmmjjvacx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.c1oappe.top/gtragxkfng.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.wangdashe.top/gtxzaczgdm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cucudq.cn/gtxwegxbvs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.havefunace.top/gteotaezrk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hysaishi.cn/gtwadoiwvb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gotoacloud.top/gtkwrvpaxx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ybcxt.top/gtfcletxnb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.smart0.xyz/gtnvyfdgzv.html

[N05] 最大公约数
来源：http://hz.jinghuilouyu.cn/gtufjxiona.html

Py:   math.gcd(a, b)
来源：http://hz.chenzaomai.com/gtyvaycwne.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.bjfxy.top/gtehmcieet.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhaomingkeji.xyz/gtuxuziwmc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj20258.top/gtkkiejcnb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.havefunace.top/gtnuxjkzop.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhijiandao.cn/gtsqcjusqd.html

Ruby: a.gcd(b)
来源：http://hz.daxiang520.top/gteodohdzp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cheryme.top/gttdygjhkr.html

[N06] 判断回文字符串
来源：http://hz.ydjk.org.cn/gthdxydwrc.html

Py:   s == s[::-1]
来源：http://hz.hysaishi.cn/gtgxifbaqn.html

PHP:  $s === strrev($s);
来源：http://hz.aizwys.cn/gtfeglwfmm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ivvv.top/gtrsfcqxek.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtmeduqqnr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.chenjidiqi.icu/gtailbovjp.html

Go:   // 双指针从两端比较
来源：http://hz.hongshengwenyu.top/gtfthzyvhj.html

Ruby: s == s.reverse
来源：http://hz.nwbrower.top/gtrodxglde.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tianlin.xyz/gtdbzewwnt.html

[N07] 两数之和（返回下标）
来源：http://hz.mhx1999.top/gtjegiopva.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.sxryk.cn/gtmspstweb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shanyushiyangkeji.top/gtokaotdqu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.pengpengdd.cyou/gtkoasclhi.html

TS:   // 手写 Map<string, number>
来源：http://hz.c1oappe.top/gtyrsvtzod.html

Java: // 手写 HashMap
来源：http://hz.hfpthk.cn/gtepzowcom.html

Go:   // 手写 map[int]int
来源：http://hz.daria6918.cn/gtxywtphqg.html

Ruby: // 手写 Hash
来源：http://hz.gaohongyu789.top/gtfvohkosi.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jiagoushi.top/gtwbvxkcaq.html

[N08] 生成全排列
来源：http://hz.jinqigfzy.top/gtuqlbxzpm.html

Py:   itertools.permutations(arr)
来源：http://hz.daxiang520.top/gtwabhzymo.html

PHP:  // 手写递归交换
来源：http://hz.shuidangran.top/gttutmamvt.html

JS:   // 手写回溯递归
来源：http://hz.daxiang520.top/gtjwumhqwc.html

TS:   // 手写回溯递归
来源：http://hz.zycfv.cn/gtdfmhquzm.html

Java: // 手写回溯递归
来源：http://hz.yj202588.top/gtknfxcvpm.html

Go:   // 手写回溯递归
来源：http://hz.ydzc1.top/gtjqwmldkp.html

Ruby: arr.permutation.to_a
来源：http://hz.jqgufenzy.top/gtwqzaeuwm.html

C#:   // 手写回溯递归
来源：http://hz.mhx1999.top/gtrtpjiydv.html

[N09] 栈与队列
来源：http://hz.aizwys.cn/gtnbegfggs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zycfv.cn/gtpyqubzjf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xingfuxueyuan.xyz/gtwvhpnmaj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.vqdsnc.cn/gtpnxzltga.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.pycfn.com/gtocnffyzk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hammf.cn/gtlldpfpww.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.pycfn.com/gtwjkkbpdh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yj202588.top/gtiylseqys.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.svipenyu.cn/gtziwbkjei.html

[N10] 链表节点定义
来源：http://hz.gogol.net.cn/gtcecgpboh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xuetiantiany.cn/gtvzxcmjzv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.316326.xyz/gtihrsosfs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.shuidangran.top/gtpsranuhb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xuetiantiany.cn/gtndtrhgyi.html

Java: class Node { int v; Node next; }
来源：http://hz.quarkkingdee.top/gtctlzzfrp.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.chenlongwang.top/gtwoohqmfg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.dashuyun.cn/gtmktnodsb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.redwolf501.top/gttirhnhuc.html

[N11] 二叉树中序遍历
来源：http://hz.hywenlv.cn/gtktizcuas.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cqqwz.cn/gtlznfzfsw.html

PHP:  // 手写递归函数
来源：http://hz.zhongyouzk.top/gtqfnzzhbk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhijiandao.cn/gtkzsuzzea.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gogol.net.cn/gtlykmbdbv.html

Java: // 手写递归
来源：http://hz.chenjidiqi.icu/gtnenkgqbp.html

Go:   // 手写递归
来源：http://hz.fengsongda.top/gthguvojrd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.iojbl.cn/gtudplgbzg.html

C#:   // 手写递归
来源：http://hz.guowangkeji.top/gtoltteqab.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jianghu66.top/gttzfqlcsm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.9152youxi.cn/gtasiuiixc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yangfankeji.com/gtqgceteno.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yangfankeji.com/gtfnerwjnc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinghuilouyu.cn/gtjqqwtetp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.mhx1999.top/gtbgbhxftm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.gotoacloud.top/gtosjwfkxe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.dianchejie.cn/gtotkzuujn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigufen.top/gtdeikfutw.html

================================================================================
来源：http://hz.quarkkingdee.top/gtilzknubu.html

O. 并发与异步
来源：http://hz.yangfankeji.com/gtkowunvlu.html

================================================================================
来源：http://hz.dashuyun.cn/gttvpxiilh.html

[O01] 启动一个线程
来源：http://hz.feifeiyinyue.top/gtmeswsakr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.feifeiyinyue.top/gtuhwagqly.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.wangshuangyany.cn/gtbshlcudg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.daria6918.cn/gtoledhepf.html

TS:   // 同 JS
来源：http://hz.52xcode.cn/gtolgzgqny.html

Java: new Thread(() -> f()).start()
来源：http://hz.daria6918.cn/gthppxldix.html

Go:   go f()
来源：http://hz.zhongyouzk.top/gtnztwlcol.html

Ruby: Thread.new { f }
来源：http://hz.xinyue.icu/gtzdfgrpjp.html

C#:   Task.Run(() => F());
来源：http://hz.52xcode.cn/gtsuuuwhoo.html

[O02] 使用线程池
来源：http://hz.jinqigfzy.top/gtzwmexqax.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xinyue.icu/gteqhqsmgd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cashguo.top/gtuzjyvpse.html

JS:   // worker_threads 线程池
来源：http://hz.ydzc1.top/gtcbfjzsiv.html

TS:   // worker_threads 线程池
来源：http://hz.daria6918.cn/gtkakwivso.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.52xcode.cn/gtvrkretvz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xinyue.icu/gtsgmtklkf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ywan-chungtsiang.top/gtrjpnuwgb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.fengsongda.top/gtotaxbgcl.html

[O03] 加锁保护共享数据
来源：http://hz.cqqwz.cn/gtclyjrwus.html

Py:   with lock: shared += 1
来源：http://hz.yueranfly.top/gtmqxusczx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yangfankeji.com/gtfwehhjdn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.snrcjt.cn/gtozpoymor.html

TS:   // 同 JS
来源：http://hz.dashuyun.cn/gtxhdyjddm.html

Java: synchronized (this) { shared++; }
来源：http://hz.shuidangran.top/gteugkmqsr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.chenjidiqi.icu/gtfhwapsvw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.bjfxy.top/gtchqduhdw.html

C#:   lock (gate) { shared++; }
来源：http://hz.zycfv.cn/gtvrkjbbos.html

[O04] 定义异步函数并等待
来源：http://hz.jlsjyb.cn/gtrqphdpst.html

Py:   async def f():⏎    await g()
来源：http://hz.tianlin.xyz/gtfvbfoohp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gaohongyu789.top/gtdenkrbkz.html

JS:   async function f() { await g(); }
来源：http://hz.daria6918.cn/gtvyxhdwky.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.pengpengdd.cyou/gtpjgzfhxf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gotoacloud.top/gtaumdpolg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xingfuxueyuan.xyz/gttzgagoxz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xinyue.icu/gtkiugkwor.html

C#:   async Task F() { await G(); }
来源：http://hz.daxiang520.top/gtqdyzynxt.html

[O05] 并发执行并等待全部完成
来源：http://hz.yuanzhike.top/gtafavnygj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhongyouzk.top/gtnfkyooms.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.nwbrower.top/gtlslbwesf.html

JS:   await Promise.all(tasks)
来源：http://hz.cashguo.top/gtielbdqlp.html

TS:   await Promise.all(tasks)
来源：http://hz.shanyushiyangtech.top/gtwxncuzjk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.sufxvd.cn/gtmexthfut.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sweek.top/gtlhzbcsmt.html

Ruby: threads.map(&:join)
来源：http://hz.aibaodan.cn/gtluqhdmvm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shzxlz.cn/gtampdkipf.html

[O06] 使用进程池
来源：http://hz.cdnleiting.top/gtbuuoagvh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hywenlv.cn/gtytoohxvb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhoulong.xyz/gtiopywshw.html

JS:   // child_process / cluster 模块
来源：http://hz.cdnleiting.top/gtzaoypkdv.html

TS:   // child_process / cluster 模块
来源：http://hz.cucudq.cn/gtytkijhxs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinqigufen.top/gtimharxyt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ydjk.org.cn/gtejpipiop.html

Ruby: // fork 块
来源：http://hz.shanyushiyangkeji.top/gtzuojsupr.html

C#:   Parallel.For
来源：http://hz.zdqjudy.top/gtxgsbbmrh.html

================================================================================
来源：http://hz.chenzaomai.com/gtewizismh.html

P. 常用工具函数
来源：http://hz.daxiang520.top/gtwmoshzwx.html

================================================================================
来源：http://hz.xinyue.icu/gthekzmncy.html

[P01] 生成 UUID
来源：http://hz.jianghu66.top/gthxohjbvb.html

Py:   str(uuid.uuid4())
来源：http://hz.cheryme.top/gtkqdykyhh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yuanzhike.top/gtyieusalx.html

JS:   crypto.randomUUID()
来源：http://hz.hnxiangtu.top/gtlhwnveob.html

TS:   crypto.randomUUID()
来源：http://hz.zhongyouzk.top/gttbadmzdd.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhaomingkeji.xyz/gtswkriink.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ywan-chungtsiang.top/gttrqixmcu.html

Ruby: SecureRandom.uuid
来源：http://hz.cdnleiting.top/gttilqxapr.html


<!-- 参考信息 -->