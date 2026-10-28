代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuanzhike.top/gtxvuolibh.html

[L04] 设置超时
来源：http://hz.feifeiyinyue.top/gtcbusociu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.sweek.top/gtmpscokcj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cucudq.cn/gtlonaqvad.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.pengpengdd.cyou/gtqiftufgx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shuidangran.top/gtmsaarusa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yuanzhike.top/gtpusutcip.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.fzhhl.top/gtcqoexydl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shzxlz.cn/gtvtwvwoqg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ydzc1.top/gtrrzywaxs.html

[L05] 上传文件（multipart）
来源：http://hz.haohaochexian.top/gtabbuxavk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinyuanbaomall.cn/gtkxkxtyfs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.smart0.xyz/gtfsgbvlnd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258.top/gtkcmqkdqw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.feifeiyinyue.top/gtzjcglkxc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.redwolf501.top/gtrceuqyou.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.aizwys.cn/gteyqhxqrs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.fengsongda.top/gtdnbrphap.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj202588.top/gthviaimtr.html

[L06] 解析响应为 JSON
来源：http://hz.yj202588.top/gtqypnqzmm.html

Py:   resp.json()
来源：http://hz.aibaodan.cn/gtofnkvabg.html

PHP:  json_decode($body, true);
来源：http://hz.dashuyun.cn/gtbppnbwif.html

JS:   await resp.json()
来源：http://hz.wangshuangyany.cn/gtnlyuhlss.html

TS:   await resp.json()
来源：http://hz.316326.xyz/gtsmnzppsq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.snrcjt.cn/gtxsacmuqp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yonumen.top/gtxocjgxpo.html

Ruby: JSON.parse(resp.body)
来源：http://hz.nanxuanxn.top/gtykpxkpjx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.havefunace.top/gtxewzbylk.html

[L07] 处理 HTTP 状态码
来源：http://hz.yuxming.cn/gtspdkxtqt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yj20258888.top/gtdstonzku.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.tian-w.cn/gtqxpiqfvk.html

JS:   resp.ok;  resp.status
来源：http://hz.jianghu66.top/gttysuqskx.html

TS:   resp.ok;  resp.status
来源：http://hz.shangyingyoupin.top/gtunjpbyww.html

Java: resp.statusCode()
来源：http://hz.cucudq.cn/gtmzmqrvkq.html

Go:   resp.StatusCode
来源：http://hz.gotoacloud.top/gthnxkyjmj.html

Ruby: resp.code.to_i
来源：http://hz.yj20258.top/gthfmhnnjr.html

C#:   (int)resp.StatusCode
来源：http://hz.yanxiufei.cn/gtcwnpyikd.html

[L08] 并发请求多个地址
来源：http://hz.meibo888.top/gtytfqevxc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhaomingkeji.xyz/gtahjiatcn.html

PHP:  curl_multi_init() 系列
来源：http://hz.smart0.xyz/gticlrswut.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guannengcc.top/gtqbfawpdg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.haohaochexian.top/gthxtafunn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.nanxinkj.top/gtdssomxqv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yj202588.top/gtqmevvkxk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yj202588.top/gtoekbolkr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.c1oappe.top/gtijfkvtqq.html

================================================================================
来源：http://hz.gaohongyu789.top/gtbvzoyvrp.html

M. 命令行 / 进程 / 环境
来源：http://hz.xylfe.cn/gtwupwpoec.html

================================================================================
来源：http://hz.hongshengwenyu.top/gterhckomr.html

[M01] 读取命令行参数
来源：http://hz.yongpay.top/gtgrqigojt.html

Py:   sys.argv[1:]
来源：http://hz.ehwqpu.com/gtjhkjehcr.html

PHP:  $argv;  $argc;
来源：http://hz.zhijiandao.cn/gtltlpiorv.html

JS:   process.argv.slice(2)
来源：http://hz.haohaochexian.top/gtvtzjfgxc.html

TS:   process.argv.slice(2)
来源：http://hz.wangshuangyany.cn/gtwbuaomoo.html

Java: args 数组（main 方法参数）
来源：http://hz.xuetiantiany.cn/gtxojmaryz.html

Go:   os.Args[1:]
来源：http://hz.zdqjudy.top/gtpfdbffxc.html

Ruby: ARGV
来源：http://hz.yueranfly.top/gtpmdmuocu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nanxuanxn.top/gtyzksgfhj.html

[M02] 读取环境变量
来源：http://hz.yanxiufei.cn/gtdhoeusjc.html

Py:   os.environ.get("HOME")
来源：http://hz.zhengqikj.top/gtmvequosr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.kuanghao11.cn/gtaphkmqpy.html

JS:   process.env.HOME
来源：http://hz.yonumen.top/gtrspcfoha.html

TS:   process.env.HOME
来源：http://hz.xuanzx.com/gthxzrusup.html

Java: System.getenv("HOME")
来源：http://hz.fzhhl.top/gtpsdizdtw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhengqikj.top/gtustaftsx.html

Ruby: ENV["HOME"]
来源：http://hz.xuanzx.com/gthqofqupt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xylfe.cn/gtvmpbxapl.html

[M03] 执行外部命令
来源：http://hz.shangyingyoupin.top/gtdgpdgyql.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.52xcode.cn/gtvowbeyer.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shanyushiyangtech.top/gthevvagdb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj202588.top/gtrujancgb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnxiangtu.top/gtcwgfxfci.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.meibo888.top/gtntsswipr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jlsjyb.cn/gtwxfkjqdl.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinghuilouyu.cn/gttyfazixq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.tianlin.xyz/gtyodxyfmu.html

[M04] 获取当前工作目录
来源：http://hz.jqgufenzy.top/gtddpctzit.html

Py:   os.getcwd()
来源：http://hz.gogol.net.cn/gtmpohpqjh.html

PHP:  getcwd();
来源：http://hz.jlsjyb.cn/gtdaqdgtwz.html

JS:   process.cwd()
来源：http://hz.tanke756.top/gtwnarvgbg.html

TS:   process.cwd()
来源：http://hz.jqgufenzy.top/gtwckjdrke.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yangfankeji.com/gtuirfezrm.html

Go:   os.Getwd()
来源：http://hz.cqqwz.cn/gtqybuvkbh.html

Ruby: Dir.pwd
来源：http://hz.dianchejie.cn/gtyafhaoiz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jiagoushi.top/gtwjprkend.html

[M05] 设置退出码
来源：http://hz.pengpengdd.cyou/gtgoppdmyt.html

Py:   sys.exit(1)
来源：http://hz.smart0.xyz/gtvlhcxvww.html

PHP:  exit(1);
来源：http://hz.sxryk.cn/gtmfrarltz.html

JS:   process.exit(1)
来源：http://hz.ydjk.org.cn/gttwlnnrzp.html

TS:   process.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtfoxudwku.html

Java: System.exit(1)
来源：http://hz.aizwys.cn/gtpxdksgvy.html

Go:   os.Exit(1)
来源：http://hz.shuidangran.top/gtyugbjekg.html

Ruby: exit 1
来源：http://hz.jyoumei.cn/gtabciknfm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jlsjyb.cn/gtoaukplyq.html

[M06] 向标准错误输出
来源：http://hz.redwolf501.top/gtiggraupg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cdnleiting.top/gtpvsbxnze.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yueranfly.top/gtumssegsl.html

JS:   console.error("err")
来源：http://hz.jyoumei.cn/gtpdktyzko.html

TS:   console.error("err")
来源：http://hz.birdmap.top/gtlfmlioyd.html

Java: System.err.println("err")
来源：http://hz.haohaochexian.top/gtzsqjlgui.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jinqigufen.top/gtwtxnceug.html

Ruby: warn "err"
来源：http://hz.quarkkingdee.top/gtmucafmgl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhoulong.xyz/gtbqomrukn.html

[M07] 判断是否为主入口
来源：http://hz.xingfuxueyuan.xyz/gtianeklyt.html

Py:   if __name__ == "__main__":
来源：http://hz.gogol.net.cn/gtjjookusw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.daxiang520.top/gtukudawor.html

JS:   require.main === module
来源：http://hz.jinyuanbaomall.cn/gtunoopxix.html

TS:   require.main === module
来源：http://hz.mhx1999.top/gtucrwngim.html

Java: public static void main(String[] args)
来源：http://hz.xuetiantiany.cn/gtikgcmylo.html

Go:   func main()
来源：http://hz.zhixingplan.top/gtfccvicwe.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cheryme.top/gtbxntbuxx.html

C#:   static void Main(string[] args)
来源：http://hz.zhijiandao.cn/gtgdxmvboi.html

[M08] 获取系统与运行时信息
来源：http://hz.jlsjyb.cn/gtcpvgbdxh.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhengqikj.top/gthvcganjo.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.vqdsnc.cn/gtakvfcynl.html

JS:   process.platform;  process.version
来源：http://hz.zhaomingkeji.xyz/gtjyvdxder.html

TS:   process.platform;  process.version
来源：http://hz.tanke756.top/gtofvffieb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.pycfn.com/gtjmnucpri.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xuetiantiany.cn/gtnltuhttr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.feifeiyinyue.top/gttzqxssld.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.vqdsnc.cn/gtnfxmcpot.html

================================================================================
来源：http://hz.sufxvd.cn/gtsmxezlvg.html

N. 数据结构与算法
来源：http://hz.fzhhl.top/gtjahwjxlf.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtzebpiwdv.html

[N01] 二分查找（有序数组）
来源：http://hz.zhiwuduotai.top/gtyrwkcabf.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ydjk.org.cn/gtjzpictap.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.dianchejie.cn/gthqbnzadc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jyoumei.cn/gtnvnghvvf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangdashe.top/gtviusecaq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cucudq.cn/gtadajazed.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.dianchejie.cn/gtlxgthcls.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.bjfxy.top/gtnxcizkkc.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nanxinkj.top/gtaqjjlkmw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.havefunace.top/gtwazkgrcx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shuidangran.top/gtrhlwwudr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.aibaodan.cn/gtnpghcodv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.snrcjt.cn/gtfsyvedgr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuanzhike.top/gtvrqjdzea.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.tian-w.cn/gthkdgowhj.html

Go:   slices.Sort(arr)
来源：http://hz.aibaodan.cn/gtdqetdflg.html

Ruby: arr.sort
来源：http://hz.ybcxt.top/gtrgjsrnjj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.haohaochexian.top/gtwfcjkjxk.html

[N03] 快速排序（分治示例）
来源：http://hz.daxiang520.top/gttxbqpqrp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.nanxinkj.top/gtqznlrzkk.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gotoacloud.top/gtanavudxq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xylfe.cn/gtvabtkopm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gtdyxcasxz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.chenjidiqi.icu/gtpfhttgmo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yangfankeji.com/gtcngfguzf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xuetiantiany.cn/gtfocjjedr.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhoulong.xyz/gtmczbdypd.html

[N04] 斐波那契数列
来源：http://hz.9152youxi.cn/gtqdsvdsuv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinyuanbaomall.cn/gtaaqbqrvh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.guowangkeji.top/gtucqhlryk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.quarkkingdee.top/gtphivnijh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.smart0.xyz/gtnpfnbczz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gogol.net.cn/gtbvmeotfp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xingfuxueyuan.xyz/gtmwxcmzno.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ywan-chungtsiang.top/gtfbfpbclv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.0kj1m.cn/gttkwbbdsy.html

[N05] 最大公约数
来源：http://hz.zhixingplan.top/gtbjplxbpm.html

Py:   math.gcd(a, b)
来源：http://hz.c1oappe.top/gttwmosuot.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinqigfzy.top/gttrtynitr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daria6918.cn/gtqlugxufm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hywenlv.cn/gtoeqoklch.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jianghu66.top/gtlolasasy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yj202588.top/gtueuttwpa.html

Ruby: a.gcd(b)
来源：http://hz.zhongyouzk.top/gttwfvsypx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.dianchejie.cn/gtamwdxavk.html

[N06] 判断回文字符串
来源：http://hz.hfpthk.cn/gtkipzzqlc.html

Py:   s == s[::-1]
来源：http://hz.ppjwa.cn/gthtayttta.html

PHP:  $s === strrev($s);
来源：http://hz.zhengqikj.top/gtxjcdomcx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gttlyjrbrt.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtorvrdajp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.birdmap.top/gtyzzbyxyf.html

Go:   // 双指针从两端比较
来源：http://hz.xinyue.icu/gtxgaeqtfw.html

Ruby: s == s.reverse
来源：http://hz.52xcode.cn/gtrnrlotqo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.nwbrower.top/gtcgakrbiz.html

[N07] 两数之和（返回下标）
来源：http://hz.jinghuilouyu.cn/gtfzbexvdw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinqigufen.top/gtpuoyxgzf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hnxiangtu.top/gthohrurjg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.daxiang520.top/gtsxzqokgu.html

TS:   // 手写 Map<string, number>
来源：http://hz.pycfn.com/gtadeblrme.html

Java: // 手写 HashMap
来源：http://hz.meibo888.top/gtrtpgxyjn.html

Go:   // 手写 map[int]int
来源：http://hz.zdqjudy.top/gtjzglieju.html

Ruby: // 手写 Hash
来源：http://hz.jlsjyb.cn/gthihqxtoo.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.tian-w.cn/gtuomjssmd.html

[N08] 生成全排列
来源：http://hz.hfpthk.cn/gtoufpvxco.html

Py:   itertools.permutations(arr)
来源：http://hz.jinqigfzy.top/gtpzylwibr.html

PHP:  // 手写递归交换
来源：http://hz.jiagoushi.top/gtgxjeljfu.html

JS:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtzqoxgtyz.html

TS:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtpeubupoo.html

Java: // 手写回溯递归
来源：http://hz.jiagoushi.top/gtcwvbfrwl.html

Go:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtwvcvsbfq.html

Ruby: arr.permutation.to_a
来源：http://hz.zhijiandao.cn/gtxhrazztd.html

C#:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtcjcypsmq.html

[N09] 栈与队列
来源：http://hz.xingfuxueyuan.xyz/gtcdmaveca.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.iojbl.cn/gtnanfpejb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.tianlin.xyz/gtbivgmoul.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ywan-chungtsiang.top/gtbezeefir.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.pengpengdd.cyou/gttycmgucw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.svipenyu.cn/gtgbvdufxg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.nanxinkj.top/gtwtmtmxcr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.nanxinkj.top/gtozgxrsop.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yj20258888.top/gtmlixrrsd.html

[N10] 链表节点定义
来源：http://hz.zhongyouzk.top/gtdruwopog.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hysaishi.cn/gtozvicowi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinyuanbaomall.cn/gtzxdgncky.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hywenlv.cn/gtxkyewybr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yj20258.top/gtlgvoyses.html

Java: class Node { int v; Node next; }
来源：http://hz.tian-w.cn/gtkmogtyfr.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.daxiang520.top/gtrwpulxkz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shanyushiyangkeji.top/gtusdfcoka.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.iojbl.cn/gtrhmkugtr.html

[N11] 二叉树中序遍历
来源：http://hz.guowangkeji.top/gtfjoeogsr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinqigufen.top/gtyfpoqpsl.html

PHP:  // 手写递归函数
来源：http://hz.yonumen.top/gtynsqlqlg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shangyingyoupin.top/gtcexcjvev.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.daxiang520.top/gtdfhfdyzg.html

Java: // 手写递归
来源：http://hz.xylfe.cn/gtuyzbegxr.html

Go:   // 手写递归
来源：http://hz.haohaochexian.top/gtxeotuizh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.wangshuangyany.cn/gtugrflttz.html

C#:   // 手写递归
来源：http://hz.wangdashe.top/gtxiymuipw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yj20258888.top/gtqkztvbfk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhongyouzk.top/gtlunevunc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xylfe.cn/gtccyupqce.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ivvv.top/gtiwybhqkf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hongshengwenyu.top/gtnhehpdgx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.bjfxy.top/gtljqbwoku.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xuetiantiany.cn/gtjtikrhlu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jqgufenzy.top/gtiefhnxca.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.9152youxi.cn/gtbgunylyd.html

================================================================================
来源：http://hz.sysykeji.top/gtctyuswvn.html

O. 并发与异步
来源：http://hz.fengsongda.top/gtkfhsjlmj.html

================================================================================
来源：http://hz.guannengcc.top/gtqbuaeuhr.html

[O01] 启动一个线程
来源：http://hz.wangshuangyany.cn/gtrakovqrm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cqqwz.cn/gthgcinfdi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zdqjudy.top/gtejnndezu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.0kj1m.cn/gtlwpcjqyg.html

TS:   // 同 JS
来源：http://hz.xziqi.cn/gtscdryxtk.html

Java: new Thread(() -> f()).start()
来源：http://hz.sufxvd.cn/gtkezodkxc.html

Go:   go f()
来源：http://hz.52xcode.cn/gtlawmduij.html

Ruby: Thread.new { f }
来源：http://hz.yanxiufei.cn/gtbrmjbbtb.html

C#:   Task.Run(() => F());
来源：http://hz.chenjidiqi.icu/gtpdmdxdaf.html

[O02] 使用线程池
来源：http://hz.guowangkeji.top/gtibfebsem.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhengqikj.top/gtybcyohrw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xuanzx.com/gtdpwamcaf.html

JS:   // worker_threads 线程池
来源：http://hz.dianchejie.cn/gtkjjomdsx.html

TS:   // worker_threads 线程池
来源：http://hz.jinyuanbaomall.cn/gtpguhqdtr.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.chenjidiqi.icu/gtsfarajzw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yonumen.top/gtsljlveih.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xylfe.cn/gtwhifmvfw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ybcxt.top/gtdcugptpr.html

[O03] 加锁保护共享数据
来源：http://hz.xingfuxueyuan.xyz/gtiqkcuiaa.html

Py:   with lock: shared += 1
来源：http://hz.0kj1m.cn/gtsqlsincy.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xingfuxueyuan.xyz/gtamqpybij.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.mhx1999.top/gtkzcdlrfn.html

TS:   // 同 JS
来源：http://hz.guowangkeji.top/gtynbbqizo.html

Java: synchronized (this) { shared++; }
来源：http://hz.c1oappe.top/gtbcxrtklu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xingfuxueyuan.xyz/gtrtijjzcl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.meibo888.top/gtmqtbffof.html

C#:   lock (gate) { shared++; }
来源：http://hz.hammf.cn/gtrcjjgavv.html

[O04] 定义异步函数并等待
来源：http://hz.jianghu66.top/gtonxvtkth.html

Py:   async def f():⏎    await g()
来源：http://hz.hywenlv.cn/gtsruknckx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.pycfn.com/gtdynkjvoz.html

JS:   async function f() { await g(); }
来源：http://hz.ppjwa.cn/gtyapmwtmw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.nanxuanxn.top/gtghbptxeo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jianghu66.top/gtuuooxbua.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.chenjidiqi.icu/gtgsrbqqqz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jinyuanbaomall.cn/gttcaxuocv.html

C#:   async Task F() { await G(); }
来源：http://hz.zycfv.cn/gtnqsimzst.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhaomingkeji.xyz/gtxyvayqxk.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shangyingyoupin.top/gtzoifrvuw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jyoumei.cn/gtybkltrch.html

JS:   await Promise.all(tasks)
来源：http://hz.zhijiandao.cn/gtppjpopet.html

TS:   await Promise.all(tasks)
来源：http://hz.yanxiufei.cn/gtnjyhscdi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ivvv.top/gtuzxpnrtb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cqqwz.cn/gthgwalgmv.html

Ruby: threads.map(&:join)
来源：http://hz.ehwqpu.com/gtjlnzavaw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.fengsongda.top/gthbtrkmhs.html

[O06] 使用进程池
来源：http://hz.gotoacloud.top/gtrcwxptjc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.nwbrower.top/gtvmtmelvr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zycfv.cn/gtidvaxjqh.html

JS:   // child_process / cluster 模块
来源：http://hz.ppjwa.cn/gtjqpqneyz.html

TS:   // child_process / cluster 模块
来源：http://hz.9152youxi.cn/gtmyhimqzg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ydjk.org.cn/gttujwdmqe.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gotoacloud.top/gtwbzptsca.html

Ruby: // fork 块
来源：http://hz.nanxuanxn.top/gtrrebarhm.html

C#:   Parallel.For
来源：http://hz.birdmap.top/gtajgnojwq.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtbtlsderz.html

P. 常用工具函数
来源：http://hz.feifeiyinyue.top/gtytktlccl.html

================================================================================
来源：http://hz.sweek.top/gtfjiubhib.html

[P01] 生成 UUID
来源：http://hz.wangshuangyany.cn/gtqzbskepg.html

Py:   str(uuid.uuid4())
来源：http://hz.svipenyu.cn/gtctmfavnk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gogol.net.cn/gtphfbxide.html

JS:   crypto.randomUUID()
来源：http://hz.xuetiantiany.cn/gtigsxvwte.html

TS:   crypto.randomUUID()
来源：http://hz.chenzaomai.com/gtkuykdqqv.html

Java: UUID.randomUUID().toString()
来源：http://hz.fzhhl.top/gtovzwjmwz.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shanyushiyangtech.top/gtcfljmwbm.html

Ruby: SecureRandom.uuid
来源：http://hz.mhx1999.top/gtqsayomoo.html


<!-- 参考信息 -->