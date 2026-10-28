代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.pengpengdd.cyou/gtufzyjnlp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sxryk.cn/gtwdzqmbnx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xinyue.icu/gtgpvzmets.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sweek.top/gtvzwljxgt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhoulong.xyz/gtzaikdvny.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.wangshuangyany.cn/gtuodhsmvv.html

[L05] 上传文件（multipart）
来源：http://hz.yj20258.top/gttqpsuscq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.chenlongwang.top/gtbaliszet.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shuidangran.top/gtskjivkwn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xuanzx.com/gtcevtkgqu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj202588.top/gtjgxqknkf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shangyingyoupin.top/gtxocxbmvc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.52xcode.cn/gtoeeugpfp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shuidangran.top/gtbrjmczmb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.havefunace.top/gtxxviinkg.html

[L06] 解析响应为 JSON
来源：http://hz.shzxlz.cn/gtgdvzivxl.html

Py:   resp.json()
来源：http://hz.nanxuanxn.top/gtgmpnzxan.html

PHP:  json_decode($body, true);
来源：http://hz.redwolf501.top/gttnefaodq.html

JS:   await resp.json()
来源：http://hz.yanxiufei.cn/gtkfrzpzsi.html

TS:   await resp.json()
来源：http://hz.jlsjyb.cn/gtkahzaklj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hnqzz.top/gtlywzzepk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yj20258.top/gtojudbbpm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhixingplan.top/gtxbqohkah.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ydjk.org.cn/gtbuyowsql.html

[L07] 处理 HTTP 状态码
来源：http://hz.zycfv.cn/gtkyzcttdf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenzaomai.com/gtcubeghxy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ydzc1.top/gtrfnjnutz.html

JS:   resp.ok;  resp.status
来源：http://hz.dianchejie.cn/gtrlnieofz.html

TS:   resp.ok;  resp.status
来源：http://hz.hammf.cn/gtbzosdysy.html

Java: resp.statusCode()
来源：http://hz.guannengcc.top/gtozvhomiy.html

Go:   resp.StatusCode
来源：http://hz.tanke756.top/gtmfhxbfjq.html

Ruby: resp.code.to_i
来源：http://hz.jyoumei.cn/gtcvyiuuyd.html

C#:   (int)resp.StatusCode
来源：http://hz.nanxinkj.top/gtylnnygii.html

[L08] 并发请求多个地址
来源：http://hz.yueranfly.top/gtwuntxnax.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yueranfly.top/gtydvgjznk.html

PHP:  curl_multi_init() 系列
来源：http://hz.0kj1m.cn/gtzrsynivx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhongyouzk.top/gtsmuqsogc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shzxlz.cn/gtwgipsiqp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yueranfly.top/gtrzchrndp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tanke756.top/gtawjsuokv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.chenzaomai.com/gtglliwvqg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yueranfly.top/gtjoaodeym.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtwobegssd.html

M. 命令行 / 进程 / 环境
来源：http://hz.sweek.top/gtmmwornkv.html

================================================================================
来源：http://hz.svipenyu.cn/gtyehieytc.html

[M01] 读取命令行参数
来源：http://hz.cdnleiting.top/gtcejcvlch.html

Py:   sys.argv[1:]
来源：http://hz.zhongyouzk.top/gthekhatli.html

PHP:  $argv;  $argc;
来源：http://hz.nanxuanxn.top/gtuiusqgon.html

JS:   process.argv.slice(2)
来源：http://hz.ppjwa.cn/gtaazwnzdv.html

TS:   process.argv.slice(2)
来源：http://hz.ydjk.org.cn/gtxoipprvg.html

Java: args 数组（main 方法参数）
来源：http://hz.gogol.net.cn/gtgnulxuer.html

Go:   os.Args[1:]
来源：http://hz.jiagoushi.top/gtdutogrqp.html

Ruby: ARGV
来源：http://hz.aibaodan.cn/gtuvnkffur.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yueranfly.top/gtzlhasudq.html

[M02] 读取环境变量
来源：http://hz.ppjwa.cn/gtmtekyjwg.html

Py:   os.environ.get("HOME")
来源：http://hz.cashguo.top/gtnfnlfuuv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhiwuduotai.top/gtaaeaqqpm.html

JS:   process.env.HOME
来源：http://hz.cucudq.cn/gtporfhemo.html

TS:   process.env.HOME
来源：http://hz.sweek.top/gtyezmcgsf.html

Java: System.getenv("HOME")
来源：http://hz.0kj1m.cn/gtnxcnoawo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.0kj1m.cn/gtxnbpakrt.html

Ruby: ENV["HOME"]
来源：http://hz.tian-w.cn/gtbgexgfzs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhoulong.xyz/gtutulqcyo.html

[M03] 执行外部命令
来源：http://hz.sxryk.cn/gtnlclkelk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.birdmap.top/gtegpnpxrw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xinyue.icu/gtopgzcmrd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xziqi.cn/gtpdechjze.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.sxryk.cn/gtbsyglulb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.chenlongwang.top/gttaiaocky.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hfpthk.cn/gtorjtimiz.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.guannengcc.top/gtqgrfhnfu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yj20258888.top/gtlisvlkbc.html

[M04] 获取当前工作目录
来源：http://hz.yangfankeji.com/gtbskfluwa.html

Py:   os.getcwd()
来源：http://hz.yangfankeji.com/gtsfenkrsg.html

PHP:  getcwd();
来源：http://hz.tianlin.xyz/gtuuvlpebr.html

JS:   process.cwd()
来源：http://hz.cashguo.top/gtnrmuoski.html

TS:   process.cwd()
来源：http://hz.shanyushiyangtech.top/gtbudkchrs.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.316326.xyz/gtqnplheec.html

Go:   os.Getwd()
来源：http://hz.zycfv.cn/gtojrrsebx.html

Ruby: Dir.pwd
来源：http://hz.nwbrower.top/gtltyjieow.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.feifeiyinyue.top/gtjdqubvkk.html

[M05] 设置退出码
来源：http://hz.jinqigfzy.top/gttyeyglwm.html

Py:   sys.exit(1)
来源：http://hz.yongpay.top/gtbgxlbqoa.html

PHP:  exit(1);
来源：http://hz.sxryk.cn/gtdnecvevk.html

JS:   process.exit(1)
来源：http://hz.yuanzhike.top/gtqfeuzygy.html

TS:   process.exit(1)
来源：http://hz.yj202588.top/gtjyzhypww.html

Java: System.exit(1)
来源：http://hz.yanxiufei.cn/gtikfqetpk.html

Go:   os.Exit(1)
来源：http://hz.ydzc1.top/gtvdagacjc.html

Ruby: exit 1
来源：http://hz.aizwys.cn/gtwzbzubqh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhengqikj.top/gtjlsyrmzf.html

[M06] 向标准错误输出
来源：http://hz.316326.xyz/gtfutrelnz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yonumen.top/gtqcklawnf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.52xcode.cn/gttmogueef.html

JS:   console.error("err")
来源：http://hz.ywan-chungtsiang.top/gtcwdawkyg.html

TS:   console.error("err")
来源：http://hz.xylfe.cn/gtfxkrikxx.html

Java: System.err.println("err")
来源：http://hz.yj20258888.top/gthxtjbykt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhijiandao.cn/gthwqhihpi.html

Ruby: warn "err"
来源：http://hz.gzhubu.top/gtcledxfae.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.iojbl.cn/gtohrdkybg.html

[M07] 判断是否为主入口
来源：http://hz.xziqi.cn/gtiffisatc.html

Py:   if __name__ == "__main__":
来源：http://hz.guowangkeji.top/gtddjxrtdi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jianghu66.top/gtzufqwwqv.html

JS:   require.main === module
来源：http://hz.0kj1m.cn/gtrzwdhfuc.html

TS:   require.main === module
来源：http://hz.aibaodan.cn/gtwyewhbte.html

Java: public static void main(String[] args)
来源：http://hz.yangfankeji.com/gtkpfntrui.html

Go:   func main()
来源：http://hz.svipenyu.cn/gttgdywosp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.quarkkingdee.top/gtfjokhhwz.html

C#:   static void Main(string[] args)
来源：http://hz.andypj.xyz/gtaxhalmov.html

[M08] 获取系统与运行时信息
来源：http://hz.daria6918.cn/gtuzpffshh.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jlsjyb.cn/gtwwccyjac.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.316326.xyz/gtzyeqgiyr.html

JS:   process.platform;  process.version
来源：http://hz.jinghuilouyu.cn/gtbkacqgkv.html

TS:   process.platform;  process.version
来源：http://hz.316326.xyz/gtfwlteacu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinqigufen.top/gtmzlgftpm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhiwuduotai.top/gtzyeqjkhg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shanyushiyangkeji.top/gtmicxddhu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hysaishi.cn/gtgatbupfa.html

================================================================================
来源：http://hz.yonumen.top/gtqjgxmynu.html

N. 数据结构与算法
来源：http://hz.feifeiyinyue.top/gtwgtvxcyu.html

================================================================================
来源：http://hz.aizwys.cn/gtcvaylbwi.html

[N01] 二分查找（有序数组）
来源：http://hz.hysaishi.cn/gtsiuahhum.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhixingplan.top/gtznzhhtpd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hywenlv.cn/gtpxoooeou.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jiagoushi.top/gtfeurkisc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shanyushiyangkeji.top/gtnpymwazw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ehwqpu.com/gtpfwexwsu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hongshengwenyu.top/gtjdkmdvwc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.kuanghao11.cn/gtxbhnzzqn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cashguo.top/gtnutwcxjn.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yangfankeji.com/gtamvipuah.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.meibo888.top/gtfypklnbi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.fengsongda.top/gtrogdhbxq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shuidangran.top/gtswcjleik.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuanzhike.top/gteajrjstv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.mhx1999.top/gttdpookoo.html

Go:   slices.Sort(arr)
来源：http://hz.shzxlz.cn/gthqbhobbc.html

Ruby: arr.sort
来源：http://hz.xuanzx.com/gtrxsnxfhj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jlsjyb.cn/gtewvztnsq.html

[N03] 快速排序（分治示例）
来源：http://hz.pycfn.com/gtyudshucg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gogol.net.cn/gthnaqpqex.html

PHP:  // 递归实现，或用 usort
来源：http://hz.52xcode.cn/gtwpiddrac.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sxryk.cn/gtyyvsagtw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sysykeji.top/gtanenpqxe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.nanxinkj.top/gtsutfdoms.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.pengpengdd.cyou/gtsfpcoxrz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sxryk.cn/gtuqqoarka.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yuxming.cn/gtspajwiqo.html

[N04] 斐波那契数列
来源：http://hz.yuxming.cn/gtilochowc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangkeji.top/gtvzncjzxt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tanke756.top/gthqqldmrc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nwbrower.top/gtkergceiu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxuanxn.top/gtmnsdbpeh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.tianlin.xyz/gtejpkuytj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yj20258888.top/gtrdzhgiai.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.feifeiyinyue.top/gtnyyrirwf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hongshengwenyu.top/gtipkneeuv.html

[N05] 最大公约数
来源：http://hz.jyoumei.cn/gtqougvkry.html

Py:   math.gcd(a, b)
来源：http://hz.nanxinkj.top/gtvsanctka.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yonumen.top/gtwwglxcmk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.bjfxy.top/gtzezbmgbj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xylfe.cn/gtsaetdgym.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.meibo888.top/gtfnsptiew.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.pengpengdd.cyou/gtmqcvqhlq.html

Ruby: a.gcd(b)
来源：http://hz.xingfuxueyuan.xyz/gtxtqqcsap.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinqigufen.top/gtkmpxioiu.html

[N06] 判断回文字符串
来源：http://hz.gotoacloud.top/gtovkjmlsb.html

Py:   s == s[::-1]
来源：http://hz.shanyushiyangkeji.top/gttqylihcq.html

PHP:  $s === strrev($s);
来源：http://hz.jinyuanbaomall.cn/gtyoyejsye.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtzhsxhfxx.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtjegwvkaa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.52xcode.cn/gtehgdwjmh.html

Go:   // 双指针从两端比较
来源：http://hz.fengsongda.top/gtyebsazeq.html

Ruby: s == s.reverse
来源：http://hz.jinqigufen.top/gtlvqmomvx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinghuilouyu.cn/gtxbetlwsn.html

[N07] 两数之和（返回下标）
来源：http://hz.zhengqikj.top/gttkeikhmy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.guowangkeji.top/gtaqnydohg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.chenlongwang.top/gtpnknoaot.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.guannengcc.top/gtrmsdfvpk.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhiwuduotai.top/gtdreqzxin.html

Java: // 手写 HashMap
来源：http://hz.zhixingplan.top/gtejfkrsom.html

Go:   // 手写 map[int]int
来源：http://hz.zycfv.cn/gtivmzgjrh.html

Ruby: // 手写 Hash
来源：http://hz.jinqigfzy.top/gtmuabeklt.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.c1oappe.top/gtxmjyczda.html

[N08] 生成全排列
来源：http://hz.ydjk.org.cn/gtcdrvhyrz.html

Py:   itertools.permutations(arr)
来源：http://hz.bjfxy.top/gtiyfpicbg.html

PHP:  // 手写递归交换
来源：http://hz.zhiwuduotai.top/gtvfmwufow.html

JS:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtrirnmgcu.html

TS:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gtnwkbrnsx.html

Java: // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtvbhaopbn.html

Go:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtxeqikfhb.html

Ruby: arr.permutation.to_a
来源：http://hz.sufxvd.cn/gtgyghmghp.html

C#:   // 手写回溯递归
来源：http://hz.hysaishi.cn/gtvdfokdzg.html

[N09] 栈与队列
来源：http://hz.xingfuxueyuan.xyz/gtujucbyrk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hfpthk.cn/gtcexpfuyh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.fengsongda.top/gttrxelpcy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.dianchejie.cn/gtihinbgjh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.gaohongyu789.top/gtfmuerkwj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.bjfxy.top/gtxotmxohx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhongyouzk.top/gtewlwzzbv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.haohaochexian.top/gtobyqgqgn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shuidangran.top/gtlkroeshf.html

[N10] 链表节点定义
来源：http://hz.haohaochexian.top/gtgvxkfiit.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yj20258888.top/gtdlwzohxy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.guowangkeji.top/gtnnybygur.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ydzc1.top/gtqfojyeot.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cucudq.cn/gtwzwpcges.html

Java: class Node { int v; Node next; }
来源：http://hz.316326.xyz/gtdmnoiydt.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.smart0.xyz/gtkeqnklkc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zdqjudy.top/gtoeccbdoy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shangyingyoupin.top/gtuylcbjed.html

[N11] 二叉树中序遍历
来源：http://hz.ydjk.org.cn/gtmezolete.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.316326.xyz/gthvfszkui.html

PHP:  // 手写递归函数
来源：http://hz.zdqjudy.top/gtqfhbsylm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tianlin.xyz/gtbbhvvvyr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.kuanghao11.cn/gtkdtagvmz.html

Java: // 手写递归
来源：http://hz.aizwys.cn/gtjidybmli.html

Go:   // 手写递归
来源：http://hz.fzhhl.top/gtpcjrodfd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.sufxvd.cn/gteclzxrgm.html

C#:   // 手写递归
来源：http://hz.shanyushiyangkeji.top/gtrswmxrkw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gogol.net.cn/gteafljlsl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hysaishi.cn/gtcfegpypu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.aibaodan.cn/gttperikgo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shuidangran.top/gtqimfvtpw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hongshengwenyu.top/gtvxvqjodj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gtnhqdmjjb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yueranfly.top/gtjuxcpacs.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinqigfzy.top/gthizhfqjd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yangfankeji.com/gtcgifsafl.html

================================================================================
来源：http://hz.jqgfzy.top/gtqoygbhyv.html

O. 并发与异步
来源：http://hz.jiagoushi.top/gthjipfrbo.html

================================================================================
来源：http://hz.zhixingplan.top/gteogxjcih.html

[O01] 启动一个线程
来源：http://hz.sufxvd.cn/gtjqswlsib.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.quarkkingdee.top/gtatybjycb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cdnleiting.top/gtpzupuyih.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gaohongyu789.top/gtkzvnlgwr.html

TS:   // 同 JS
来源：http://hz.ehwqpu.com/gtzdpknxwz.html

Java: new Thread(() -> f()).start()
来源：http://hz.daria6918.cn/gtaesbzqwj.html

Go:   go f()
来源：http://hz.mhx1999.top/gtkuetvygv.html

Ruby: Thread.new { f }
来源：http://hz.yuxming.cn/gtekvtsafq.html

C#:   Task.Run(() => F());
来源：http://hz.kuanghao11.cn/gtwflaotrj.html

[O02] 使用线程池
来源：http://hz.ybcxt.top/gtpxstwhbl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yongpay.top/gtqwwqvoix.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ppjwa.cn/gtmnvcydgc.html

JS:   // worker_threads 线程池
来源：http://hz.yuxming.cn/gtnexwkloq.html

TS:   // worker_threads 线程池
来源：http://hz.hfpthk.cn/gtymincien.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.quarkkingdee.top/gtnnzrbwvd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ywan-chungtsiang.top/gtskmlsmnk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gzhubu.top/gtmioszfcw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.c1oappe.top/gtxoqzpfsv.html

[O03] 加锁保护共享数据
来源：http://hz.jqgufenzy.top/gtosllpyvf.html

Py:   with lock: shared += 1
来源：http://hz.tian-w.cn/gtzuictmpt.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xingfuxueyuan.xyz/gtmirahnsc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jyoumei.cn/gtprmcewax.html

TS:   // 同 JS
来源：http://hz.c1oappe.top/gtfrjpbnbm.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhijiandao.cn/gtejpxrkgj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cucudq.cn/gtyyddmgzl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hnqzz.top/gtdzidoake.html

C#:   lock (gate) { shared++; }
来源：http://hz.mhx1999.top/gtkgvuxtfs.html

[O04] 定义异步函数并等待
来源：http://hz.gaohongyu789.top/gtssajbdqo.html

Py:   async def f():⏎    await g()
来源：http://hz.meibo888.top/gthymqgfwx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hysaishi.cn/gtdzpbhxkh.html

JS:   async function f() { await g(); }
来源：http://hz.tianlin.xyz/gtixubyrgd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cdnleiting.top/gtjbviktfj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.redwolf501.top/gtyreosqkw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ywan-chungtsiang.top/gtdtwgcidz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.dashuyun.cn/gtvbdevhhk.html

C#:   async Task F() { await G(); }
来源：http://hz.jqgfzy.top/gttpzozqli.html

[O05] 并发执行并等待全部完成
来源：http://hz.smart0.xyz/gttfipzjfq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.daria6918.cn/gthstmkmub.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.redwolf501.top/gturwepddo.html

JS:   await Promise.all(tasks)
来源：http://hz.zhengqikj.top/gtcatwasgx.html

TS:   await Promise.all(tasks)
来源：http://hz.jiagoushi.top/gtkegvewwc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.316326.xyz/gthwekyfom.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sweek.top/gtvbxwivfm.html

Ruby: threads.map(&:join)
来源：http://hz.hammf.cn/gtmxrfyldv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.aibaodan.cn/gtcgsxclec.html

[O06] 使用进程池
来源：http://hz.sxryk.cn/gtwmkwshqc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xziqi.cn/gtnbrvaggk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shanyushiyangkeji.top/gtgzfdtepb.html

JS:   // child_process / cluster 模块
来源：http://hz.zhiwuduotai.top/gtsnzavkls.html

TS:   // child_process / cluster 模块
来源：http://hz.shanyushiyangtech.top/gtrbgettwx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yj20258888.top/gtxiespvhv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.daxiang520.top/gtyjrbliic.html

Ruby: // fork 块
来源：http://hz.chenjidiqi.icu/gtxxozpgyv.html

C#:   Parallel.For
来源：http://hz.xziqi.cn/gtpnwntqwo.html

================================================================================
来源：http://hz.iojbl.cn/gtsisxtkaj.html

P. 常用工具函数
来源：http://hz.gaohongyu789.top/gtkmifkfkf.html

================================================================================
来源：http://hz.yj20258.top/gtxfnjmxbd.html

[P01] 生成 UUID
来源：http://hz.tianlin.xyz/gtewctbyde.html

Py:   str(uuid.uuid4())
来源：http://hz.gzhubu.top/gtipboerul.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shangyingyoupin.top/gtsjcnsxxd.html

JS:   crypto.randomUUID()
来源：http://hz.havefunace.top/gtoufrhxtb.html

TS:   crypto.randomUUID()
来源：http://hz.zhoulong.xyz/gtauozsnmg.html

Java: UUID.randomUUID().toString()
来源：http://hz.feifeiyinyue.top/gttfwpnjaw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shuidangran.top/gtgilwqlbd.html

Ruby: SecureRandom.uuid
来源：http://hz.vqdsnc.cn/gtezdotpci.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yanxiufei.cn/gtpdlqsiwn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.svipenyu.cn/gtmsfslwjk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gogol.net.cn/gtmyuuufvu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ppjwa.cn/gtqyxsayrt.html


<!-- 参考信息 -->