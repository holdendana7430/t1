代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.wangshuangyany.cn/gtpusvmpaw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.nwbrower.top/gtmcqjmtas.html

[L05] 上传文件（multipart）
来源：http://hz.aibaodan.cn/gtaencaedd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.havefunace.top/gtwrcnxkxe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.sysykeji.top/gtbjzgdpsq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shzxlz.cn/gtnxiodlcb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hywenlv.cn/gtyhwagccs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.pengpengdd.cyou/gtqcpuvoct.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.andypj.xyz/gtrfzpcsza.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.chenlongwang.top/gtrfdfjnkq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ivvv.top/gtyovhooev.html

[L06] 解析响应为 JSON
来源：http://hz.xuetiantiany.cn/gtqpvhxxic.html

Py:   resp.json()
来源：http://hz.gzhubu.top/gtrecxjxye.html

PHP:  json_decode($body, true);
来源：http://hz.pycfn.com/gtjdjzplwb.html

JS:   await resp.json()
来源：http://hz.hnqzz.top/gtqacboudm.html

TS:   await resp.json()
来源：http://hz.birdmap.top/gtajrhvexz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zdqjudy.top/gtaoavoaqr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xziqi.cn/gtfdttmeiy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sufxvd.cn/gtvxybcjmi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.quarkkingdee.top/gttltwaptq.html

[L07] 处理 HTTP 状态码
来源：http://hz.meibo888.top/gtjaeobmhy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenjidiqi.icu/gtzyvssnrq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yonumen.top/gterqmzjfo.html

JS:   resp.ok;  resp.status
来源：http://hz.hongshengwenyu.top/gttgfurbhz.html

TS:   resp.ok;  resp.status
来源：http://hz.yangfankeji.com/gtbyzupbsn.html

Java: resp.statusCode()
来源：http://hz.chenjidiqi.icu/gthsjlfnpi.html

Go:   resp.StatusCode
来源：http://hz.havefunace.top/gtngrwqyxk.html

Ruby: resp.code.to_i
来源：http://hz.kuanghao11.cn/gtccrqvzqf.html

C#:   (int)resp.StatusCode
来源：http://hz.iojbl.cn/gtqlkvqrup.html

[L08] 并发请求多个地址
来源：http://hz.gzhubu.top/gtsspsoyia.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xziqi.cn/gtucpbxhmo.html

PHP:  curl_multi_init() 系列
来源：http://hz.shanyushiyangtech.top/gtevkvfzmi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuanzhike.top/gtotoajgli.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fzhhl.top/gtccbfazsk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhoulong.xyz/gtjdobthkb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.nanxinkj.top/gtktzstgfu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jqgfzy.top/gtrnoaorvs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xingfuxueyuan.xyz/gtcarulyon.html

================================================================================
来源：http://hz.c1oappe.top/gtcgmdgxin.html

M. 命令行 / 进程 / 环境
来源：http://hz.316326.xyz/gtiaoglzln.html

================================================================================
来源：http://hz.gogol.net.cn/gtuuwixkgz.html

[M01] 读取命令行参数
来源：http://hz.tanke756.top/gthxelxpay.html

Py:   sys.argv[1:]
来源：http://hz.hammf.cn/gtjvmfpmut.html

PHP:  $argv;  $argc;
来源：http://hz.hongshengwenyu.top/gtgyikvhpc.html

JS:   process.argv.slice(2)
来源：http://hz.chenzaomai.com/gtwazyqmua.html

TS:   process.argv.slice(2)
来源：http://hz.wangshuangyany.cn/gtqaupeczi.html

Java: args 数组（main 方法参数）
来源：http://hz.yueranfly.top/gtuwlnwcjc.html

Go:   os.Args[1:]
来源：http://hz.xziqi.cn/gtvzpnraon.html

Ruby: ARGV
来源：http://hz.zhongyouzk.top/gtudeptrwx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhixingplan.top/gtdcjkykfe.html

[M02] 读取环境变量
来源：http://hz.zhaomingkeji.xyz/gtebneciqz.html

Py:   os.environ.get("HOME")
来源：http://hz.yuanzhike.top/gthnnyvwfr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hnxiangtu.top/gtiucxtmcx.html

JS:   process.env.HOME
来源：http://hz.nanxuanxn.top/gtegyfpwwc.html

TS:   process.env.HOME
来源：http://hz.shzxlz.cn/gtvsuxkved.html

Java: System.getenv("HOME")
来源：http://hz.smart0.xyz/gtxonclvdw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.snrcjt.cn/gtdiqukjop.html

Ruby: ENV["HOME"]
来源：http://hz.jqgufenzy.top/gtccoplmuz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zycfv.cn/gtxeuyttct.html

[M03] 执行外部命令
来源：http://hz.tianlin.xyz/gtfkywvnts.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuxming.cn/gtoecufkps.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.aibaodan.cn/gttsulcfrw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhiwuduotai.top/gtjpvtaqwy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ywan-chungtsiang.top/gtuslftgvz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xinyue.icu/gtkpgehcse.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zycfv.cn/gtkesrysml.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shangyingyoupin.top/gtygmcngfn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hnxiangtu.top/gtxyhnslye.html

[M04] 获取当前工作目录
来源：http://hz.jqgfzy.top/gtjxsbsoff.html

Py:   os.getcwd()
来源：http://hz.zhiwuduotai.top/gtfqodyiob.html

PHP:  getcwd();
来源：http://hz.fzhhl.top/gtmyrojmuz.html

JS:   process.cwd()
来源：http://hz.vqdsnc.cn/gtscxmonpm.html

TS:   process.cwd()
来源：http://hz.guannengcc.top/gtfxlwhnka.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yvedp.cn/gtgyvabttq.html

Go:   os.Getwd()
来源：http://hz.nanxinkj.top/gtebgkswgf.html

Ruby: Dir.pwd
来源：http://hz.jinghuilouyu.cn/gtsjlhgnjl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yueranfly.top/gtuwoxssgd.html

[M05] 设置退出码
来源：http://hz.yonumen.top/gtbpmlxyvq.html

Py:   sys.exit(1)
来源：http://hz.52xcode.cn/gtwrbmcltr.html

PHP:  exit(1);
来源：http://hz.gzhubu.top/gtwqhnryzn.html

JS:   process.exit(1)
来源：http://hz.haohaochexian.top/gtrejqfhkh.html

TS:   process.exit(1)
来源：http://hz.smart0.xyz/gtktvhnmea.html

Java: System.exit(1)
来源：http://hz.iojbl.cn/gttgmsjviw.html

Go:   os.Exit(1)
来源：http://hz.hammf.cn/gthcoysppj.html

Ruby: exit 1
来源：http://hz.zycfv.cn/gttfibintv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yvedp.cn/gtqfajurbq.html

[M06] 向标准错误输出
来源：http://hz.yanxiufei.cn/gtanixwrpw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.c1oappe.top/gtokepqnol.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cashguo.top/gtxazubpih.html

JS:   console.error("err")
来源：http://hz.cdnleiting.top/gtpjyzxkot.html

TS:   console.error("err")
来源：http://hz.gotoacloud.top/gtmuwsanug.html

Java: System.err.println("err")
来源：http://hz.kuanghao11.cn/gtfnbrzxhu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.wangshuangyany.cn/gtxtfspllt.html

Ruby: warn "err"
来源：http://hz.birdmap.top/gtyzflfhvq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cdnleiting.top/gttehrkvgh.html

[M07] 判断是否为主入口
来源：http://hz.bjfxy.top/gtwplahyca.html

Py:   if __name__ == "__main__":
来源：http://hz.sysykeji.top/gtdpdwqtjw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.52xcode.cn/gthrhakdai.html

JS:   require.main === module
来源：http://hz.gogol.net.cn/gtqrnwdafz.html

TS:   require.main === module
来源：http://hz.gaohongyu789.top/gtonwyilhc.html

Java: public static void main(String[] args)
来源：http://hz.gogol.net.cn/gtpgjtzqck.html

Go:   func main()
来源：http://hz.pengpengdd.cyou/gtmgqaiafx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinqigufen.top/gtoqnerxxe.html

C#:   static void Main(string[] args)
来源：http://hz.ydzc1.top/gtyzkilfpv.html

[M08] 获取系统与运行时信息
来源：http://hz.ehwqpu.com/gtevchvsqo.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jianghu66.top/gtskxalkxh.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shzxlz.cn/gtmpcwsiwp.html

JS:   process.platform;  process.version
来源：http://hz.ydzc1.top/gtydgghhqb.html

TS:   process.platform;  process.version
来源：http://hz.snrcjt.cn/gtssvfenrl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.dashuyun.cn/gtoxtinvzj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jqgufenzy.top/gtwpffxggg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xingfuxueyuan.xyz/gtllaqlywz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.birdmap.top/gturyfmcyh.html

================================================================================
来源：http://hz.nanxuanxn.top/gtfdwxpybs.html

N. 数据结构与算法
来源：http://hz.quarkkingdee.top/gtbdkpqjxh.html

================================================================================
来源：http://hz.cucudq.cn/gtpzqlppqz.html

[N01] 二分查找（有序数组）
来源：http://hz.yj20258.top/gtpwkltpsw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.tian-w.cn/gtgxmcmubm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yangfankeji.com/gtkfgeqwgy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigfzy.top/gtteguosbp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fengsongda.top/gtvuwgkhrb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gotoacloud.top/gtlirqhvis.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.wangdashe.top/gtcoqkzpwp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ydjk.org.cn/gtdrkdkxtd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yj20258888.top/gtjslkzdyz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shangyingyoupin.top/gtbqaotdoy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hammf.cn/gtvvlrbztb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinyuanbaomall.cn/gtobnwsvej.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jlsjyb.cn/gtmuyqshia.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinqigfzy.top/gtaohdahud.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yj20258.top/gtbtlbbnyf.html

Go:   slices.Sort(arr)
来源：http://hz.tian-w.cn/gtrrxdrzsb.html

Ruby: arr.sort
来源：http://hz.jiagoushi.top/gtydzloslk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shangyingyoupin.top/gtopyvgdhy.html

[N03] 快速排序（分治示例）
来源：http://hz.svipenyu.cn/gtxlvbsxnx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.c1oappe.top/gtsqmtcwvi.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ydzc1.top/gtgcvtoulf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydzc1.top/gtdxbktgts.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sufxvd.cn/gtshyzeekn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.smart0.xyz/gtzotsqlgw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.meibo888.top/gtyaywsmmu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.fengsongda.top/gtmpthuiwu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.aibaodan.cn/gtsgmgobuk.html

[N04] 斐波那契数列
来源：http://hz.yj20258888.top/gtdmkqmkzm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zycfv.cn/gtsmclaviq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tanke756.top/gthcmnpzyi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yangfankeji.com/gtniyvpilv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ywan-chungtsiang.top/gtgvdesovk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xziqi.cn/gtscymlcwt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.redwolf501.top/gtphkrpedj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ydzc1.top/gtrosxfupi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.feifeiyinyue.top/gtosbafjdf.html

[N05] 最大公约数
来源：http://hz.pycfn.com/gtggstaxbk.html

Py:   math.gcd(a, b)
来源：http://hz.dianchejie.cn/gthnzbjyol.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shanyushiyangkeji.top/gtoxyzpgtw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gtctonopss.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xinyue.icu/gtbwygtdvn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.pycfn.com/gtopftdvnp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.svipenyu.cn/gtycitysgq.html

Ruby: a.gcd(b)
来源：http://hz.chenzaomai.com/gtqmmyrume.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hywenlv.cn/gtbnjoqzxl.html

[N06] 判断回文字符串
来源：http://hz.zhijiandao.cn/gttnwzuniz.html

Py:   s == s[::-1]
来源：http://hz.fzhhl.top/gtafbfqwxt.html

PHP:  $s === strrev($s);
来源：http://hz.aibaodan.cn/gtmnxjjuhq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.0kj1m.cn/gtlqowvukv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yanxiufei.cn/gtsscygxtn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhongyouzk.top/gtkszxicqy.html

Go:   // 双指针从两端比较
来源：http://hz.cdnleiting.top/gtczchkdhy.html

Ruby: s == s.reverse
来源：http://hz.zhijiandao.cn/gtkticowwe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.aibaodan.cn/gtrnbefvix.html

[N07] 两数之和（返回下标）
来源：http://hz.zycfv.cn/gtmxazbneq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.havefunace.top/gtfykwzjaf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.andypj.xyz/gtoyjhvxnz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yuxming.cn/gtklydxxef.html

TS:   // 手写 Map<string, number>
来源：http://hz.yangfankeji.com/gtjogngcle.html

Java: // 手写 HashMap
来源：http://hz.tian-w.cn/gtubnsgmwz.html

Go:   // 手写 map[int]int
来源：http://hz.ppjwa.cn/gtskzfndhk.html

Ruby: // 手写 Hash
来源：http://hz.shanyushiyangtech.top/gtvhwecfbh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ppjwa.cn/gtrkqekixy.html

[N08] 生成全排列
来源：http://hz.nwbrower.top/gtgtoigkup.html

Py:   itertools.permutations(arr)
来源：http://hz.ywan-chungtsiang.top/gtcscbubls.html

PHP:  // 手写递归交换
来源：http://hz.jinqigufen.top/gtmjitlfej.html

JS:   // 手写回溯递归
来源：http://hz.yongpay.top/gtxltxgzyh.html

TS:   // 手写回溯递归
来源：http://hz.daxiang520.top/gtzpakokvo.html

Java: // 手写回溯递归
来源：http://hz.kuanghao11.cn/gtpjrcwvut.html

Go:   // 手写回溯递归
来源：http://hz.cheryme.top/gtuznaelpy.html

Ruby: arr.permutation.to_a
来源：http://hz.redwolf501.top/gtfpbryvvo.html

C#:   // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtlaqnmvcb.html

[N09] 栈与队列
来源：http://hz.hnxiangtu.top/gtjhnlggqb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.nanxuanxn.top/gtskejrscx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhixingplan.top/gtvlrupuyc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhixingplan.top/gtzceqmbon.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ehwqpu.com/gtaxlcwjhh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.birdmap.top/gtauldligs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.pycfn.com/gtxvpztswh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xuanzx.com/gtwybisikn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.vqdsnc.cn/gtncbwqadi.html

[N10] 链表节点定义
来源：http://hz.nanxinkj.top/gtndrvaulf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.tanke756.top/gtuapgdmyt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.guowangkeji.top/gtodedbdau.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.aibaodan.cn/gtsgbkdrub.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shuidangran.top/gtiefebdjo.html

Java: class Node { int v; Node next; }
来源：http://hz.daria6918.cn/gtiwsgzjlz.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ydjk.org.cn/gtgwsnwzep.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.nanxuanxn.top/gtokoxjile.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.pycfn.com/gtjwhbkmpk.html

[N11] 二叉树中序遍历
来源：http://hz.hammf.cn/gtqnztbsbu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sysykeji.top/gtheivkbkr.html

PHP:  // 手写递归函数
来源：http://hz.hysaishi.cn/gtfspwcjpi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gogol.net.cn/gtdojllxam.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gotoacloud.top/gtenyidpms.html

Java: // 手写递归
来源：http://hz.ybcxt.top/gtnxwwooxg.html

Go:   // 手写递归
来源：http://hz.quarkkingdee.top/gtjjbwdzci.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhiwuduotai.top/gtcxrlehxb.html

C#:   // 手写递归
来源：http://hz.zycfv.cn/gtnnaddkep.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.chenzaomai.com/gtqeebkcwu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.meibo888.top/gtmletjhjn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hnxiangtu.top/gttkdcstio.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cdnleiting.top/gtvbiexsbz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hywenlv.cn/gtynngicpr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xinyue.icu/gtaswrdaoi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.iojbl.cn/gtqlqkjcpa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yongpay.top/gtdbuwoloh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.feifeiyinyue.top/gtjeedrivl.html

================================================================================
来源：http://hz.tanke756.top/gtrlnkegmt.html

O. 并发与异步
来源：http://hz.dianchejie.cn/gthcyzjuqd.html

================================================================================
来源：http://hz.redwolf501.top/gthngchzal.html

[O01] 启动一个线程
来源：http://hz.pengpengdd.cyou/gtmxfgpjao.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.daxiang520.top/gtebyfamhz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gotoacloud.top/gtxwagdcbv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.sysykeji.top/gtsvuievzm.html

TS:   // 同 JS
来源：http://hz.aizwys.cn/gtzwslmqny.html

Java: new Thread(() -> f()).start()
来源：http://hz.yuanzhike.top/gtprcvsllr.html

Go:   go f()
来源：http://hz.redwolf501.top/gtahizxjak.html

Ruby: Thread.new { f }
来源：http://hz.gaohongyu789.top/gtwqzinhht.html

C#:   Task.Run(() => F());
来源：http://hz.quarkkingdee.top/gtvfpbdzjf.html

[O02] 使用线程池
来源：http://hz.hongshengwenyu.top/gtcdzbqnff.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.guannengcc.top/gtwctvhnel.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinyuanbaomall.cn/gtmnubfpgm.html

JS:   // worker_threads 线程池
来源：http://hz.wangdashe.top/gtjhttmxhw.html

TS:   // worker_threads 线程池
来源：http://hz.shzxlz.cn/gtfjzxwmox.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.sufxvd.cn/gtsbwxiqts.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.andypj.xyz/gtzcearwmi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zycfv.cn/gtrbhshipu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xziqi.cn/gtpsaqwqox.html

[O03] 加锁保护共享数据
来源：http://hz.sysykeji.top/gtygyicvav.html

Py:   with lock: shared += 1
来源：http://hz.9152youxi.cn/gtwnzeapnd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.pycfn.com/gttzapiguo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hnxiangtu.top/gtuswsmquu.html

TS:   // 同 JS
来源：http://hz.yj202588.top/gtbpdfdbij.html

Java: synchronized (this) { shared++; }
来源：http://hz.tianlin.xyz/gtsdoyvfcc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hysaishi.cn/gtczjmbmdt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.birdmap.top/gtyjzclyts.html

C#:   lock (gate) { shared++; }
来源：http://hz.c1oappe.top/gtkaqcutnz.html

[O04] 定义异步函数并等待
来源：http://hz.daria6918.cn/gtatrqkgkx.html

Py:   async def f():⏎    await g()
来源：http://hz.fzhhl.top/gtfzlbmjqp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sysykeji.top/gtjtoxpuke.html

JS:   async function f() { await g(); }
来源：http://hz.aibaodan.cn/gttbbvfqyq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shanyushiyangkeji.top/gtoesvlgva.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jinqigfzy.top/gtjeeprlwn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhoulong.xyz/gtwbztswwc.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hnxiangtu.top/gtekpffjts.html

C#:   async Task F() { await G(); }
来源：http://hz.shzxlz.cn/gtsvfjckoe.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinghuilouyu.cn/gtimoltkyv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cashguo.top/gtpxwxfhxz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.vqdsnc.cn/gtqjjjrgog.html

JS:   await Promise.all(tasks)
来源：http://hz.quarkkingdee.top/gtmwyluyla.html

TS:   await Promise.all(tasks)
来源：http://hz.tanke756.top/gtbonkifvv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.wangshuangyany.cn/gtdvcmdgxs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhijiandao.cn/gtznmfxgod.html

Ruby: threads.map(&:join)
来源：http://hz.gzhubu.top/gtqnwrbhbq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.quarkkingdee.top/gtowxhxjap.html

[O06] 使用进程池
来源：http://hz.hammf.cn/gtyfylgqdt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhixingplan.top/gtbntasgow.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.svipenyu.cn/gtlzzdxllq.html

JS:   // child_process / cluster 模块
来源：http://hz.yvedp.cn/gtqptfbhkh.html

TS:   // child_process / cluster 模块
来源：http://hz.cucudq.cn/gtfybixfgl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sufxvd.cn/gteogkwmdz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.quarkkingdee.top/gtlmoveoup.html

Ruby: // fork 块
来源：http://hz.guowangkeji.top/gtahqwpzxy.html

C#:   Parallel.For
来源：http://hz.ivvv.top/gtmsijumvi.html

================================================================================
来源：http://hz.chenzaomai.com/gtgtofusko.html

P. 常用工具函数
来源：http://hz.ydjk.org.cn/gtpaotbkyn.html

================================================================================
来源：http://hz.jqgufenzy.top/gtcmnuvgne.html

[P01] 生成 UUID
来源：http://hz.0kj1m.cn/gtlgkuptco.html

Py:   str(uuid.uuid4())
来源：http://hz.zhijiandao.cn/gtnynjdcce.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinghuilouyu.cn/gtqjfzsfof.html

JS:   crypto.randomUUID()
来源：http://hz.ehwqpu.com/gtbnedatps.html

TS:   crypto.randomUUID()
来源：http://hz.pengpengdd.cyou/gtmoxypwfx.html

Java: UUID.randomUUID().toString()
来源：http://hz.xylfe.cn/gtkhmvudmc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ybcxt.top/gtczzozplt.html

Ruby: SecureRandom.uuid
来源：http://hz.0kj1m.cn/gtmrtsetxm.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hysaishi.cn/gtcvfybwxh.html

[P02] MD5 / SHA256 摘要
来源：http://hz.daxiang520.top/gtiliecweo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yj20258.top/gtqmasxcll.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.wangshuangyany.cn/gtddsnyang.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cdnleiting.top/gtnfctfqsr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yuxming.cn/gtgdlhkmwg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jlsjyb.cn/gttlwlzjwv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.havefunace.top/gtsspewvms.html


<!-- 参考信息 -->