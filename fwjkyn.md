代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.snrcjt.cn/gtsnrkqjjc.html

[L04] 设置超时
来源：http://hz.yueranfly.top/gtmlzlboyo.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhongyouzk.top/gtjkiafmwd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.wangdashe.top/gtrhoavduk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.pengpengdd.cyou/gtsnaxcwmt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.quarkkingdee.top/gtokmrtfws.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.pengpengdd.cyou/gtoflmkekh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.pycfn.com/gtgjzqunhv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.52xcode.cn/gtcuwvxjsv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.pycfn.com/gtbunhgbxs.html

[L05] 上传文件（multipart）
来源：http://hz.gotoacloud.top/gtmhsudtut.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.meibo888.top/gtqizdriyv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.tanke756.top/gtrtzhevlj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shangyingyoupin.top/gtgyahgxxw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sweek.top/gtxgdjmcqh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hysaishi.cn/gtrhwlhjar.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yongpay.top/gtutcigwje.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sxryk.cn/gtzpypdoef.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.havefunace.top/gtbyfqtmyi.html

[L06] 解析响应为 JSON
来源：http://hz.iojbl.cn/gtpxlfzxyo.html

Py:   resp.json()
来源：http://hz.shanyushiyangkeji.top/gtjsbtpywe.html

PHP:  json_decode($body, true);
来源：http://hz.redwolf501.top/gtkfjpsxba.html

JS:   await resp.json()
来源：http://hz.hysaishi.cn/gtsmzqhvwj.html

TS:   await resp.json()
来源：http://hz.jinyuanbaomall.cn/gtxcjxkyyj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhongyouzk.top/gtxcypewhy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.bjfxy.top/gtxsnpwizo.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shanyushiyangkeji.top/gtfbbvupci.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.vqdsnc.cn/gtiinwdpvp.html

[L07] 处理 HTTP 状态码
来源：http://hz.wangdashe.top/gtdihizask.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gotoacloud.top/gtiuhcwjxk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhijiandao.cn/gtbfqjqmxk.html

JS:   resp.ok;  resp.status
来源：http://hz.bjfxy.top/gtazzlmqxs.html

TS:   resp.ok;  resp.status
来源：http://hz.chenjidiqi.icu/gtdyabafws.html

Java: resp.statusCode()
来源：http://hz.jiagoushi.top/gtvurkhlmx.html

Go:   resp.StatusCode
来源：http://hz.zhixingplan.top/gtcmvcljjv.html

Ruby: resp.code.to_i
来源：http://hz.tanke756.top/gtpfhwliyx.html

C#:   (int)resp.StatusCode
来源：http://hz.ydjk.org.cn/gthyxofaey.html

[L08] 并发请求多个地址
来源：http://hz.zycfv.cn/gtjstkpagm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.daria6918.cn/gtkjbgvmcb.html

PHP:  curl_multi_init() 系列
来源：http://hz.hnxiangtu.top/gtukpvirse.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aizwys.cn/gtktqfcknf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj202588.top/gtdduhbrlr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yuxming.cn/gtqujfafcv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xinyue.icu/gtfflkkwmm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.svipenyu.cn/gtcfnbgsnw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.daxiang520.top/gtpjfdqkuf.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtdtiqqmnl.html

M. 命令行 / 进程 / 环境
来源：http://hz.316326.xyz/gtsfwodqsw.html

================================================================================
来源：http://hz.yj20258888.top/gtbvruzbee.html

[M01] 读取命令行参数
来源：http://hz.jqgfzy.top/gteiepzkmb.html

Py:   sys.argv[1:]
来源：http://hz.redwolf501.top/gtwgesjavw.html

PHP:  $argv;  $argc;
来源：http://hz.ybcxt.top/gtwoaqplsg.html

JS:   process.argv.slice(2)
来源：http://hz.guowangkeji.top/gtvxadlssv.html

TS:   process.argv.slice(2)
来源：http://hz.aibaodan.cn/gttxymqpbw.html

Java: args 数组（main 方法参数）
来源：http://hz.jinqigufen.top/gtcrihzpyx.html

Go:   os.Args[1:]
来源：http://hz.jinyuanbaomall.cn/gtwwqimsjq.html

Ruby: ARGV
来源：http://hz.jinqigufen.top/gtmojbqhdy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sufxvd.cn/gtrviwzmkd.html

[M02] 读取环境变量
来源：http://hz.daxiang520.top/gtxzqecpgg.html

Py:   os.environ.get("HOME")
来源：http://hz.316326.xyz/gtfdtzyalt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yj202588.top/gteydxgflo.html

JS:   process.env.HOME
来源：http://hz.xingfuxueyuan.xyz/gtudmkvqxx.html

TS:   process.env.HOME
来源：http://hz.cheryme.top/gtonhsyxgs.html

Java: System.getenv("HOME")
来源：http://hz.gaohongyu789.top/gtiftpnmen.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sxryk.cn/gtgmrqoltx.html

Ruby: ENV["HOME"]
来源：http://hz.kuanghao11.cn/gtghwpnrwe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.feifeiyinyue.top/gtfsvbkhrn.html

[M03] 执行外部命令
来源：http://hz.ivvv.top/gtjnbxfcgs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuxming.cn/gtyqtlwrbu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hammf.cn/gtjetwlkju.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yongpay.top/gtgssomtrs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zycfv.cn/gtcpwqmxdg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhaomingkeji.xyz/gthscxvroh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cdnleiting.top/gtgqjjbcnq.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hammf.cn/gtwlwpmuzh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yongpay.top/gtrrjilgpz.html

[M04] 获取当前工作目录
来源：http://hz.zhixingplan.top/gtwekoajkm.html

Py:   os.getcwd()
来源：http://hz.sysykeji.top/gtqkbvgguk.html

PHP:  getcwd();
来源：http://hz.yangfankeji.com/gtpjgciyst.html

JS:   process.cwd()
来源：http://hz.zhaomingkeji.xyz/gtotuhykib.html

TS:   process.cwd()
来源：http://hz.guowangkeji.top/gtxzlpvchu.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.quarkkingdee.top/gtpgrgvfqy.html

Go:   os.Getwd()
来源：http://hz.zhengqikj.top/gtkiemtjdr.html

Ruby: Dir.pwd
来源：http://hz.zhaomingkeji.xyz/gtcqcqzoof.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhaomingkeji.xyz/gteiruywvy.html

[M05] 设置退出码
来源：http://hz.zdqjudy.top/gttnzehfyj.html

Py:   sys.exit(1)
来源：http://hz.shuidangran.top/gtluanvpyj.html

PHP:  exit(1);
来源：http://hz.chenzaomai.com/gthemozkll.html

JS:   process.exit(1)
来源：http://hz.shangyingyoupin.top/gtthwgtcxg.html

TS:   process.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtqoctetbr.html

Java: System.exit(1)
来源：http://hz.xylfe.cn/gtvbyossxw.html

Go:   os.Exit(1)
来源：http://hz.hfpthk.cn/gtuqzzawgw.html

Ruby: exit 1
来源：http://hz.cucudq.cn/gtalqjcoma.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinyuanbaomall.cn/gtxvsxrdhd.html

[M06] 向标准错误输出
来源：http://hz.zhiwuduotai.top/gtnytghyfj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shanyushiyangtech.top/gthgelknls.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gzhubu.top/gttcxbspcb.html

JS:   console.error("err")
来源：http://hz.nanxinkj.top/gtemgnuywm.html

TS:   console.error("err")
来源：http://hz.yueranfly.top/gtrrbwnqck.html

Java: System.err.println("err")
来源：http://hz.jinqigfzy.top/gtayjhurra.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sysykeji.top/gtvirtgcbq.html

Ruby: warn "err"
来源：http://hz.jqgfzy.top/gtvexpjtpx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.andypj.xyz/gtxzxhiwah.html

[M07] 判断是否为主入口
来源：http://hz.daria6918.cn/gttrrhdgze.html

Py:   if __name__ == "__main__":
来源：http://hz.zhiwuduotai.top/gtanjccfaa.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shanyushiyangtech.top/gtpavgfkkd.html

JS:   require.main === module
来源：http://hz.316326.xyz/gtikepkxrq.html

TS:   require.main === module
来源：http://hz.xziqi.cn/gtbljtvzgb.html

Java: public static void main(String[] args)
来源：http://hz.52xcode.cn/gtuwriahwy.html

Go:   func main()
来源：http://hz.xingfuxueyuan.xyz/gtrbrxhram.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhengqikj.top/gtkduavmjg.html

C#:   static void Main(string[] args)
来源：http://hz.yj20258888.top/gtfxkftfmx.html

[M08] 获取系统与运行时信息
来源：http://hz.xuetiantiany.cn/gtdwxhxpdd.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhijiandao.cn/gtneoufkzo.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jqgfzy.top/gtlvefsoof.html

JS:   process.platform;  process.version
来源：http://hz.vqdsnc.cn/gtwogsswvi.html

TS:   process.platform;  process.version
来源：http://hz.shuidangran.top/gtsfkajbul.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.9152youxi.cn/gtxvdvtjvh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.haohaochexian.top/gtbylwhmfz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.wangdashe.top/gtaajuevwd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj20258.top/gtlpiursrp.html

================================================================================
来源：http://hz.yanxiufei.cn/gtlwqwitnl.html

N. 数据结构与算法
来源：http://hz.jinqigfzy.top/gtdgsnmhuq.html

================================================================================
来源：http://hz.gogol.net.cn/gtepwmwwws.html

[N01] 二分查找（有序数组）
来源：http://hz.zycfv.cn/gttkcmmrwq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zdqjudy.top/gtuyfuwqcm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hongshengwenyu.top/gtmuzyrmqo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.svipenyu.cn/gtyznpzgut.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.quarkkingdee.top/gtwiqzzjuc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.sufxvd.cn/gtbtebhuys.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhixingplan.top/gtmjnvesmn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xingfuxueyuan.xyz/gtblkjdgpy.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.c1oappe.top/gttvmurjys.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.sxryk.cn/gtdvredcgp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhongyouzk.top/gtbsjpjrht.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shuidangran.top/gtbwbhesez.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fzhhl.top/gtaiysxrba.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxuanxn.top/gtccrhxces.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhijiandao.cn/gtmuwqyulk.html

Go:   slices.Sort(arr)
来源：http://hz.zdqjudy.top/gtlvwwumhy.html

Ruby: arr.sort
来源：http://hz.chenlongwang.top/gtgthziwoa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shanyushiyangkeji.top/gtyjeakqib.html

[N03] 快速排序（分治示例）
来源：http://hz.sufxvd.cn/gtaygynlev.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jqgufenzy.top/gtxxboxzgx.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yonumen.top/gtwtpjrhut.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.smart0.xyz/gtqcravwwu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gaohongyu789.top/gtjeonvvhc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cheryme.top/gtrjxlbbkv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhongyouzk.top/gtcgllpcgx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jqgfzy.top/gthdhvonpt.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.c1oappe.top/gttkhavtzi.html

[N04] 斐波那契数列
来源：http://hz.guannengcc.top/gtklxrnfcd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.gogol.net.cn/gtiofvkhrk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yueranfly.top/gtsbmtodbk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuanzhike.top/gtfhqxkauy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ehwqpu.com/gtzilyiiqb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.haohaochexian.top/gtjyhzraax.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinqigfzy.top/gtsoicovkq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.guowangkeji.top/gtblthnpja.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.wangdashe.top/gtchvnphjh.html

[N05] 最大公约数
来源：http://hz.smart0.xyz/gtbihusvuc.html

Py:   math.gcd(a, b)
来源：http://hz.shanyushiyangkeji.top/gtywgywayp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.316326.xyz/gtupcwqtjh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shzxlz.cn/gtcsaaalna.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.kuanghao11.cn/gtpmslfefh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yj202588.top/gtmlpgbuyp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.andypj.xyz/gtyyozbhvb.html

Ruby: a.gcd(b)
来源：http://hz.ivvv.top/gtzblyarjz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cqqwz.cn/gtcjjmihzo.html

[N06] 判断回文字符串
来源：http://hz.xuanzx.com/gttbdggqla.html

Py:   s == s[::-1]
来源：http://hz.mhx1999.top/gtpzjfjren.html

PHP:  $s === strrev($s);
来源：http://hz.hnqzz.top/gtrbcniucu.html

JS:   s === [...s].reverse().join("")
来源：http://hz.wangshuangyany.cn/gtgaoqboqy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ivvv.top/gtzoobokqa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shzxlz.cn/gtriqmjssr.html

Go:   // 双指针从两端比较
来源：http://hz.xinyue.icu/gtikecxyds.html

Ruby: s == s.reverse
来源：http://hz.zhoulong.xyz/gtoiqbrysu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.pycfn.com/gtqlahfovo.html

[N07] 两数之和（返回下标）
来源：http://hz.316326.xyz/gthyljjbim.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gzhubu.top/gtcufkktwf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gaohongyu789.top/gtkfteyjdp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinqigufen.top/gtufbkodbj.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinqigfzy.top/gtavqotfsl.html

Java: // 手写 HashMap
来源：http://hz.hfpthk.cn/gtxanpcnbw.html

Go:   // 手写 map[int]int
来源：http://hz.xylfe.cn/gtatwttrwy.html

Ruby: // 手写 Hash
来源：http://hz.yuxming.cn/gtmvwzbtby.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.iojbl.cn/gtvbjszdzj.html

[N08] 生成全排列
来源：http://hz.chenlongwang.top/gtsxyqeqjp.html

Py:   itertools.permutations(arr)
来源：http://hz.iojbl.cn/gtzxjrgett.html

PHP:  // 手写递归交换
来源：http://hz.smart0.xyz/gtavosuocx.html

JS:   // 手写回溯递归
来源：http://hz.mhx1999.top/gtuqpiokwv.html

TS:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtaujkrtnd.html

Java: // 手写回溯递归
来源：http://hz.dashuyun.cn/gtiqivtrgw.html

Go:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtzbvydopk.html

Ruby: arr.permutation.to_a
来源：http://hz.guowangkeji.top/gtbnwohgqw.html

C#:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtbebvzqlh.html

[N09] 栈与队列
来源：http://hz.iojbl.cn/gtyjxgtvxf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.316326.xyz/gtqbnyocnf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.smart0.xyz/gtogvsryik.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhongyouzk.top/gtnrfzvbks.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yvedp.cn/gtsukltiog.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.guannengcc.top/gtqpgznchk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sysykeji.top/gtcarduxbh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.gogol.net.cn/gtmtnfjqbz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.sweek.top/gtozoyagvt.html

[N10] 链表节点定义
来源：http://hz.shanyushiyangkeji.top/gtcnrbanez.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jqgufenzy.top/gtdpxdezfk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sufxvd.cn/gtrbpnhtlm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yonumen.top/gtmfuxylzt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cdnleiting.top/gtwqqdejtq.html

Java: class Node { int v; Node next; }
来源：http://hz.0kj1m.cn/gtkimbcudy.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.kuanghao11.cn/gtxspdrcbs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinqigufen.top/gtyaideukp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xuetiantiany.cn/gtzdqgbuxq.html

[N11] 二叉树中序遍历
来源：http://hz.xuanzx.com/gthlwjaqwv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cheryme.top/gtxhpnoomu.html

PHP:  // 手写递归函数
来源：http://hz.yuxming.cn/gtxyujgvby.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yvedp.cn/gtiushllyr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gaohongyu789.top/gtriupvpux.html

Java: // 手写递归
来源：http://hz.feifeiyinyue.top/gtstmmhlxa.html

Go:   // 手写递归
来源：http://hz.tian-w.cn/gtnstzmhev.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.feifeiyinyue.top/gtxbbqqoit.html

C#:   // 手写递归
来源：http://hz.chenlongwang.top/gtbkjjgbwd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ppjwa.cn/gtgkiziekx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.guowangkeji.top/gtzprcyvap.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jiagoushi.top/gtdguwminp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.guowangkeji.top/gtjwjtmbnu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.c1oappe.top/gtzvgrxudd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.vqdsnc.cn/gtwsakxoec.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hnqzz.top/gtxlbjnvmk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yj202588.top/gtbshdieis.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hongshengwenyu.top/gtrchwwiie.html

================================================================================
来源：http://hz.yj20258.top/gtzotuiasu.html

O. 并发与异步
来源：http://hz.yj20258.top/gtcncvpbny.html

================================================================================
来源：http://hz.svipenyu.cn/gtojqwpfxd.html

[O01] 启动一个线程
来源：http://hz.iojbl.cn/gtubsxgelt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shuidangran.top/gtzjlsymqm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhijiandao.cn/gtlkmpjumj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ydzc1.top/gthdenierv.html

TS:   // 同 JS
来源：http://hz.meibo888.top/gttbawcxeh.html

Java: new Thread(() -> f()).start()
来源：http://hz.ybcxt.top/gtkxpnwrmw.html

Go:   go f()
来源：http://hz.c1oappe.top/gtxfuzihdl.html

Ruby: Thread.new { f }
来源：http://hz.zhongyouzk.top/gthjowxstm.html

C#:   Task.Run(() => F());
来源：http://hz.yvedp.cn/gtkuqthxqr.html

[O02] 使用线程池
来源：http://hz.aibaodan.cn/gtxfcnmdhi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.gaohongyu789.top/gtasxycvof.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.kuanghao11.cn/gtsluuyfkc.html

JS:   // worker_threads 线程池
来源：http://hz.feifeiyinyue.top/gtvwkbgwbs.html

TS:   // worker_threads 线程池
来源：http://hz.havefunace.top/gtzhibdval.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ybcxt.top/gtxnuthumf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhengqikj.top/gtwoxypnrx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shzxlz.cn/gtrzgdtsbw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shangyingyoupin.top/gtqsjbmkxl.html

[O03] 加锁保护共享数据
来源：http://hz.yangfankeji.com/gttnifqbfq.html

Py:   with lock: shared += 1
来源：http://hz.nwbrower.top/gtpriggmwl.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhaomingkeji.xyz/gtloepiest.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hnxiangtu.top/gtoeliblxo.html

TS:   // 同 JS
来源：http://hz.sufxvd.cn/gtasuauczw.html

Java: synchronized (this) { shared++; }
来源：http://hz.hammf.cn/gtxgivalcw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.chenzaomai.com/gtulssmtzk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jqgufenzy.top/gtffztbqnv.html

C#:   lock (gate) { shared++; }
来源：http://hz.smart0.xyz/gtapknucet.html

[O04] 定义异步函数并等待
来源：http://hz.wangshuangyany.cn/gtjnqtppyx.html

Py:   async def f():⏎    await g()
来源：http://hz.zycfv.cn/gtpfjrujuq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jiagoushi.top/gtbqvyehht.html

JS:   async function f() { await g(); }
来源：http://hz.0kj1m.cn/gtkopkwwsk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.guannengcc.top/gtgksllizr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhiwuduotai.top/gtozlmgvzs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.vqdsnc.cn/gtmhtfixcq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jiagoushi.top/gtfburmnfn.html

C#:   async Task F() { await G(); }
来源：http://hz.jyoumei.cn/gtidxtbayv.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhijiandao.cn/gtdixqdbxg.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinqigfzy.top/gtuklfqtmz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.nwbrower.top/gtjcwnkygi.html

JS:   await Promise.all(tasks)
来源：http://hz.snrcjt.cn/gtswodzmck.html

TS:   await Promise.all(tasks)
来源：http://hz.jinqigfzy.top/gtqqmpxwje.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cdnleiting.top/gttkwgrdsn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hongshengwenyu.top/gtimqyvaqa.html

Ruby: threads.map(&:join)
来源：http://hz.cucudq.cn/gtjzumcirz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.meibo888.top/gtybxvngpi.html

[O06] 使用进程池
来源：http://hz.mhx1999.top/gtgtwqpmvn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.9152youxi.cn/gtaozffrya.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ehwqpu.com/gtbduhsukw.html

JS:   // child_process / cluster 模块
来源：http://hz.mhx1999.top/gtdjwfmzom.html

TS:   // child_process / cluster 模块
来源：http://hz.gotoacloud.top/gtusvsrcux.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.0kj1m.cn/gtzgfvkzfx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hnxiangtu.top/gtbfvjeekd.html

Ruby: // fork 块
来源：http://hz.nanxinkj.top/gtrgpmejgf.html

C#:   Parallel.For
来源：http://hz.zdqjudy.top/gthjkmymme.html

================================================================================
来源：http://hz.gogol.net.cn/gtjhiydgtq.html

P. 常用工具函数
来源：http://hz.ydzc1.top/gtuhdrwsrx.html

================================================================================
来源：http://hz.yvedp.cn/gtomvvjfzs.html

[P01] 生成 UUID
来源：http://hz.zhongyouzk.top/gtgadubvqj.html

Py:   str(uuid.uuid4())
来源：http://hz.tianlin.xyz/gtfyvybksg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhaomingkeji.xyz/gtepbjjbbi.html

JS:   crypto.randomUUID()
来源：http://hz.kuanghao11.cn/gtjqmunofk.html

TS:   crypto.randomUUID()
来源：http://hz.smart0.xyz/gtrddrruux.html

Java: UUID.randomUUID().toString()
来源：http://hz.yj20258888.top/gtdvsvpawl.html

Go:   // 用 github.com/google/uuid
来源：http://hz.nwbrower.top/gtflizdgxy.html

Ruby: SecureRandom.uuid
来源：http://hz.zhixingplan.top/gtdpzjuogb.html


<!-- 参考信息 -->