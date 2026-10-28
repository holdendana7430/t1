代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenzaomai.com/gtepcgnavh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cashguo.top/gtbcxfianj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.redwolf501.top/gtdxfjpmro.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gogol.net.cn/gtaeorcfat.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.chenzaomai.com/gtmxjypxvc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sysykeji.top/gtmsbkogfe.html

[L05] 上传文件（multipart）
来源：http://hz.yangfankeji.com/gtwodkxeyh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.tian-w.cn/gtaeacbtje.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.316326.xyz/gtrzlamiat.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cucudq.cn/gtwmajgzvl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhixingplan.top/gturbhgxsk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.316326.xyz/gtjpwvumhw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yonumen.top/gtdxsdnxex.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.wangdashe.top/gtjeovzftu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.fengsongda.top/gtutxdobxb.html

[L06] 解析响应为 JSON
来源：http://hz.aibaodan.cn/gturnaujsl.html

Py:   resp.json()
来源：http://hz.xuanzx.com/gtoqvbuasl.html

PHP:  json_decode($body, true);
来源：http://hz.cqqwz.cn/gtrnasnoki.html

JS:   await resp.json()
来源：http://hz.nwbrower.top/gtjimycqxi.html

TS:   await resp.json()
来源：http://hz.cqqwz.cn/gtbibjicgh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yuxming.cn/gtxyxjwpin.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xinyue.icu/gtoxuklyoc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xziqi.cn/gtsgrivhso.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hnxiangtu.top/gtucuepsqf.html

[L07] 处理 HTTP 状态码
来源：http://hz.ydzc1.top/gtukbnrkjj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gogol.net.cn/gtkxzytkut.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.kuanghao11.cn/gtylaeokep.html

JS:   resp.ok;  resp.status
来源：http://hz.hammf.cn/gtxkyynqpf.html

TS:   resp.ok;  resp.status
来源：http://hz.chenlongwang.top/gtpyemskrg.html

Java: resp.statusCode()
来源：http://hz.quarkkingdee.top/gtwsbdwqwd.html

Go:   resp.StatusCode
来源：http://hz.guannengcc.top/gtnpjtnqeq.html

Ruby: resp.code.to_i
来源：http://hz.gotoacloud.top/gtmtuzgovh.html

C#:   (int)resp.StatusCode
来源：http://hz.meibo888.top/gtbznafyav.html

[L08] 并发请求多个地址
来源：http://hz.yuanzhike.top/gtfbomhxfi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj20258.top/gtafashmfn.html

PHP:  curl_multi_init() 系列
来源：http://hz.jyoumei.cn/gtfaygofql.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydjk.org.cn/gtcrqmryho.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shangyingyoupin.top/gtcxeipykw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sufxvd.cn/gtdasodgoy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.0kj1m.cn/gtgsqndpqj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.chenlongwang.top/gtbevibmjd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.tian-w.cn/gtyualjmsy.html

================================================================================
来源：http://hz.zycfv.cn/gtubavjyqh.html

M. 命令行 / 进程 / 环境
来源：http://hz.kuanghao11.cn/gtbbofqcic.html

================================================================================
来源：http://hz.yj20258.top/gtnllgggkx.html

[M01] 读取命令行参数
来源：http://hz.redwolf501.top/gtecamtiuo.html

Py:   sys.argv[1:]
来源：http://hz.jinqigufen.top/gtumwpldjz.html

PHP:  $argv;  $argc;
来源：http://hz.pycfn.com/gtjbhnrxtt.html

JS:   process.argv.slice(2)
来源：http://hz.yuxming.cn/gtbcqaoknf.html

TS:   process.argv.slice(2)
来源：http://hz.c1oappe.top/gtyzrgeoru.html

Java: args 数组（main 方法参数）
来源：http://hz.gaohongyu789.top/gtqfikbtpt.html

Go:   os.Args[1:]
来源：http://hz.zdqjudy.top/gtykpnfwvi.html

Ruby: ARGV
来源：http://hz.zhongyouzk.top/gtrkzimlbd.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hywenlv.cn/gtbgsmicve.html

[M02] 读取环境变量
来源：http://hz.redwolf501.top/gtjialzlli.html

Py:   os.environ.get("HOME")
来源：http://hz.jiagoushi.top/gthqnbfhqw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.daria6918.cn/gtcjzgzohj.html

JS:   process.env.HOME
来源：http://hz.zhixingplan.top/gtwxqetspz.html

TS:   process.env.HOME
来源：http://hz.wangdashe.top/gthusqetpr.html

Java: System.getenv("HOME")
来源：http://hz.sufxvd.cn/gtflklmdyf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.dashuyun.cn/gtzpckhueb.html

Ruby: ENV["HOME"]
来源：http://hz.zhengqikj.top/gtabvemtfh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xingfuxueyuan.xyz/gtnlaascyo.html

[M03] 执行外部命令
来源：http://hz.chenjidiqi.icu/gtugqqbbty.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.pycfn.com/gtbgatxogd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jlsjyb.cn/gtrzaxmltn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgfzy.top/gtumqecmpq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.daria6918.cn/gtyunvkqsn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.kuanghao11.cn/gtbsyzijds.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.guannengcc.top/gtfbgifwsf.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yj202588.top/gtjrorvzzi.html

C#:   Process.Start("ls", "-l");
来源：http://hz.chenjidiqi.icu/gtdpfkwnwx.html

[M04] 获取当前工作目录
来源：http://hz.birdmap.top/gtulklmlex.html

Py:   os.getcwd()
来源：http://hz.xuanzx.com/gtqokxmtya.html

PHP:  getcwd();
来源：http://hz.xziqi.cn/gtisjdbrdh.html

JS:   process.cwd()
来源：http://hz.cashguo.top/gtsxyyczyj.html

TS:   process.cwd()
来源：http://hz.ydzc1.top/gtfnddhtdt.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.svipenyu.cn/gthueusybw.html

Go:   os.Getwd()
来源：http://hz.jqgfzy.top/gthkmyexcz.html

Ruby: Dir.pwd
来源：http://hz.dashuyun.cn/gtkofpamxe.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.bjfxy.top/gtgbdhotuw.html

[M05] 设置退出码
来源：http://hz.sweek.top/gtidayhrqt.html

Py:   sys.exit(1)
来源：http://hz.yonumen.top/gtfaynxzwh.html

PHP:  exit(1);
来源：http://hz.zdqjudy.top/gtgxudkcop.html

JS:   process.exit(1)
来源：http://hz.jinqigufen.top/gtxdvrhfih.html

TS:   process.exit(1)
来源：http://hz.nanxinkj.top/gtvftknpqo.html

Java: System.exit(1)
来源：http://hz.0kj1m.cn/gtiunccvfg.html

Go:   os.Exit(1)
来源：http://hz.jiagoushi.top/gtmbpucfbi.html

Ruby: exit 1
来源：http://hz.yongpay.top/gtbwnefhfu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yonumen.top/gtthjhrioi.html

[M06] 向标准错误输出
来源：http://hz.ydjk.org.cn/gtdwcaeyir.html

Py:   print("err", file=sys.stderr)
来源：http://hz.vqdsnc.cn/gtozoaalcg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yueranfly.top/gtroqowlrv.html

JS:   console.error("err")
来源：http://hz.birdmap.top/gtqzeyjrfo.html

TS:   console.error("err")
来源：http://hz.hongshengwenyu.top/gttyygcxud.html

Java: System.err.println("err")
来源：http://hz.chenzaomai.com/gtckyzlnps.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xylfe.cn/gtsuyaljjf.html

Ruby: warn "err"
来源：http://hz.haohaochexian.top/gttgvmcowf.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hysaishi.cn/gtozgspibt.html

[M07] 判断是否为主入口
来源：http://hz.yj202588.top/gtwwrdivzg.html

Py:   if __name__ == "__main__":
来源：http://hz.sufxvd.cn/gtdcainiiz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.dashuyun.cn/gtcqvtuguh.html

JS:   require.main === module
来源：http://hz.zhiwuduotai.top/gtjeqszfrh.html

TS:   require.main === module
来源：http://hz.zhiwuduotai.top/gtphvnnxum.html

Java: public static void main(String[] args)
来源：http://hz.tanke756.top/gtsggfvocw.html

Go:   func main()
来源：http://hz.xziqi.cn/gtjpjpcomi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xingfuxueyuan.xyz/gthheaywly.html

C#:   static void Main(string[] args)
来源：http://hz.hywenlv.cn/gtxdumhiad.html

[M08] 获取系统与运行时信息
来源：http://hz.tian-w.cn/gtdwbxsimb.html

Py:   platform.system();  platform.python_version()
来源：http://hz.aizwys.cn/gtfyjxooyr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.dashuyun.cn/gtvmkrgwhr.html

JS:   process.platform;  process.version
来源：http://hz.ydzc1.top/gtppozjelc.html

TS:   process.platform;  process.version
来源：http://hz.chenjidiqi.icu/gtaiisvmrp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jiagoushi.top/gtbicqoobh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.tanke756.top/gtumsugmvp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinyuanbaomall.cn/gtvvtijdfj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.haohaochexian.top/gtlnjuexma.html

================================================================================
来源：http://hz.gogol.net.cn/gtasmzehka.html

N. 数据结构与算法
来源：http://hz.yonumen.top/gtromuypgg.html

================================================================================
来源：http://hz.meibo888.top/gtealcdiye.html

[N01] 二分查找（有序数组）
来源：http://hz.yj20258888.top/gtqyyyxjsi.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ydzc1.top/gtnedavpwv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cashguo.top/gtwgasjktf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yuanzhike.top/gtyzkjtmov.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinghuilouyu.cn/gtgmiblnwb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.nanxuanxn.top/gtnpxdhqmm.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.dianchejie.cn/gtalfsffqe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jqgufenzy.top/gtjofxyndf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gaohongyu789.top/gthfcygzmd.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xuetiantiany.cn/gtrcehgscy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.guowangkeji.top/gtzbhpzmsd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinqigufen.top/gtrlzlmsve.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xingfuxueyuan.xyz/gtikobuhvx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jiagoushi.top/gtckikioii.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cheryme.top/gtfjibhzue.html

Go:   slices.Sort(arr)
来源：http://hz.hfpthk.cn/gtxbnalnxe.html

Ruby: arr.sort
来源：http://hz.cashguo.top/gtgxfljprl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.52xcode.cn/gtabbtubvh.html

[N03] 快速排序（分治示例）
来源：http://hz.zhaomingkeji.xyz/gtydrzcrno.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.meibo888.top/gtaxrhhqgw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tianlin.xyz/gtnghzdkoh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tian-w.cn/gtvhoxokyv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sweek.top/gtepszfwfr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.0kj1m.cn/gtynwxezth.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.bjfxy.top/gtjbgepbby.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.wangshuangyany.cn/gteruxalbb.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.birdmap.top/gtwuuyfjlf.html

[N04] 斐波那契数列
来源：http://hz.fzhhl.top/gtrtgobucc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ybcxt.top/gtbipaqdmp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yonumen.top/gtsoyqfdyh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ybcxt.top/gtxjgozbbo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ehwqpu.com/gtxudodcfl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.dashuyun.cn/gtkfzemufv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xinyue.icu/gtxxorgnrz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.andypj.xyz/gtyrpykink.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenjidiqi.icu/gtdvvaypdt.html

[N05] 最大公约数
来源：http://hz.gogol.net.cn/gtfesomriy.html

Py:   math.gcd(a, b)
来源：http://hz.andypj.xyz/gtnmikrqxn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.nanxuanxn.top/gthyrmxthl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jlsjyb.cn/gtcqvklzpd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jianghu66.top/gtysbbivwx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gaohongyu789.top/gtvzrdkekc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yangfankeji.com/gtkkyfhgpr.html

Ruby: a.gcd(b)
来源：http://hz.sufxvd.cn/gtyiajaohj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gotoacloud.top/gtytupuuti.html

[N06] 判断回文字符串
来源：http://hz.zdqjudy.top/gtrzdngozr.html

Py:   s == s[::-1]
来源：http://hz.jyoumei.cn/gtekgqzxyu.html

PHP:  $s === strrev($s);
来源：http://hz.meibo888.top/gtmjoryxyr.html

JS:   s === [...s].reverse().join("")
来源：http://hz.kuanghao11.cn/gturzqhfgy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtuzxwjvxe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinghuilouyu.cn/gtavztvfnt.html

Go:   // 双指针从两端比较
来源：http://hz.zhoulong.xyz/gtagbgmpui.html

Ruby: s == s.reverse
来源：http://hz.aizwys.cn/gthwosqkfh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shzxlz.cn/gtryaybfgm.html

[N07] 两数之和（返回下标）
来源：http://hz.ivvv.top/gtsvhergjz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gaohongyu789.top/gtmlworbis.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.smart0.xyz/gtmgpdxsvh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jiagoushi.top/gttyxjpisf.html

TS:   // 手写 Map<string, number>
来源：http://hz.chenzaomai.com/gtyjfrsfln.html

Java: // 手写 HashMap
来源：http://hz.aizwys.cn/gtuotvefhe.html

Go:   // 手写 map[int]int
来源：http://hz.yonumen.top/gtvmsfmpll.html

Ruby: // 手写 Hash
来源：http://hz.gaohongyu789.top/gtcqmrfuje.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gzhubu.top/gtcrpqqgmr.html

[N08] 生成全排列
来源：http://hz.aizwys.cn/gtzbtpjcuw.html

Py:   itertools.permutations(arr)
来源：http://hz.ydzc1.top/gtekvpdvei.html

PHP:  // 手写递归交换
来源：http://hz.hnqzz.top/gtkvaewymj.html

JS:   // 手写回溯递归
来源：http://hz.fengsongda.top/gturhanbvr.html

TS:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtndvcqrxk.html

Java: // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtzuputwws.html

Go:   // 手写回溯递归
来源：http://hz.xziqi.cn/gtdtndwwrr.html

Ruby: arr.permutation.to_a
来源：http://hz.shuidangran.top/gtexdzzzgn.html

C#:   // 手写回溯递归
来源：http://hz.meibo888.top/gthnrrfrhb.html

[N09] 栈与队列
来源：http://hz.nanxuanxn.top/gtxwfgvkar.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.mhx1999.top/gteocdbnnk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ivvv.top/gtlefguseu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yueranfly.top/gtdjhstnai.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.dianchejie.cn/gtpaabctrd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.havefunace.top/gtxexwxotw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ydjk.org.cn/gtydnxbrwc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.feifeiyinyue.top/gtaegtmjhf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jiagoushi.top/gtjoyxvjnl.html

[N10] 链表节点定义
来源：http://hz.gogol.net.cn/gtfgxexbmu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jqgfzy.top/gtgenxqobv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zycfv.cn/gtygixkttt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.vqdsnc.cn/gtwmwgfwnz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hnxiangtu.top/gtiyulnnym.html

Java: class Node { int v; Node next; }
来源：http://hz.shuidangran.top/gtlfexbavt.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.0kj1m.cn/gtllqfrzfo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.tianlin.xyz/gtcyqazrme.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jqgfzy.top/gtirotibus.html

[N11] 二叉树中序遍历
来源：http://hz.dashuyun.cn/gtixregffc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yangfankeji.com/gtrqaxkjdo.html

PHP:  // 手写递归函数
来源：http://hz.wangdashe.top/gtinjgduhy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.haohaochexian.top/gtoovmoerr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shanyushiyangtech.top/gtuipyluep.html

Java: // 手写递归
来源：http://hz.hysaishi.cn/gtrsxiqetk.html

Go:   // 手写递归
来源：http://hz.yj20258888.top/gtogefdaeg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.dianchejie.cn/gtrrtnghfq.html

C#:   // 手写递归
来源：http://hz.yj202588.top/gtugqfucvw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gaohongyu789.top/gtilztsiur.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hnxiangtu.top/gtksqjbkkt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhengqikj.top/gteughtxdg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aizwys.cn/gtelalkzyq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gogol.net.cn/gtldiztnwn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258.top/gthjwnmbsy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sweek.top/gtrixkjfxk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zdqjudy.top/gttgnugsxn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinyuanbaomall.cn/gtzpsdxdaq.html

================================================================================
来源：http://hz.zycfv.cn/gtbgnxbfyk.html

O. 并发与异步
来源：http://hz.hysaishi.cn/gtlakmqteb.html

================================================================================
来源：http://hz.zhengqikj.top/gtgitgtaqv.html

[O01] 启动一个线程
来源：http://hz.chenzaomai.com/gtdqmnnnqk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.0kj1m.cn/gthkuezdef.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yuxming.cn/gtzipkknaq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jqgufenzy.top/gtaocotoms.html

TS:   // 同 JS
来源：http://hz.jyoumei.cn/gtqgqcixyx.html

Java: new Thread(() -> f()).start()
来源：http://hz.zdqjudy.top/gtobqomcof.html

Go:   go f()
来源：http://hz.yanxiufei.cn/gtauzqvwrp.html

Ruby: Thread.new { f }
来源：http://hz.yuanzhike.top/gtrojmqmvu.html

C#:   Task.Run(() => F());
来源：http://hz.aizwys.cn/gtkotzdxrr.html

[O02] 使用线程池
来源：http://hz.yvedp.cn/gtqhoqnolj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.daria6918.cn/gtishnzyef.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhaomingkeji.xyz/gteylxirwb.html

JS:   // worker_threads 线程池
来源：http://hz.yanxiufei.cn/gtuonqxeab.html

TS:   // worker_threads 线程池
来源：http://hz.havefunace.top/gtwqpzadxv.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yanxiufei.cn/gtohksrmup.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhixingplan.top/gtrxlbigci.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.daxiang520.top/gtpvaflgzo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xingfuxueyuan.xyz/gtnlazmcir.html

[O03] 加锁保护共享数据
来源：http://hz.gotoacloud.top/gtngignirl.html

Py:   with lock: shared += 1
来源：http://hz.52xcode.cn/gtcujgysek.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.dashuyun.cn/gtpzdezanh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zdqjudy.top/gtsdshnxcw.html

TS:   // 同 JS
来源：http://hz.jqgfzy.top/gtqqcootlo.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhiwuduotai.top/gtcgzheave.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.nanxuanxn.top/gtgklcccdv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xziqi.cn/gtmsoilqua.html

C#:   lock (gate) { shared++; }
来源：http://hz.xylfe.cn/gtqvjncuux.html

[O04] 定义异步函数并等待
来源：http://hz.xziqi.cn/gtszdpchse.html

Py:   async def f():⏎    await g()
来源：http://hz.gotoacloud.top/gtsmlpmjgs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.bjfxy.top/gtzsozwbyd.html

JS:   async function f() { await g(); }
来源：http://hz.tianlin.xyz/gtsnwqozqm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.c1oappe.top/gtxwpvcjev.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xylfe.cn/gtwgffsuvx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cdnleiting.top/gtcnzgprun.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jiagoushi.top/gtewbsdnca.html

C#:   async Task F() { await G(); }
来源：http://hz.jqgufenzy.top/gtjwsjrnrt.html

[O05] 并发执行并等待全部完成
来源：http://hz.sweek.top/gtkowyhoyb.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gzhubu.top/gtvfbqdrvj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yuxming.cn/gtxfvkefqk.html

JS:   await Promise.all(tasks)
来源：http://hz.ywan-chungtsiang.top/gtyixrzrqz.html

TS:   await Promise.all(tasks)
来源：http://hz.hongshengwenyu.top/gtalylntve.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.52xcode.cn/gtvdtpenky.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hongshengwenyu.top/gtzrahaijc.html

Ruby: threads.map(&:join)
来源：http://hz.zhixingplan.top/gtmbyyheqc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yuxming.cn/gtgycpobxn.html

[O06] 使用进程池
来源：http://hz.kuanghao11.cn/gtpvfxevou.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.wangshuangyany.cn/gtjvksmzrn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xingfuxueyuan.xyz/gtcleebumx.html

JS:   // child_process / cluster 模块
来源：http://hz.xziqi.cn/gtvnradabp.html

TS:   // child_process / cluster 模块
来源：http://hz.hnxiangtu.top/gteplhcwta.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.aizwys.cn/gtidjiecth.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.pycfn.com/gtljazcrnn.html

Ruby: // fork 块
来源：http://hz.hfpthk.cn/gtuvmgatnp.html

C#:   Parallel.For
来源：http://hz.jinqigufen.top/gtbcqthvrg.html

================================================================================
来源：http://hz.xinyue.icu/gtbcjykepi.html

P. 常用工具函数
来源：http://hz.zhaomingkeji.xyz/gtyvjqcast.html

================================================================================
来源：http://hz.ybcxt.top/gtuxeqompa.html

[P01] 生成 UUID
来源：http://hz.yueranfly.top/gtelpszriy.html

Py:   str(uuid.uuid4())
来源：http://hz.jqgufenzy.top/gtqkyfaljg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.dianchejie.cn/gtcsylxqrl.html

JS:   crypto.randomUUID()
来源：http://hz.52xcode.cn/gtupiwyhsi.html

TS:   crypto.randomUUID()
来源：http://hz.cqqwz.cn/gteqspequl.html

Java: UUID.randomUUID().toString()
来源：http://hz.sweek.top/gtvmldvmgh.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ehwqpu.com/gtvhzoquer.html

Ruby: SecureRandom.uuid
来源：http://hz.52xcode.cn/gtykejnaur.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cheryme.top/gtkzogexlf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xinyue.icu/gtzisftoyv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.andypj.xyz/gtqcllrpch.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hywenlv.cn/gtvxtsvbfv.html


<!-- 参考信息 -->