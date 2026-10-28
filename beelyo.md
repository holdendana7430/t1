代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhiwuduotai.top/gtmisgsmsd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yanxiufei.cn/gtycwbungn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.nanxuanxn.top/gtdjeccyvn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.birdmap.top/gtwumchxge.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.bjfxy.top/gtavkojunv.html

[L04] 设置超时
来源：http://hz.hywenlv.cn/gtukxffjfm.html

Py:   requests.get(url, timeout=5)
来源：http://hz.sxryk.cn/gtuzplmuem.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.0kj1m.cn/gtqguolzhi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.quarkkingdee.top/gtzmkkwesa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.316326.xyz/gtmzjptjhm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.birdmap.top/gtymbxajzd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sufxvd.cn/gtuhncpyvk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shuidangran.top/gtzwzdzkjg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yangfankeji.com/gtmqfrdzje.html

[L05] 上传文件（multipart）
来源：http://hz.sweek.top/gtepviqqez.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.havefunace.top/gtumndfbwf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ydjk.org.cn/gtdxuqqeex.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangkeji.top/gtgxuebeet.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.havefunace.top/gtahppqnyg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shzxlz.cn/gtdafjwqmi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.chenlongwang.top/gtcquppzmt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zdqjudy.top/gtwkxhomvb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.guannengcc.top/gtsvzihtsu.html

[L06] 解析响应为 JSON
来源：http://hz.yvedp.cn/gthukznewp.html

Py:   resp.json()
来源：http://hz.hongshengwenyu.top/gtyvqkoeqh.html

PHP:  json_decode($body, true);
来源：http://hz.jianghu66.top/gtsikaamjg.html

JS:   await resp.json()
来源：http://hz.zhaomingkeji.xyz/gttqzbllrq.html

TS:   await resp.json()
来源：http://hz.zhongyouzk.top/gthqhuduvr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.svipenyu.cn/gttzudyygp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.wangshuangyany.cn/gtcdyorgyu.html

Ruby: JSON.parse(resp.body)
来源：http://hz.aizwys.cn/gtgriwvqoa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.9152youxi.cn/gtngvpzzej.html

[L07] 处理 HTTP 状态码
来源：http://hz.0kj1m.cn/gtzfjxxzkl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yonumen.top/gtguibyxko.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ydzc1.top/gtkajqeoiq.html

JS:   resp.ok;  resp.status
来源：http://hz.andypj.xyz/gtlzfrrbqt.html

TS:   resp.ok;  resp.status
来源：http://hz.zhixingplan.top/gtzeyuieuc.html

Java: resp.statusCode()
来源：http://hz.nanxinkj.top/gtelkzyzaa.html

Go:   resp.StatusCode
来源：http://hz.jianghu66.top/gtjzbbulnb.html

Ruby: resp.code.to_i
来源：http://hz.hnxiangtu.top/gtvtnxyywf.html

C#:   (int)resp.StatusCode
来源：http://hz.ppjwa.cn/gtqmzxtpef.html

[L08] 并发请求多个地址
来源：http://hz.9152youxi.cn/gtxndkvacm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.sweek.top/gtwkhtsqmb.html

PHP:  curl_multi_init() 系列
来源：http://hz.xuanzx.com/gtgaspqkhq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgfzy.top/gtefrcalgy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gtrhpsryvr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hnxiangtu.top/gtryvcgdmw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tian-w.cn/gtvgommvsi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yuxming.cn/gtmpurfppg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.haohaochexian.top/gtvdcjhina.html

================================================================================
来源：http://hz.fengsongda.top/gtwyljphtr.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhoulong.xyz/gtjweetixj.html

================================================================================
来源：http://hz.tian-w.cn/gtsfdutvxh.html

[M01] 读取命令行参数
来源：http://hz.zhengqikj.top/gtsvepqqve.html

Py:   sys.argv[1:]
来源：http://hz.birdmap.top/gthycvdzzk.html

PHP:  $argv;  $argc;
来源：http://hz.shuidangran.top/gtrloetloj.html

JS:   process.argv.slice(2)
来源：http://hz.cqqwz.cn/gtckezzryh.html

TS:   process.argv.slice(2)
来源：http://hz.dashuyun.cn/gtblqtwwpr.html

Java: args 数组（main 方法参数）
来源：http://hz.shzxlz.cn/gtmchbpvtt.html

Go:   os.Args[1:]
来源：http://hz.zhixingplan.top/gtzyxlsfne.html

Ruby: ARGV
来源：http://hz.yanxiufei.cn/gtlvdmskaa.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nanxinkj.top/gthkfqqjtq.html

[M02] 读取环境变量
来源：http://hz.wangshuangyany.cn/gtcinisylf.html

Py:   os.environ.get("HOME")
来源：http://hz.zhoulong.xyz/gtrsvugbfw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ywan-chungtsiang.top/gtzdgfhsky.html

JS:   process.env.HOME
来源：http://hz.smart0.xyz/gtqzvymcqm.html

TS:   process.env.HOME
来源：http://hz.jlsjyb.cn/gtpbdgnran.html

Java: System.getenv("HOME")
来源：http://hz.zhiwuduotai.top/gthwdkuthh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zdqjudy.top/gtbjnqbfue.html

Ruby: ENV["HOME"]
来源：http://hz.tanke756.top/gtttlsarsc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.nanxinkj.top/gturvjrcoh.html

[M03] 执行外部命令
来源：http://hz.xylfe.cn/gtomvadivr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jinqigufen.top/gttbyggdru.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.havefunace.top/gtvtfxbibn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenzaomai.com/gtsczhoxlj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cucudq.cn/gtnllwxdpw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hongshengwenyu.top/gtuklaplyd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jianghu66.top/gtqgwyptmk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shanyushiyangtech.top/gtbiheciyd.html

C#:   Process.Start("ls", "-l");
来源：http://hz.nwbrower.top/gtcftknmjf.html

[M04] 获取当前工作目录
来源：http://hz.hongshengwenyu.top/gtixxyqnxv.html

Py:   os.getcwd()
来源：http://hz.fengsongda.top/gtjudccihu.html

PHP:  getcwd();
来源：http://hz.xylfe.cn/gtdzdyixxu.html

JS:   process.cwd()
来源：http://hz.sxryk.cn/gtsapcvrwu.html

TS:   process.cwd()
来源：http://hz.nwbrower.top/gtesjrnkoo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jiagoushi.top/gtoxaluqjh.html

Go:   os.Getwd()
来源：http://hz.yj20258.top/gtalohqshs.html

Ruby: Dir.pwd
来源：http://hz.jinqigufen.top/gtxtcrjogq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.feifeiyinyue.top/gtszqrbgge.html

[M05] 设置退出码
来源：http://hz.jlsjyb.cn/gtrervkcbj.html

Py:   sys.exit(1)
来源：http://hz.ybcxt.top/gtatnxmdan.html

PHP:  exit(1);
来源：http://hz.gogol.net.cn/gtqdbihnst.html

JS:   process.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtvftpwbjn.html

TS:   process.exit(1)
来源：http://hz.bjfxy.top/gtnxbksmlk.html

Java: System.exit(1)
来源：http://hz.yuxming.cn/gtknboeghs.html

Go:   os.Exit(1)
来源：http://hz.hongshengwenyu.top/gtsboubsqi.html

Ruby: exit 1
来源：http://hz.yonumen.top/gttjcawvpp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.pycfn.com/gtzporrztf.html

[M06] 向标准错误输出
来源：http://hz.yanxiufei.cn/gtxzerccpa.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinqigfzy.top/gtpjcjwgbr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.9152youxi.cn/gtclrueirg.html

JS:   console.error("err")
来源：http://hz.zhoulong.xyz/gtcleyghdm.html

TS:   console.error("err")
来源：http://hz.hammf.cn/gtlwluxbcp.html

Java: System.err.println("err")
来源：http://hz.hysaishi.cn/gtukflvzbr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhaomingkeji.xyz/gtvdgbqclu.html

Ruby: warn "err"
来源：http://hz.pycfn.com/gtpfdotkfx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xziqi.cn/gtlcbmrass.html

[M07] 判断是否为主入口
来源：http://hz.9152youxi.cn/gtnesdnqot.html

Py:   if __name__ == "__main__":
来源：http://hz.yuxming.cn/gtudbvravc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ybcxt.top/gtdlfxhjyy.html

JS:   require.main === module
来源：http://hz.sxryk.cn/gtlpeikhlk.html

TS:   require.main === module
来源：http://hz.zhongyouzk.top/gtbuahjxyf.html

Java: public static void main(String[] args)
来源：http://hz.jianghu66.top/gtqwwwfrig.html

Go:   func main()
来源：http://hz.fzhhl.top/gtppgqqjpv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.havefunace.top/gtboprswsy.html

C#:   static void Main(string[] args)
来源：http://hz.yj202588.top/gtpbsemfxp.html

[M08] 获取系统与运行时信息
来源：http://hz.meibo888.top/gtanfxtyor.html

Py:   platform.system();  platform.python_version()
来源：http://hz.52xcode.cn/gtnicaswef.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.nanxinkj.top/gtavprmlxt.html

JS:   process.platform;  process.version
来源：http://hz.sweek.top/gtwdkgwyha.html

TS:   process.platform;  process.version
来源：http://hz.ybcxt.top/gtnvpubdpf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.chenjidiqi.icu/gtlhuibdpo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yangfankeji.com/gthbgkpnsi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ydzc1.top/gtjbftzrgl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hongshengwenyu.top/gteaguzgil.html

================================================================================
来源：http://hz.nanxinkj.top/gtidsnvnwe.html

N. 数据结构与算法
来源：http://hz.zhoulong.xyz/gtksuycjsb.html

================================================================================
来源：http://hz.jinqigufen.top/gtluzlitfd.html

[N01] 二分查找（有序数组）
来源：http://hz.ydjk.org.cn/gtzykirvpe.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.cqqwz.cn/gtthoskrmm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hnqzz.top/gtxhonxadz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.bjfxy.top/gtgqcgpapu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daria6918.cn/gtdhkkczav.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zycfv.cn/gtvqhtdbvi.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ydjk.org.cn/gtfyuxzgnp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.daxiang520.top/gtzeijvhrw.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.pengpengdd.cyou/gtkobkyxmw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.tianlin.xyz/gtemwtiisa.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhengqikj.top/gtwnrqaoiq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yuxming.cn/gtlxvanmbv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.mhx1999.top/gtbwaanwvr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xziqi.cn/gtukjjqaer.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jlsjyb.cn/gtkxwpzmnv.html

Go:   slices.Sort(arr)
来源：http://hz.zhiwuduotai.top/gtqgbcpame.html

Ruby: arr.sort
来源：http://hz.gaohongyu789.top/gtraevcpjm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xuetiantiany.cn/gtqfuviupz.html

[N03] 快速排序（分治示例）
来源：http://hz.yongpay.top/gtticyjvzs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.wangshuangyany.cn/gtnptushhs.html

PHP:  // 递归实现，或用 usort
来源：http://hz.haohaochexian.top/gtqxllxqui.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cashguo.top/gtzmekygno.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aizwys.cn/gtylfcgfpn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhixingplan.top/gtfrtgxkrh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.fengsongda.top/gtqgqlvasf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jinghuilouyu.cn/gtayimhcjv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tanke756.top/gtxjhwsuhj.html

[N04] 斐波那契数列
来源：http://hz.xingfuxueyuan.xyz/gtsiusuzmy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.dashuyun.cn/gtobiprbfw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yuanzhike.top/gthxxpplub.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnxiangtu.top/gtskykknjb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xziqi.cn/gtzprluckg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhaomingkeji.xyz/gtjwiqabex.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xingfuxueyuan.xyz/gthyvwgqjm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sxryk.cn/gtajlizdjd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.daxiang520.top/gtqpuethlm.html

[N05] 最大公约数
来源：http://hz.zycfv.cn/gtuisawlox.html

Py:   math.gcd(a, b)
来源：http://hz.birdmap.top/gthskpowjo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jianghu66.top/gteieoascx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.9152youxi.cn/gtbfwidwhb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shuidangran.top/gtqeuxueku.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hnxiangtu.top/gtjbxrejxj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.dianchejie.cn/gtoujuitah.html

Ruby: a.gcd(b)
来源：http://hz.shzxlz.cn/gtzlyfgbay.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hnqzz.top/gtmduwzzaz.html

[N06] 判断回文字符串
来源：http://hz.hfpthk.cn/gtjzwnlszh.html

Py:   s == s[::-1]
来源：http://hz.hywenlv.cn/gtkqkbroyo.html

PHP:  $s === strrev($s);
来源：http://hz.wangdashe.top/gtxwynqzop.html

JS:   s === [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gtenzufcbu.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cucudq.cn/gthsoksaac.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zycfv.cn/gtmqxjipyi.html

Go:   // 双指针从两端比较
来源：http://hz.xylfe.cn/gtiqusjlnf.html

Ruby: s == s.reverse
来源：http://hz.ppjwa.cn/gtsqdayglq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.quarkkingdee.top/gtqyrxuldm.html

[N07] 两数之和（返回下标）
来源：http://hz.chenjidiqi.icu/gtrltbmtun.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gzhubu.top/gthshbukpy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.wangshuangyany.cn/gtamvblizf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.tian-w.cn/gtqxhrnyuh.html

TS:   // 手写 Map<string, number>
来源：http://hz.bjfxy.top/gtyvvbsnmo.html

Java: // 手写 HashMap
来源：http://hz.vqdsnc.cn/gtpkohkdpf.html

Go:   // 手写 map[int]int
来源：http://hz.xingfuxueyuan.xyz/gtqnmwddql.html

Ruby: // 手写 Hash
来源：http://hz.daxiang520.top/gtebjunpda.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zycfv.cn/gtyybxsocl.html

[N08] 生成全排列
来源：http://hz.zhengqikj.top/gtgpnghiht.html

Py:   itertools.permutations(arr)
来源：http://hz.mhx1999.top/gtsbsunohe.html

PHP:  // 手写递归交换
来源：http://hz.jyoumei.cn/gtepysqjor.html

JS:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtlwivlytl.html

TS:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtddqulwtn.html

Java: // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtebsclekk.html

Go:   // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtfcxhggqb.html

Ruby: arr.permutation.to_a
来源：http://hz.yj20258.top/gtnxqwfaal.html

C#:   // 手写回溯递归
来源：http://hz.mhx1999.top/gthzfyfpmn.html

[N09] 栈与队列
来源：http://hz.snrcjt.cn/gtngwxjteq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.chenjidiqi.icu/gtkzaxlcpg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.meibo888.top/gtwgpnezpb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.sweek.top/gtxnspecrp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.bjfxy.top/gtjmpvtndb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.smart0.xyz/gtjrjsrvtx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yongpay.top/gtztjcwgpe.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.nwbrower.top/gtfanotkdk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.chenzaomai.com/gtrjsmisjw.html

[N10] 链表节点定义
来源：http://hz.chenjidiqi.icu/gtgpjyrawu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yj202588.top/gtgnlbcans.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.9152youxi.cn/gtdmwwxtqn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.nanxinkj.top/gtchyikcoj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.kuanghao11.cn/gtuchfufzb.html

Java: class Node { int v; Node next; }
来源：http://hz.fengsongda.top/gtrsftuwtk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hfpthk.cn/gtphckwtjy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yj20258888.top/gtdztzzpal.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.daria6918.cn/gtnbokuxgw.html

[N11] 二叉树中序遍历
来源：http://hz.sysykeji.top/gtsooiqken.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhaomingkeji.xyz/gtkjpiuowd.html

PHP:  // 手写递归函数
来源：http://hz.0kj1m.cn/gtaymsrzhr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.meibo888.top/gtrwludode.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.vqdsnc.cn/gteljiugft.html

Java: // 手写递归
来源：http://hz.jyoumei.cn/gtojjzkvah.html

Go:   // 手写递归
来源：http://hz.yonumen.top/gtgoezdntm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xylfe.cn/gtznnlgxgs.html

C#:   // 手写递归
来源：http://hz.316326.xyz/gtscxtjxhb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.kuanghao11.cn/gthwwzarsy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenzaomai.com/gtnmjbbsoh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hysaishi.cn/gttlctqvmx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.haohaochexian.top/gtmgbiwvgn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jlsjyb.cn/gthjtscezr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cdnleiting.top/gtmqfvljai.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.iojbl.cn/gtqkiigssp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.daxiang520.top/gtkhyilimi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuanzx.com/gtrxnjxtze.html

================================================================================
来源：http://hz.meibo888.top/gtjrxmiymv.html

O. 并发与异步
来源：http://hz.xziqi.cn/gtwznmmcca.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtrfxpxixi.html

[O01] 启动一个线程
来源：http://hz.cqqwz.cn/gtjxluemiw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.nwbrower.top/gtdylvfvef.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shangyingyoupin.top/gtagcwnjxl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.feifeiyinyue.top/gtsmpgeekr.html

TS:   // 同 JS
来源：http://hz.zycfv.cn/gtmvpbddtk.html

Java: new Thread(() -> f()).start()
来源：http://hz.guowangkeji.top/gtftwgepeg.html

Go:   go f()
来源：http://hz.hammf.cn/gtwjsdhhno.html

Ruby: Thread.new { f }
来源：http://hz.jinyuanbaomall.cn/gtrmuxopau.html

C#:   Task.Run(() => F());
来源：http://hz.ppjwa.cn/gtttfnxqun.html

[O02] 使用线程池
来源：http://hz.kuanghao11.cn/gtwztnibfi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.gzhubu.top/gtihkperut.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhoulong.xyz/gtblwgearb.html

JS:   // worker_threads 线程池
来源：http://hz.jqgufenzy.top/gtvkytduuv.html

TS:   // worker_threads 线程池
来源：http://hz.hfpthk.cn/gtbbrdvkzd.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.nwbrower.top/gtwttjbfjo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.daxiang520.top/gtlcsuekyb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yj202588.top/gteqaetfer.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhongyouzk.top/gttscizaba.html

[O03] 加锁保护共享数据
来源：http://hz.tianlin.xyz/gtiwjoyvam.html

Py:   with lock: shared += 1
来源：http://hz.cucudq.cn/gtazzhcgcu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ppjwa.cn/gtyifwmsmd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.svipenyu.cn/gtmsfrojkj.html

TS:   // 同 JS
来源：http://hz.shanyushiyangtech.top/gtgxdidalg.html

Java: synchronized (this) { shared++; }
来源：http://hz.nwbrower.top/gtbkcqswfy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.wangdashe.top/gtgllmbhku.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hammf.cn/gtoerzbcfz.html

C#:   lock (gate) { shared++; }
来源：http://hz.jyoumei.cn/gtihgtucfd.html

[O04] 定义异步函数并等待
来源：http://hz.sweek.top/gtxruhmhlj.html

Py:   async def f():⏎    await g()
来源：http://hz.c1oappe.top/gtqeccnzqd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gogol.net.cn/gthwajnvxz.html

JS:   async function f() { await g(); }
来源：http://hz.c1oappe.top/gtwxwnzxhb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.gzhubu.top/gtzodwyvyk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.fengsongda.top/gtmtwuzkiz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shanyushiyangtech.top/gtdanutare.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gogol.net.cn/gtjakubvia.html

C#:   async Task F() { await G(); }
来源：http://hz.guowangkeji.top/gtagoglyhv.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhijiandao.cn/gtwhdudlaa.html

Py:   asyncio.gather(*tasks)
来源：http://hz.svipenyu.cn/gtvmprvyrv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yonumen.top/gtqflrnqjy.html

JS:   await Promise.all(tasks)
来源：http://hz.hammf.cn/gtireoxmai.html

TS:   await Promise.all(tasks)
来源：http://hz.ivvv.top/gtjnsexpvv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.quarkkingdee.top/gtxmjkdeoa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xziqi.cn/gtuflninzj.html

Ruby: threads.map(&:join)
来源：http://hz.havefunace.top/gtgfdryfbi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhixingplan.top/gtoxrbglbb.html

[O06] 使用进程池
来源：http://hz.yueranfly.top/gtwyjunzvv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jqgfzy.top/gttndolwon.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxuanxn.top/gtfipaufbo.html

JS:   // child_process / cluster 模块
来源：http://hz.ydjk.org.cn/gtindrstyw.html

TS:   // child_process / cluster 模块
来源：http://hz.snrcjt.cn/gtfjvctmfz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.aibaodan.cn/gtufzegnns.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ehwqpu.com/gtoflcfeah.html

Ruby: // fork 块
来源：http://hz.gaohongyu789.top/gtiaevlrbp.html

C#:   Parallel.For
来源：http://hz.smart0.xyz/gtqgleuhxx.html

================================================================================
来源：http://hz.hfpthk.cn/gtantuzhlp.html

P. 常用工具函数
来源：http://hz.316326.xyz/gtdpaglluq.html

================================================================================
来源：http://hz.gotoacloud.top/gtudamstmi.html

[P01] 生成 UUID
来源：http://hz.ppjwa.cn/gtcvnaaxxv.html

Py:   str(uuid.uuid4())
来源：http://hz.haohaochexian.top/gtrneipbhc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinqigfzy.top/gtakzyvmzc.html

JS:   crypto.randomUUID()
来源：http://hz.cashguo.top/gtjatofdmc.html


<!-- 参考信息 -->