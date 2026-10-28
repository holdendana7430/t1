代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ydzc1.top/gtvitutxfc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ybcxt.top/gtpaqgnmpt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.quarkkingdee.top/gtbiwgvzye.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jyoumei.cn/gtlhdkvznl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.feifeiyinyue.top/gtkdwvgpfj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.daria6918.cn/gtfmjcmzpx.html

[L05] 上传文件（multipart）
来源：http://hz.xuanzx.com/gtnpnwhjbl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhijiandao.cn/gtmtyjkzyb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.meibo888.top/gttipritlk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258.top/gtdgvxcksn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hfpthk.cn/gtjawpzqvf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.snrcjt.cn/gttgvatefd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hfpthk.cn/gtksyafjdw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shanyushiyangtech.top/gtbatibvni.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.sysykeji.top/gtkgktigoj.html

[L06] 解析响应为 JSON
来源：http://hz.gaohongyu789.top/gtoiszpbpv.html

Py:   resp.json()
来源：http://hz.ywan-chungtsiang.top/gtzuabehfb.html

PHP:  json_decode($body, true);
来源：http://hz.yueranfly.top/gtcpfuxqux.html

JS:   await resp.json()
来源：http://hz.redwolf501.top/gtkakmzstx.html

TS:   await resp.json()
来源：http://hz.feifeiyinyue.top/gtlbghxhue.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cucudq.cn/gtlgvgypma.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hnxiangtu.top/gtnuduhvfy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sxryk.cn/gtrylxlagn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.andypj.xyz/gtpetnzdxs.html

[L07] 处理 HTTP 状态码
来源：http://hz.feifeiyinyue.top/gthzmnnwoz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sysykeji.top/gtqnpgacbz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.c1oappe.top/gtayhomncw.html

JS:   resp.ok;  resp.status
来源：http://hz.sysykeji.top/gtgtcsnzwx.html

TS:   resp.ok;  resp.status
来源：http://hz.redwolf501.top/gtpfsuueyt.html

Java: resp.statusCode()
来源：http://hz.tian-w.cn/gtxdnhfsgu.html

Go:   resp.StatusCode
来源：http://hz.nanxuanxn.top/gtcvkqumfg.html

Ruby: resp.code.to_i
来源：http://hz.ppjwa.cn/gtzsxizeok.html

C#:   (int)resp.StatusCode
来源：http://hz.yonumen.top/gtydvrbfdo.html

[L08] 并发请求多个地址
来源：http://hz.jqgufenzy.top/gtgbyyqtfn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jiagoushi.top/gtesxbgoqu.html

PHP:  curl_multi_init() 系列
来源：http://hz.dianchejie.cn/gtdltqnwzu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.quarkkingdee.top/gtfroljxia.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuanzx.com/gtyaqaxnnc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ybcxt.top/gttpaskwii.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yuxming.cn/gtvdwdwbmu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cashguo.top/gtkfahpnoy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gotoacloud.top/gtaenbrplg.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtoosfzjym.html

M. 命令行 / 进程 / 环境
来源：http://hz.jqgufenzy.top/gtwyksugue.html

================================================================================
来源：http://hz.dianchejie.cn/gthwqjteqv.html

[M01] 读取命令行参数
来源：http://hz.xingfuxueyuan.xyz/gtmdekbnrh.html

Py:   sys.argv[1:]
来源：http://hz.dashuyun.cn/gthuinykfm.html

PHP:  $argv;  $argc;
来源：http://hz.ybcxt.top/gtpgdcviwg.html

JS:   process.argv.slice(2)
来源：http://hz.bjfxy.top/gtcyilckdf.html

TS:   process.argv.slice(2)
来源：http://hz.sysykeji.top/gtllifhslg.html

Java: args 数组（main 方法参数）
来源：http://hz.guannengcc.top/gtmacsxwzx.html

Go:   os.Args[1:]
来源：http://hz.hongshengwenyu.top/gtcmpmwxsq.html

Ruby: ARGV
来源：http://hz.ywan-chungtsiang.top/gtytmegwwz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sufxvd.cn/gtorhjifpy.html

[M02] 读取环境变量
来源：http://hz.tanke756.top/gtjxenkmrc.html

Py:   os.environ.get("HOME")
来源：http://hz.jinqigufen.top/gtysxtrurm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.pycfn.com/gtzilohvtv.html

JS:   process.env.HOME
来源：http://hz.yj20258888.top/gtiryupmnt.html

TS:   process.env.HOME
来源：http://hz.ydjk.org.cn/gtehrfyfis.html

Java: System.getenv("HOME")
来源：http://hz.ydzc1.top/gtrejtbumb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.pengpengdd.cyou/gtpndscdfp.html

Ruby: ENV["HOME"]
来源：http://hz.yongpay.top/gtcijjleio.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenjidiqi.icu/gtzgfgxdhb.html

[M03] 执行外部命令
来源：http://hz.zycfv.cn/gtlnccjdyh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xingfuxueyuan.xyz/gttgeygstg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gotoacloud.top/gtbvjdusaz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hongshengwenyu.top/gtkctpnxbl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gzhubu.top/gtfxcizivh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.iojbl.cn/gtxikucswz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.redwolf501.top/gtejbmtoow.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jianghu66.top/gtrtknftvq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ydzc1.top/gtrzhipwcu.html

[M04] 获取当前工作目录
来源：http://hz.zhengqikj.top/gtgenzrsjr.html

Py:   os.getcwd()
来源：http://hz.zhaomingkeji.xyz/gtonkzjjnd.html

PHP:  getcwd();
来源：http://hz.yangfankeji.com/gtdtgvqlcz.html

JS:   process.cwd()
来源：http://hz.wangshuangyany.cn/gtjjrqehmv.html

TS:   process.cwd()
来源：http://hz.tanke756.top/gtbazieoyu.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.iojbl.cn/gtqydbhuds.html

Go:   os.Getwd()
来源：http://hz.xylfe.cn/gtubaxlryk.html

Ruby: Dir.pwd
来源：http://hz.yj20258888.top/gtnqyiplio.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.fzhhl.top/gtannukxnd.html

[M05] 设置退出码
来源：http://hz.xuanzx.com/gtrgpflvzv.html

Py:   sys.exit(1)
来源：http://hz.sweek.top/gtbptrsgrz.html

PHP:  exit(1);
来源：http://hz.jqgufenzy.top/gtketpimjn.html

JS:   process.exit(1)
来源：http://hz.sxryk.cn/gtflrtcksv.html

TS:   process.exit(1)
来源：http://hz.jinghuilouyu.cn/gtnwnttwzd.html

Java: System.exit(1)
来源：http://hz.cucudq.cn/gtertexzlq.html

Go:   os.Exit(1)
来源：http://hz.xuetiantiany.cn/gtirdrncvd.html

Ruby: exit 1
来源：http://hz.yongpay.top/gtvneklggw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.havefunace.top/gtbheyruyj.html

[M06] 向标准错误输出
来源：http://hz.zhijiandao.cn/gtbysgllwj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.birdmap.top/gtxkaxjfrn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.wangshuangyany.cn/gttfxmuzho.html

JS:   console.error("err")
来源：http://hz.daxiang520.top/gtatnaeype.html

TS:   console.error("err")
来源：http://hz.kuanghao11.cn/gtlffvqnzn.html

Java: System.err.println("err")
来源：http://hz.hfpthk.cn/gtjlttrjae.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.wangshuangyany.cn/gtexegnsxn.html

Ruby: warn "err"
来源：http://hz.birdmap.top/gtitvnfjmh.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jinghuilouyu.cn/gtushpzkjt.html

[M07] 判断是否为主入口
来源：http://hz.yuxming.cn/gtwoowyiut.html

Py:   if __name__ == "__main__":
来源：http://hz.jlsjyb.cn/gtvkonkvwb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yongpay.top/gtmntwiljf.html

JS:   require.main === module
来源：http://hz.vqdsnc.cn/gtcauubgtj.html

TS:   require.main === module
来源：http://hz.zhongyouzk.top/gtfgcxktxh.html

Java: public static void main(String[] args)
来源：http://hz.zdqjudy.top/gtaoukuttf.html

Go:   func main()
来源：http://hz.nanxinkj.top/gtwcaqjzxt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.aibaodan.cn/gtwojwoquc.html

C#:   static void Main(string[] args)
来源：http://hz.redwolf501.top/gtsqxsekce.html

[M08] 获取系统与运行时信息
来源：http://hz.aizwys.cn/gtvaqqfmfe.html

Py:   platform.system();  platform.python_version()
来源：http://hz.haohaochexian.top/gtqrnszkyc.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhengqikj.top/gtgujfgcil.html

JS:   process.platform;  process.version
来源：http://hz.chenjidiqi.icu/gtzvhrslpf.html

TS:   process.platform;  process.version
来源：http://hz.xingfuxueyuan.xyz/gttgnilbrw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ehwqpu.com/gtlbjnupkh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.dianchejie.cn/gtvzfypkhz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.snrcjt.cn/gtlkrhdlhg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj20258.top/gtawiwfutw.html

================================================================================
来源：http://hz.yj202588.top/gtjsckgfph.html

N. 数据结构与算法
来源：http://hz.meibo888.top/gtmdqhkqtf.html

================================================================================
来源：http://hz.svipenyu.cn/gtkeqswbop.html

[N01] 二分查找（有序数组）
来源：http://hz.jinghuilouyu.cn/gticzjylos.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shanyushiyangtech.top/gtjmwjeahu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.bjfxy.top/gtqwnbbqml.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhengqikj.top/gtfbkrunzn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhijiandao.cn/gtcalwszch.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenzaomai.com/gtpidxorrg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.52xcode.cn/gtfvkzntsm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yvedp.cn/gtoudawlmd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.0kj1m.cn/gtfjogphoq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhongyouzk.top/gtqxnjbucp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangtech.top/gtlsaqtvkw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhengqikj.top/gtqolbuzxn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.dashuyun.cn/gtwjkrxnmr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fengsongda.top/gtpgbidxsy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.gzhubu.top/gtgcqtqilo.html

Go:   slices.Sort(arr)
来源：http://hz.shangyingyoupin.top/gtawvbbkbo.html

Ruby: arr.sort
来源：http://hz.yueranfly.top/gtfqzrqawg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.9152youxi.cn/gtqqoeyscs.html

[N03] 快速排序（分治示例）
来源：http://hz.aizwys.cn/gtroxdjvcl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.tian-w.cn/gtquzvxhgn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yvedp.cn/gtttrpdkwi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cashguo.top/gtuluydprr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigfzy.top/gtfvygwznc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jiagoushi.top/gtqzoaxzzb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.gaohongyu789.top/gtttrheknc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yuxming.cn/gtzuaxbqoz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.wangdashe.top/gtjzegktbe.html

[N04] 斐波那契数列
来源：http://hz.zhoulong.xyz/gtapuwbwwb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jianghu66.top/gtnrmnaqfl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tianlin.xyz/gtnkkgrhyc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.birdmap.top/gtbymtmkvn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jlsjyb.cn/gtlqoejrbc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sweek.top/gtbsscgbgk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.316326.xyz/gtegzxnfkh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xuetiantiany.cn/gtcmoeyiqg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gtqvujvdxz.html

[N05] 最大公约数
来源：http://hz.cheryme.top/gtnzdtndty.html

Py:   math.gcd(a, b)
来源：http://hz.svipenyu.cn/gtcjwqazpj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shanyushiyangkeji.top/gtwjayofjk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yongpay.top/gtoaqukvzw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangtech.top/gtzzjkmmrp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cqqwz.cn/gtayfjvrpi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.redwolf501.top/gtspfioiin.html

Ruby: a.gcd(b)
来源：http://hz.wangshuangyany.cn/gtefcgwhsz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.chenlongwang.top/gthndyicxk.html

[N06] 判断回文字符串
来源：http://hz.snrcjt.cn/gtfhlkmzhu.html

Py:   s == s[::-1]
来源：http://hz.fzhhl.top/gthlqhvmhl.html

PHP:  $s === strrev($s);
来源：http://hz.dashuyun.cn/gttvcwfnmb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ywan-chungtsiang.top/gtvmpebayb.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtjqdfcvkr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hnqzz.top/gtfwzhtmaa.html

Go:   // 双指针从两端比较
来源：http://hz.ppjwa.cn/gtgcchxygj.html

Ruby: s == s.reverse
来源：http://hz.meibo888.top/gtbzeprorv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zycfv.cn/gtivchorfq.html

[N07] 两数之和（返回下标）
来源：http://hz.sysykeji.top/gtstansskq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jlsjyb.cn/gthvwokdnm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yongpay.top/gtbbsyegzm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shangyingyoupin.top/gtebsywgoi.html

TS:   // 手写 Map<string, number>
来源：http://hz.xinyue.icu/gtnkxgmxxf.html

Java: // 手写 HashMap
来源：http://hz.tian-w.cn/gtwymfujkt.html

Go:   // 手写 map[int]int
来源：http://hz.jlsjyb.cn/gttembrzlh.html

Ruby: // 手写 Hash
来源：http://hz.cqqwz.cn/gtpnmcrgbz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinqigufen.top/gtibwsfyfh.html

[N08] 生成全排列
来源：http://hz.yvedp.cn/gtxozlvfsm.html

Py:   itertools.permutations(arr)
来源：http://hz.zhiwuduotai.top/gtpfsdlxpl.html

PHP:  // 手写递归交换
来源：http://hz.pycfn.com/gtroyrvzjg.html

JS:   // 手写回溯递归
来源：http://hz.sweek.top/gtowphxawa.html

TS:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtobaacwoq.html

Java: // 手写回溯递归
来源：http://hz.hammf.cn/gtyeuledlv.html

Go:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtvhqocdvi.html

Ruby: arr.permutation.to_a
来源：http://hz.cdnleiting.top/gtmalozvsg.html

C#:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtkvixyxnd.html

[N09] 栈与队列
来源：http://hz.chenlongwang.top/gtvkqwbjet.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.c1oappe.top/gtysetpwiq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.shuidangran.top/gtuepimjms.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.sufxvd.cn/gtzavdbppi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinqigfzy.top/gtfzhrqphn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xuetiantiany.cn/gtrqzrwawd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hysaishi.cn/gtlzklosni.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hongshengwenyu.top/gtsnjrhujd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.pycfn.com/gtmorgeoid.html

[N10] 链表节点定义
来源：http://hz.yj20258.top/gtggkbdivo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.guowangkeji.top/gtqzthowoa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ivvv.top/gtircuedni.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhixingplan.top/gtvnfidkvd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xingfuxueyuan.xyz/gtqbucmhlq.html

Java: class Node { int v; Node next; }
来源：http://hz.snrcjt.cn/gtxdjmaqks.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ydjk.org.cn/gtkspdsnob.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yj20258888.top/gtndeiwhzh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.52xcode.cn/gtulmunfli.html

[N11] 二叉树中序遍历
来源：http://hz.cashguo.top/gtphmlfgcv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shangyingyoupin.top/gtacilptew.html

PHP:  // 手写递归函数
来源：http://hz.nanxinkj.top/gtqmxdypcu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sweek.top/gtphcsldrz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.iojbl.cn/gthfdyusan.html

Java: // 手写递归
来源：http://hz.hywenlv.cn/gtiduuqhsd.html

Go:   // 手写递归
来源：http://hz.zhaomingkeji.xyz/gthqpuoxqv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.guowangkeji.top/gtsmhenskz.html

C#:   // 手写递归
来源：http://hz.cashguo.top/gtptmqtovi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cdnleiting.top/gtafksvgky.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hysaishi.cn/gtburvtuyn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ppjwa.cn/gtzgdbyvfj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenjidiqi.icu/gtrsiowrxg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.havefunace.top/gtzgqpqecn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.svipenyu.cn/gtwmhyfazk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.tianlin.xyz/gtnpxvnizw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cashguo.top/gtwgxhnafu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cashguo.top/gtxbkjnisn.html

================================================================================
来源：http://hz.ybcxt.top/gtorguxvvb.html

O. 并发与异步
来源：http://hz.chenjidiqi.icu/gtmbnplgzr.html

================================================================================
来源：http://hz.ydjk.org.cn/gttlakjycs.html

[O01] 启动一个线程
来源：http://hz.jinqigfzy.top/gtajuefies.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yuanzhike.top/gtwclrlyvm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhixingplan.top/gtubdsekvw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.tian-w.cn/gtnkilbsgj.html

TS:   // 同 JS
来源：http://hz.zycfv.cn/gtpdvvpnur.html

Java: new Thread(() -> f()).start()
来源：http://hz.ydjk.org.cn/gtojybxiud.html

Go:   go f()
来源：http://hz.yueranfly.top/gthvlkgjnx.html

Ruby: Thread.new { f }
来源：http://hz.andypj.xyz/gtwcimdlou.html

C#:   Task.Run(() => F());
来源：http://hz.yvedp.cn/gtslhaicmc.html

[O02] 使用线程池
来源：http://hz.sxryk.cn/gtmalrvcoj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xuetiantiany.cn/gtmudgvleq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinghuilouyu.cn/gtsqqgllnt.html

JS:   // worker_threads 线程池
来源：http://hz.zdqjudy.top/gtxhzhqjyb.html

TS:   // worker_threads 线程池
来源：http://hz.smart0.xyz/gtmfljfgzm.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.meibo888.top/gtxnuaoneg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yj202588.top/gthirixwev.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.guannengcc.top/gttxoidmdz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shanyushiyangkeji.top/gthqozscjq.html

[O03] 加锁保护共享数据
来源：http://hz.yueranfly.top/gtbbtoqbug.html

Py:   with lock: shared += 1
来源：http://hz.yvedp.cn/gtjzsdhmxw.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jyoumei.cn/gtfutserxr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yvedp.cn/gteslimvyx.html

TS:   // 同 JS
来源：http://hz.jinqigufen.top/gtsgiutyit.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhixingplan.top/gtguvuqnwn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zycfv.cn/gtyvdjbumx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ybcxt.top/gtoknhtslk.html

C#:   lock (gate) { shared++; }
来源：http://hz.nanxuanxn.top/gtnxdjggku.html

[O04] 定义异步函数并等待
来源：http://hz.zycfv.cn/gtpcefhvlm.html

Py:   async def f():⏎    await g()
来源：http://hz.feifeiyinyue.top/gthnonshnj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.redwolf501.top/gttlexvxno.html

JS:   async function f() { await g(); }
来源：http://hz.guowangkeji.top/gtznzlmhak.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yj20258888.top/gtpaeurrlk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jyoumei.cn/gttahovdtj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jyoumei.cn/gtyocrevwr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.haohaochexian.top/gthmayhoxy.html

C#:   async Task F() { await G(); }
来源：http://hz.aibaodan.cn/gtdjtvmfhl.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhijiandao.cn/gtbbvkoueb.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cucudq.cn/gtytscgext.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hnxiangtu.top/gtofspyzqi.html

JS:   await Promise.all(tasks)
来源：http://hz.haohaochexian.top/gtiiorfnjb.html

TS:   await Promise.all(tasks)
来源：http://hz.quarkkingdee.top/gtmbarllgk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hnxiangtu.top/gtlrxcexxz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.quarkkingdee.top/gthddqbmdc.html

Ruby: threads.map(&:join)
来源：http://hz.gogol.net.cn/gtcfdqzelp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.bjfxy.top/gtteaefjfm.html

[O06] 使用进程池
来源：http://hz.zhongyouzk.top/gtmydmcysw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shanyushiyangkeji.top/gtkummrkhd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.0kj1m.cn/gtflukierm.html

JS:   // child_process / cluster 模块
来源：http://hz.quarkkingdee.top/gtqsevnruo.html

TS:   // child_process / cluster 模块
来源：http://hz.vqdsnc.cn/gtflzgfeur.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.bjfxy.top/gtdnedxibk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.cqqwz.cn/gtlokdlbtg.html

Ruby: // fork 块
来源：http://hz.redwolf501.top/gtoudedafc.html

C#:   Parallel.For
来源：http://hz.kuanghao11.cn/gtvkieqwmx.html

================================================================================
来源：http://hz.iojbl.cn/gtzpqxtlty.html

P. 常用工具函数
来源：http://hz.yuanzhike.top/gtvoppalnw.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtdpbeopht.html

[P01] 生成 UUID
来源：http://hz.shuidangran.top/gtdkajltav.html

Py:   str(uuid.uuid4())
来源：http://hz.dianchejie.cn/gtqmmqovnz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yongpay.top/gtkgkfvhvt.html

JS:   crypto.randomUUID()
来源：http://hz.0kj1m.cn/gtdgxeoqua.html

TS:   crypto.randomUUID()
来源：http://hz.xuanzx.com/gttnnlkbvf.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhixingplan.top/gtlqoerokc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.0kj1m.cn/gtpdixthyr.html

Ruby: SecureRandom.uuid
来源：http://hz.hnqzz.top/gtizmcdgob.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.gzhubu.top/gtxbwxdocn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.daxiang520.top/gthqyngbqg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sweek.top/gtouedyycy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.chenzaomai.com/gtfgemisrk.html


<!-- 参考信息 -->