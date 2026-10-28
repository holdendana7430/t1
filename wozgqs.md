代发 wailian999

[L03] 设置自定义请求头
来源：http://hz.cdnleiting.top/gtalvaxkbe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhongyouzk.top/gtljowmicq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhoulong.xyz/gtmyjvcxci.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.haohaochexian.top/gtzpmgzgmj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhijiandao.cn/gtlsjkwolq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yuanzhike.top/gthqcbxnub.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenjidiqi.icu/gtsdohsrez.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ydjk.org.cn/gtqlkubjeo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.sysykeji.top/gtygquosns.html

[L04] 设置超时
来源：http://hz.xinyue.icu/gtydpotrxa.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cdnleiting.top/gtsootjgwx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ppjwa.cn/gtvdygaapf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhijiandao.cn/gtxbgsgnci.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj202588.top/gtdqchfcqq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.iojbl.cn/gtwladkelm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.tanke756.top/gtedggcxhw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.nanxinkj.top/gtbasaxkbs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gogol.net.cn/gtorvokkoh.html

[L05] 上传文件（multipart）
来源：http://hz.hfpthk.cn/gtqvehvgsx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hysaishi.cn/gtmllemcft.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cheryme.top/gtfssbiiug.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.0kj1m.cn/gtrbxlmrgf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.bjfxy.top/gtctvlzyhz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.aizwys.cn/gtymoiliaj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.dianchejie.cn/gtpnzwmezu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhongyouzk.top/gtwwyuxpsq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinqigufen.top/gtgzezdimi.html

[L06] 解析响应为 JSON
来源：http://hz.ehwqpu.com/gtnapujyvf.html

Py:   resp.json()
来源：http://hz.chenlongwang.top/gtryuphlpt.html

PHP:  json_decode($body, true);
来源：http://hz.kuanghao11.cn/gtuspzztmd.html

JS:   await resp.json()
来源：http://hz.cheryme.top/gtyapwsiyo.html

TS:   await resp.json()
来源：http://hz.nanxuanxn.top/gtxybjepfs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhongyouzk.top/gtvubzprvj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ppjwa.cn/gtuvxvgysy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ivvv.top/gtxnfzxewv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.smart0.xyz/gtoqxmqolm.html

[L07] 处理 HTTP 状态码
来源：http://hz.yuxming.cn/gtybccbwxz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhongyouzk.top/gtpdbhebnm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yueranfly.top/gtanwwnjcy.html

JS:   resp.ok;  resp.status
来源：http://hz.ppjwa.cn/gtoihlcjoo.html

TS:   resp.ok;  resp.status
来源：http://hz.cqqwz.cn/gtfjsckstr.html

Java: resp.statusCode()
来源：http://hz.birdmap.top/gtgesvurkj.html

Go:   resp.StatusCode
来源：http://hz.jlsjyb.cn/gtxfkzmqlu.html

Ruby: resp.code.to_i
来源：http://hz.nanxinkj.top/gtdwzehijh.html

C#:   (int)resp.StatusCode
来源：http://hz.yangfankeji.com/gtgohternh.html

[L08] 并发请求多个地址
来源：http://hz.snrcjt.cn/gtnnoodlse.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hywenlv.cn/gtfxtemvrt.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhengqikj.top/gtdkbeevxp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.316326.xyz/gtsablmqko.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.vqdsnc.cn/gtufhkecnu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhijiandao.cn/gtvhgybwrw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhoulong.xyz/gtxfwkabrs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.tanke756.top/gtsvotgjst.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinyuanbaomall.cn/gtjibyrmqs.html

================================================================================
来源：http://hz.chenlongwang.top/gtalpjsihb.html

M. 命令行 / 进程 / 环境
来源：http://hz.jinqigufen.top/gtabretgbf.html

================================================================================
来源：http://hz.ppjwa.cn/gtstcrotqd.html

[M01] 读取命令行参数
来源：http://hz.ppjwa.cn/gtpjlmlvaj.html

Py:   sys.argv[1:]
来源：http://hz.sufxvd.cn/gtjzjdalau.html

PHP:  $argv;  $argc;
来源：http://hz.xinyue.icu/gtnfyreyaq.html

JS:   process.argv.slice(2)
来源：http://hz.gotoacloud.top/gtrqnlhipr.html

TS:   process.argv.slice(2)
来源：http://hz.meibo888.top/gtqmhmuifg.html

Java: args 数组（main 方法参数）
来源：http://hz.zhongyouzk.top/gtlhwmmokr.html

Go:   os.Args[1:]
来源：http://hz.redwolf501.top/gtikblxtrj.html

Ruby: ARGV
来源：http://hz.xingfuxueyuan.xyz/gtpmqmhvrl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhixingplan.top/gtquhechfg.html

[M02] 读取环境变量
来源：http://hz.yvedp.cn/gtamgjafvk.html

Py:   os.environ.get("HOME")
来源：http://hz.hongshengwenyu.top/gtoycuncpl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.wangdashe.top/gtlhaxwepc.html

JS:   process.env.HOME
来源：http://hz.ehwqpu.com/gtlkvlehap.html

TS:   process.env.HOME
来源：http://hz.pengpengdd.cyou/gtfnxtxvyx.html

Java: System.getenv("HOME")
来源：http://hz.xziqi.cn/gtgznokcsj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.kuanghao11.cn/gthonlxroe.html

Ruby: ENV["HOME"]
来源：http://hz.gzhubu.top/gtudbmrnwf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhixingplan.top/gtxgmhxtja.html

[M03] 执行外部命令
来源：http://hz.ppjwa.cn/gthpvbyijc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ydzc1.top/gtjkitiwug.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.chenlongwang.top/gtdbdkcmyr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.316326.xyz/gtvdwqtoyk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.tian-w.cn/gtgzrgjvck.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ydjk.org.cn/gttnyrqpec.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhoulong.xyz/gtrmdbeonh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cqqwz.cn/gtsgofahdi.html

C#:   Process.Start("ls", "-l");
来源：http://hz.mhx1999.top/gtyzdymacv.html

[M04] 获取当前工作目录
来源：http://hz.yanxiufei.cn/gtoxntstul.html

Py:   os.getcwd()
来源：http://hz.ywan-chungtsiang.top/gtwidnwyim.html

PHP:  getcwd();
来源：http://hz.haohaochexian.top/gtdybgdoqh.html

JS:   process.cwd()
来源：http://hz.yongpay.top/gthaxbofho.html

TS:   process.cwd()
来源：http://hz.pengpengdd.cyou/gtbwiqjhik.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.chenlongwang.top/gtvnsxctdb.html

Go:   os.Getwd()
来源：http://hz.nanxinkj.top/gtzwownadw.html

Ruby: Dir.pwd
来源：http://hz.tianlin.xyz/gtverxgbib.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ehwqpu.com/gtjdqnspfc.html

[M05] 设置退出码
来源：http://hz.hysaishi.cn/gtuwcrnwrt.html

Py:   sys.exit(1)
来源：http://hz.redwolf501.top/gtcegaeoxt.html

PHP:  exit(1);
来源：http://hz.hongshengwenyu.top/gtxodwazzg.html

JS:   process.exit(1)
来源：http://hz.nwbrower.top/gttepsliyo.html

TS:   process.exit(1)
来源：http://hz.pengpengdd.cyou/gtkabhotil.html

Java: System.exit(1)
来源：http://hz.9152youxi.cn/gtykiepncd.html

Go:   os.Exit(1)
来源：http://hz.tanke756.top/gtgnudkjio.html

Ruby: exit 1
来源：http://hz.quarkkingdee.top/gtoxtqycrh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.daxiang520.top/gtpmcxjmop.html

[M06] 向标准错误输出
来源：http://hz.guowangkeji.top/gtexqbgorf.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ywan-chungtsiang.top/gtzsajnzne.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.haohaochexian.top/gtlsegfjpn.html

JS:   console.error("err")
来源：http://hz.quarkkingdee.top/gtewlgegwl.html

TS:   console.error("err")
来源：http://hz.chenzaomai.com/gtyyznqkvz.html

Java: System.err.println("err")
来源：http://hz.zhaomingkeji.xyz/gtgymcragb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hysaishi.cn/gtebxixkvm.html

Ruby: warn "err"
来源：http://hz.hfpthk.cn/gtrnczghvt.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yj202588.top/gtuvparltv.html

[M07] 判断是否为主入口
来源：http://hz.cdnleiting.top/gtteemplqc.html

Py:   if __name__ == "__main__":
来源：http://hz.aibaodan.cn/gttyuohqeu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.fengsongda.top/gtaqpusuoy.html

JS:   require.main === module
来源：http://hz.yj20258.top/gtqusgjfkq.html

TS:   require.main === module
来源：http://hz.zdqjudy.top/gtvbswueae.html

Java: public static void main(String[] args)
来源：http://hz.fzhhl.top/gtwoparfrc.html

Go:   func main()
来源：http://hz.svipenyu.cn/gtiomriiju.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.andypj.xyz/gtxghkadvx.html

C#:   static void Main(string[] args)
来源：http://hz.smart0.xyz/gtltfuwjrv.html

[M08] 获取系统与运行时信息
来源：http://hz.gzhubu.top/gtybywmupr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yonumen.top/gtaqdhrkhd.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.mhx1999.top/gtzabnfhel.html

JS:   process.platform;  process.version
来源：http://hz.zhaomingkeji.xyz/gtvutixdzj.html

TS:   process.platform;  process.version
来源：http://hz.fzhhl.top/gtghwshwze.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hammf.cn/gttfpsmkmt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.aibaodan.cn/gtvmocfbcu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinqigfzy.top/gtrrqtoxet.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shuidangran.top/gtuxahvxwz.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtgtmnyylo.html

N. 数据结构与算法
来源：http://hz.hammf.cn/gtqpzdhmfx.html

================================================================================
来源：http://hz.yueranfly.top/gtnubagsxi.html

[N01] 二分查找（有序数组）
来源：http://hz.snrcjt.cn/gtnqdjelvp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ppjwa.cn/gtdsdpnycd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hywenlv.cn/gtuybzumfw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dashuyun.cn/gtubjkvuvi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shanyushiyangtech.top/gttgtnveaw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jqgfzy.top/gtizdhduny.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ydzc1.top/gtgcqjvhex.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.gogol.net.cn/gtivmomhot.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.havefunace.top/gteqrngtme.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.aizwys.cn/gtwgbqgksr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tanke756.top/gtvetvgyka.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jyoumei.cn/gthxkrzscm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yanxiufei.cn/gtmvywiixr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtkjbzoidm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hywenlv.cn/gtebmswkxz.html

Go:   slices.Sort(arr)
来源：http://hz.gogol.net.cn/gtjzifzivg.html

Ruby: arr.sort
来源：http://hz.daxiang520.top/gtmuiinyph.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.mhx1999.top/gttuzlxmoa.html

[N03] 快速排序（分治示例）
来源：http://hz.redwolf501.top/gtpxfrkjdg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yj20258888.top/gtwyboeadl.html

PHP:  // 递归实现，或用 usort
来源：http://hz.feifeiyinyue.top/gtfswnzlva.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.birdmap.top/gtiybpwzlg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.bjfxy.top/gttnoppavt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhongyouzk.top/gtezsnrfqg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yvedp.cn/gtruubwefy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.aibaodan.cn/gtgshxkfuq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.aizwys.cn/gtqhlihhrb.html

[N04] 斐波那契数列
来源：http://hz.shanyushiyangkeji.top/gtxyjudqtn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hongshengwenyu.top/gtpkiprlfr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.meibo888.top/gtnspoayna.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.guowangkeji.top/gtcsniawpx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gtunhxtvul.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.chenjidiqi.icu/gtcbbyhbkg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ppjwa.cn/gtiodskciz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.0kj1m.cn/gtbwvbtzmm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gogol.net.cn/gteplhxqhi.html

[N05] 最大公约数
来源：http://hz.hywenlv.cn/gtrmmtsnrg.html

Py:   math.gcd(a, b)
来源：http://hz.zdqjudy.top/gtbcftwwwv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shangyingyoupin.top/gtolkjnlew.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pycfn.com/gtychlxkcy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sweek.top/gtunraurgm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shanyushiyangkeji.top/gtokhfkvmy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jyoumei.cn/gtmvlprjwx.html

Ruby: a.gcd(b)
来源：http://hz.gzhubu.top/gtlvioejoc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gaohongyu789.top/gtgsuohawp.html

[N06] 判断回文字符串
来源：http://hz.yuxming.cn/gtzdhjeqod.html

Py:   s == s[::-1]
来源：http://hz.hnxiangtu.top/gtceazevpm.html

PHP:  $s === strrev($s);
来源：http://hz.snrcjt.cn/gtbvqeiavl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtzmnynvxo.html

TS:   s === [...s].reverse().join("")
来源：http://hz.fzhhl.top/gtssjykeqo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.kuanghao11.cn/gtipjykktd.html

Go:   // 双指针从两端比较
来源：http://hz.gogol.net.cn/gtoxdxnjhc.html

Ruby: s == s.reverse
来源：http://hz.pengpengdd.cyou/gtwxhkvpjg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangtech.top/gtyrxqodpr.html

[N07] 两数之和（返回下标）
来源：http://hz.yj20258888.top/gtkpeyjvwa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xingfuxueyuan.xyz/gtzpwqnrmf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jinqigufen.top/gtvceanyfa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinqigfzy.top/gtqhivvcpb.html

TS:   // 手写 Map<string, number>
来源：http://hz.yueranfly.top/gtndehisku.html

Java: // 手写 HashMap
来源：http://hz.zhiwuduotai.top/gtqjvkslbp.html

Go:   // 手写 map[int]int
来源：http://hz.zhijiandao.cn/gthvvltobz.html

Ruby: // 手写 Hash
来源：http://hz.ivvv.top/gtnjhahvju.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hfpthk.cn/gthplvvqpy.html

[N08] 生成全排列
来源：http://hz.zhijiandao.cn/gtogfcflbo.html

Py:   itertools.permutations(arr)
来源：http://hz.xziqi.cn/gtoifgasmq.html

PHP:  // 手写递归交换
来源：http://hz.xuanzx.com/gtsnzfysvk.html

JS:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtojrpbbgw.html

TS:   // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtcwpwmsuw.html

Java: // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtxusrefya.html

Go:   // 手写回溯递归
来源：http://hz.yvedp.cn/gtrxkfovkv.html

Ruby: arr.permutation.to_a
来源：http://hz.zhiwuduotai.top/gtfvelvovb.html

C#:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtwmndbmuy.html

[N09] 栈与队列
来源：http://hz.svipenyu.cn/gtolvevrau.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.fzhhl.top/gtglzfkuyw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.wangshuangyany.cn/gtebejugtt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.9152youxi.cn/gtbbakypei.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shuidangran.top/gtygzwwjqf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinqigufen.top/gtqumlxhoh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.wangdashe.top/gtjpyuyvuo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jiagoushi.top/gttdjhnmdc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhongyouzk.top/gtjhdrswym.html

[N10] 链表节点定义
来源：http://hz.hysaishi.cn/gtrpdxfhlq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yonumen.top/gtzcsredwu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cdnleiting.top/gtkgpjcvyt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jqgfzy.top/gtcpawkkbz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhiwuduotai.top/gtlgkpknte.html

Java: class Node { int v; Node next; }
来源：http://hz.hysaishi.cn/gtdrcxubex.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gaohongyu789.top/gthcgdvqar.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.guannengcc.top/gtbmnbuokg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yangfankeji.com/gtwtzvcimg.html

[N11] 二叉树中序遍历
来源：http://hz.ydzc1.top/gtlynnrzno.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinghuilouyu.cn/gtfgnzcgfw.html

PHP:  // 手写递归函数
来源：http://hz.chenjidiqi.icu/gtpbpkepqk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sweek.top/gtgjiikpat.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sufxvd.cn/gtymzfvbqj.html

Java: // 手写递归
来源：http://hz.cucudq.cn/gttncaokmd.html

Go:   // 手写递归
来源：http://hz.shangyingyoupin.top/gtmynjwtmn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ivvv.top/gtixeqbbee.html

C#:   // 手写递归
来源：http://hz.yj20258.top/gtfibzjhgh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhoulong.xyz/gtkenrbnsz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.fengsongda.top/gtwywtcmte.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.daxiang520.top/gtyaduvegp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.mhx1999.top/gtfquuznii.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.quarkkingdee.top/gtlubnknlc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.52xcode.cn/gtzuqnqkvk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.9152youxi.cn/gtrijijvqr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.aibaodan.cn/gtbuscxpcu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenjidiqi.icu/gtwdhobder.html

================================================================================
来源：http://hz.iojbl.cn/gtprkpokcp.html

O. 并发与异步
来源：http://hz.shanyushiyangtech.top/gtvxlwkpag.html

================================================================================
来源：http://hz.dashuyun.cn/gtuntzaiyc.html

[O01] 启动一个线程
来源：http://hz.yj202588.top/gtobuqoyra.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.chenjidiqi.icu/gthjhqxuss.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hywenlv.cn/gtkknwmfze.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhengqikj.top/gtuhyibguq.html

TS:   // 同 JS
来源：http://hz.gogol.net.cn/gtjrnivpzb.html

Java: new Thread(() -> f()).start()
来源：http://hz.sufxvd.cn/gtotwtzngh.html

Go:   go f()
来源：http://hz.jinqigfzy.top/gtoncsvhhf.html

Ruby: Thread.new { f }
来源：http://hz.hywenlv.cn/gtfamphdpj.html

C#:   Task.Run(() => F());
来源：http://hz.svipenyu.cn/gtlggmnkxv.html

[O02] 使用线程池
来源：http://hz.cheryme.top/gtyamvxtqe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.meibo888.top/gtsyirgndu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ywan-chungtsiang.top/gtidvgsvob.html

JS:   // worker_threads 线程池
来源：http://hz.jlsjyb.cn/gtptrqhkfs.html

TS:   // worker_threads 线程池
来源：http://hz.yvedp.cn/gtnnfurmgv.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.havefunace.top/gtzqjhevdk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ywan-chungtsiang.top/gtahuaavia.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xingfuxueyuan.xyz/gtbluemjfy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xylfe.cn/gtvcakcghg.html

[O03] 加锁保护共享数据
来源：http://hz.sxryk.cn/gtottqvbyu.html

Py:   with lock: shared += 1
来源：http://hz.shangyingyoupin.top/gtitmjvdcy.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.fengsongda.top/gtbqslecfz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yangfankeji.com/gttkoxndav.html

TS:   // 同 JS
来源：http://hz.chenlongwang.top/gtphsenhfv.html

Java: synchronized (this) { shared++; }
来源：http://hz.jlsjyb.cn/gtpncqeaim.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xinyue.icu/gtuxdmwwje.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.birdmap.top/gtxjztpkxu.html

C#:   lock (gate) { shared++; }
来源：http://hz.daria6918.cn/gtiwboanji.html

[O04] 定义异步函数并等待
来源：http://hz.52xcode.cn/gtdqotvxhe.html

Py:   async def f():⏎    await g()
来源：http://hz.nanxinkj.top/gtrrwmatcc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nwbrower.top/gtobvioslq.html

JS:   async function f() { await g(); }
来源：http://hz.guannengcc.top/gtvkusqlzp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cucudq.cn/gtzgegwqks.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.guowangkeji.top/gtizicqcdp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yangfankeji.com/gtttmperzq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xziqi.cn/gtabjsdwes.html

C#:   async Task F() { await G(); }
来源：http://hz.yvedp.cn/gtaaqawctx.html

[O05] 并发执行并等待全部完成
来源：http://hz.bjfxy.top/gtnhiwcapq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.bjfxy.top/gtfitposzy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.svipenyu.cn/gtyaicrdvx.html

JS:   await Promise.all(tasks)
来源：http://hz.zhaomingkeji.xyz/gtcyoqwwea.html

TS:   await Promise.all(tasks)
来源：http://hz.sxryk.cn/gtphxsdusf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hnqzz.top/gtddxknoun.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xylfe.cn/gtzyauxfhw.html

Ruby: threads.map(&:join)
来源：http://hz.yvedp.cn/gtcyqfleeg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhengqikj.top/gtvnbshxbi.html

[O06] 使用进程池
来源：http://hz.yj202588.top/gtptdkwese.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yuxming.cn/gtecnrnshx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.pycfn.com/gtudmztosr.html

JS:   // child_process / cluster 模块
来源：http://hz.redwolf501.top/gtvudjzhnj.html

TS:   // child_process / cluster 模块
来源：http://hz.iojbl.cn/gthhribdod.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.nanxinkj.top/gttwiywtke.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xingfuxueyuan.xyz/gtztvoxpwr.html

Ruby: // fork 块
来源：http://hz.wangshuangyany.cn/gtcqgslyil.html

C#:   Parallel.For
来源：http://hz.nanxuanxn.top/gtxfaxlzbj.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gttsvcarst.html

P. 常用工具函数
来源：http://hz.cqqwz.cn/gtnppsnqgk.html

================================================================================
来源：http://hz.vqdsnc.cn/gtxtpnljnh.html


<!-- 参考信息 -->