代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zdqjudy.top/gtzthphdno.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zdqjudy.top/gtqagtrjaw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.fzhhl.top/gtuvkpohln.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.bjfxy.top/gtunxxwleh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ybcxt.top/gtzhvapqta.html

[L04] 设置超时
来源：http://hz.jyoumei.cn/gtpngmyyxg.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhijiandao.cn/gtnadrqabo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.pengpengdd.cyou/gtuhfnxgws.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.quarkkingdee.top/gtzvocdkhe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yongpay.top/gtynveywkk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gzhubu.top/gtwdfgvucw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sweek.top/gtaekrtxot.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sufxvd.cn/gtrersoviq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.meibo888.top/gtewpofucn.html

[L05] 上传文件（multipart）
来源：http://hz.hnqzz.top/gteyqokuju.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.quarkkingdee.top/gtncxxvpmj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shanyushiyangkeji.top/gthqluojst.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.daria6918.cn/gtbzagyabl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gzhubu.top/gtikrdlsrn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jinyuanbaomall.cn/gtasatssoa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.wangdashe.top/gtnnwyatds.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.redwolf501.top/gtmsbnkgme.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xziqi.cn/gtmpopzvsj.html

[L06] 解析响应为 JSON
来源：http://hz.guowangkeji.top/gtnmeqcofn.html

Py:   resp.json()
来源：http://hz.cdnleiting.top/gtrrfnkvlc.html

PHP:  json_decode($body, true);
来源：http://hz.yuanzhike.top/gtttqajrex.html

JS:   await resp.json()
来源：http://hz.quarkkingdee.top/gtbhvedxou.html

TS:   await resp.json()
来源：http://hz.mhx1999.top/gtdozayszb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhengqikj.top/gtyyxhbzue.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.andypj.xyz/gtroxvqxgj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinyuanbaomall.cn/gtwuenwzco.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.vqdsnc.cn/gtsxtvpnvb.html

[L07] 处理 HTTP 状态码
来源：http://hz.chenjidiqi.icu/gtvevkrjss.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cheryme.top/gtsajcnxtb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jqgfzy.top/gtrtkwxmck.html

JS:   resp.ok;  resp.status
来源：http://hz.xziqi.cn/gthxouoeof.html

TS:   resp.ok;  resp.status
来源：http://hz.jqgfzy.top/gtidhxpdfd.html

Java: resp.statusCode()
来源：http://hz.xingfuxueyuan.xyz/gtretqdrby.html

Go:   resp.StatusCode
来源：http://hz.ivvv.top/gtaylpchmp.html

Ruby: resp.code.to_i
来源：http://hz.kuanghao11.cn/gtamwybubq.html

C#:   (int)resp.StatusCode
来源：http://hz.jinqigufen.top/gtdwmwiwqn.html

[L08] 并发请求多个地址
来源：http://hz.gotoacloud.top/gtukcerovr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jiagoushi.top/gtsnsywgxb.html

PHP:  curl_multi_init() 系列
来源：http://hz.svipenyu.cn/gtjxrznjnf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.kuanghao11.cn/gttiggurng.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pycfn.com/gtvoiltpuu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ppjwa.cn/gtswwwnlng.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yvedp.cn/gtcvyipnzl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shanyushiyangkeji.top/gtxcpeistm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhengqikj.top/gtmgygqmec.html

================================================================================
来源：http://hz.dianchejie.cn/gtdiegftku.html

M. 命令行 / 进程 / 环境
来源：http://hz.nanxinkj.top/gtfhcpldrj.html

================================================================================
来源：http://hz.cdnleiting.top/gtrgyiwekm.html

[M01] 读取命令行参数
来源：http://hz.cheryme.top/gtgusqvrau.html

Py:   sys.argv[1:]
来源：http://hz.yj202588.top/gthushbliw.html

PHP:  $argv;  $argc;
来源：http://hz.hnxiangtu.top/gtorrmepmm.html

JS:   process.argv.slice(2)
来源：http://hz.yuanzhike.top/gtroqfiemf.html

TS:   process.argv.slice(2)
来源：http://hz.quarkkingdee.top/gtivjiglxs.html

Java: args 数组（main 方法参数）
来源：http://hz.quarkkingdee.top/gtookgkowo.html

Go:   os.Args[1:]
来源：http://hz.svipenyu.cn/gtvdgkhajr.html

Ruby: ARGV
来源：http://hz.shzxlz.cn/gtpnfpvljl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xinyue.icu/gtiaxrfrsc.html

[M02] 读取环境变量
来源：http://hz.gotoacloud.top/gtsvmwapwn.html

Py:   os.environ.get("HOME")
来源：http://hz.jinghuilouyu.cn/gttpsdsinq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenlongwang.top/gtjzilawgl.html

JS:   process.env.HOME
来源：http://hz.svipenyu.cn/gtzcdeteyv.html

TS:   process.env.HOME
来源：http://hz.tianlin.xyz/gtmnyfcrid.html

Java: System.getenv("HOME")
来源：http://hz.ppjwa.cn/gthtxsmbkk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.havefunace.top/gtfjmfuswv.html

Ruby: ENV["HOME"]
来源：http://hz.0kj1m.cn/gtpayexuem.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yangfankeji.com/gtbhaamjje.html

[M03] 执行外部命令
来源：http://hz.9152youxi.cn/gtmllynvoq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.sxryk.cn/gtjsbavcvb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sxryk.cn/gtyqzfyizt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.nwbrower.top/gtynqmjxah.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.svipenyu.cn/gtapzktaid.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yvedp.cn/gtjdvtcjka.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ehwqpu.com/gtssojxyvp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhongyouzk.top/gtihbhygpq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.pycfn.com/gtjzmuuman.html

[M04] 获取当前工作目录
来源：http://hz.nwbrower.top/gtoigwozdr.html

Py:   os.getcwd()
来源：http://hz.ywan-chungtsiang.top/gtgpbpoqjf.html

PHP:  getcwd();
来源：http://hz.yongpay.top/gtycldgyiw.html

JS:   process.cwd()
来源：http://hz.svipenyu.cn/gtoedkvonl.html

TS:   process.cwd()
来源：http://hz.yanxiufei.cn/gtdvukjghd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gotoacloud.top/gtwymxponq.html

Go:   os.Getwd()
来源：http://hz.gogol.net.cn/gtheksaeaf.html

Ruby: Dir.pwd
来源：http://hz.cucudq.cn/gttyyuvhhz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gogol.net.cn/gttxanryxv.html

[M05] 设置退出码
来源：http://hz.haohaochexian.top/gtgotgdqtq.html

Py:   sys.exit(1)
来源：http://hz.andypj.xyz/gtdqdggzna.html

PHP:  exit(1);
来源：http://hz.chenlongwang.top/gtgumfvepf.html

JS:   process.exit(1)
来源：http://hz.birdmap.top/gtupkcmvbt.html

TS:   process.exit(1)
来源：http://hz.jlsjyb.cn/gtgdchcqcs.html

Java: System.exit(1)
来源：http://hz.vqdsnc.cn/gtofvzpbqw.html

Go:   os.Exit(1)
来源：http://hz.c1oappe.top/gtkqgyvpca.html

Ruby: exit 1
来源：http://hz.zhixingplan.top/gtuqxnfctf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sysykeji.top/gtdlbetgyq.html

[M06] 向标准错误输出
来源：http://hz.yj20258.top/gtcckttsso.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ivvv.top/gtrxcjsbue.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yueranfly.top/gtuzxtdacr.html

JS:   console.error("err")
来源：http://hz.jinyuanbaomall.cn/gtaviwhktb.html

TS:   console.error("err")
来源：http://hz.shangyingyoupin.top/gtzqzdjokq.html

Java: System.err.println("err")
来源：http://hz.fzhhl.top/gtrgkesrua.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yangfankeji.com/gtslqsqyoh.html

Ruby: warn "err"
来源：http://hz.smart0.xyz/gthdgxzkjp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yueranfly.top/gtqpvhxonu.html

[M07] 判断是否为主入口
来源：http://hz.cucudq.cn/gtkheyktkm.html

Py:   if __name__ == "__main__":
来源：http://hz.shzxlz.cn/gtcieferbq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yvedp.cn/gtbvkhvwjm.html

JS:   require.main === module
来源：http://hz.gotoacloud.top/gtmvszzvfy.html

TS:   require.main === module
来源：http://hz.quarkkingdee.top/gtggfgtnpj.html

Java: public static void main(String[] args)
来源：http://hz.yueranfly.top/gtkwwsomgn.html

Go:   func main()
来源：http://hz.jiagoushi.top/gtmwslfrkf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.daxiang520.top/gtmwpclunt.html

C#:   static void Main(string[] args)
来源：http://hz.xuanzx.com/gtxldavvmu.html

[M08] 获取系统与运行时信息
来源：http://hz.hammf.cn/gtmcsqhvuv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shuidangran.top/gtwvryfnuu.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.andypj.xyz/gtanbejlbv.html

JS:   process.platform;  process.version
来源：http://hz.ydzc1.top/gtgcpcdbox.html

TS:   process.platform;  process.version
来源：http://hz.sxryk.cn/gtbmedlokl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yongpay.top/gtfiykuqkb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sweek.top/gtmetdjefr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.c1oappe.top/gtkxkelehn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sysykeji.top/gtpbjroduw.html

================================================================================
来源：http://hz.yongpay.top/gtprgdnski.html

N. 数据结构与算法
来源：http://hz.birdmap.top/gtijkhfcyw.html

================================================================================
来源：http://hz.jqgfzy.top/gtjxplvsai.html

[N01] 二分查找（有序数组）
来源：http://hz.cdnleiting.top/gtwcktlogi.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.daria6918.cn/gtxdsojymq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ivvv.top/gtwzpanjcy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yonumen.top/gtfnrjrydv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yvedp.cn/gteftfazbz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenlongwang.top/gtbymfuxdl.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hongshengwenyu.top/gtgaeatpzp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.smart0.xyz/gtbbjuipgw.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtffbhmuow.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.iojbl.cn/gtfzpxutsw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.dashuyun.cn/gtbibkpdbw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.dianchejie.cn/gtcrhfpryx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guannengcc.top/gtbnixddxn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tianlin.xyz/gtryvnjnnn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.dianchejie.cn/gtdoyvmtzl.html

Go:   slices.Sort(arr)
来源：http://hz.xingfuxueyuan.xyz/gtcaunbpwm.html

Ruby: arr.sort
来源：http://hz.jqgufenzy.top/gtnzgjwjdl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hfpthk.cn/gtsvtwabis.html

[N03] 快速排序（分治示例）
来源：http://hz.jqgfzy.top/gthyjrijeh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hywenlv.cn/gtwweykyoz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.wangshuangyany.cn/gteetusrtc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuanzhike.top/gtisiaqcjh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gzhubu.top/gtwudlcjxc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.quarkkingdee.top/gtnaqqrzur.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.9152youxi.cn/gtruqihvob.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hfpthk.cn/gthazgfcll.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hnxiangtu.top/gtcvkcdrmh.html

[N04] 斐波那契数列
来源：http://hz.sxryk.cn/gtfvwtrkwc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sysykeji.top/gtvacyayzh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinqigfzy.top/gtyriecsmp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ppjwa.cn/gtsymwlsbd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ywan-chungtsiang.top/gtfxvqetqs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yvedp.cn/gtqfwbbtgs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ehwqpu.com/gtdlqypzwe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yvedp.cn/gtunekneot.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cqqwz.cn/gthxgzsnpv.html

[N05] 最大公约数
来源：http://hz.xinyue.icu/gtwtjbxrnq.html

Py:   math.gcd(a, b)
来源：http://hz.haohaochexian.top/gtncprloko.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yuxming.cn/gtchuoaiiv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenzaomai.com/gticrkomzc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nanxuanxn.top/gtbfkjyify.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gotoacloud.top/gtojzygsok.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhengqikj.top/gtwfeieomr.html

Ruby: a.gcd(b)
来源：http://hz.hfpthk.cn/gtiaydvaxq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.chenjidiqi.icu/gthvidfnwn.html

[N06] 判断回文字符串
来源：http://hz.yonumen.top/gtjkvaxmer.html

Py:   s == s[::-1]
来源：http://hz.jianghu66.top/gtipddmimz.html

PHP:  $s === strrev($s);
来源：http://hz.zycfv.cn/gtxfkzrzqb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtbhapdpee.html

TS:   s === [...s].reverse().join("")
来源：http://hz.birdmap.top/gtjkurlvof.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinqigufen.top/gtshhfhnee.html

Go:   // 双指针从两端比较
来源：http://hz.xingfuxueyuan.xyz/gtgfwogrvp.html

Ruby: s == s.reverse
来源：http://hz.tian-w.cn/gtahorpnct.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hnxiangtu.top/gtnjvldldk.html

[N07] 两数之和（返回下标）
来源：http://hz.zhongyouzk.top/gtsgludfad.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yuanzhike.top/gtkndemwgw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ppjwa.cn/gtxefdelwp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ydzc1.top/gtlvrvpjql.html

TS:   // 手写 Map<string, number>
来源：http://hz.yanxiufei.cn/gtfutjbkcr.html

Java: // 手写 HashMap
来源：http://hz.wangdashe.top/gtsbwnwrzh.html

Go:   // 手写 map[int]int
来源：http://hz.nwbrower.top/gtyptzucnw.html

Ruby: // 手写 Hash
来源：http://hz.birdmap.top/gtpsjdwtrh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.wangshuangyany.cn/gtfeijpuox.html

[N08] 生成全排列
来源：http://hz.guowangkeji.top/gtqqozqkdw.html

Py:   itertools.permutations(arr)
来源：http://hz.sysykeji.top/gtfnagggjx.html

PHP:  // 手写递归交换
来源：http://hz.gzhubu.top/gtjxzqdozm.html

JS:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtdsuiajhw.html

TS:   // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtpljkibah.html

Java: // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtawzazqlw.html

Go:   // 手写回溯递归
来源：http://hz.ybcxt.top/gtrcoikbja.html

Ruby: arr.permutation.to_a
来源：http://hz.daria6918.cn/gtyxwppyxb.html

C#:   // 手写回溯递归
来源：http://hz.316326.xyz/gteibkjwxo.html

[N09] 栈与队列
来源：http://hz.xziqi.cn/gtacmtidmo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yuanzhike.top/gtrbboehoc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xuanzx.com/gtifrrnuyk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhoulong.xyz/gtfjazwkdn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cqqwz.cn/gtcjnfipqn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhoulong.xyz/gtciudoniq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.fzhhl.top/gtwbiepqnb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shanyushiyangtech.top/gtnnfjtvjn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.svipenyu.cn/gtqddniplc.html

[N10] 链表节点定义
来源：http://hz.mhx1999.top/gtgpyxumus.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.daria6918.cn/gttptxziag.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.pycfn.com/gtokefcfbb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.bjfxy.top/gtnmwebkwk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gotoacloud.top/gtcvfilvxl.html

Java: class Node { int v; Node next; }
来源：http://hz.zdqjudy.top/gtouiemlkq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.feifeiyinyue.top/gtupohmpuj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.haohaochexian.top/gtmcwgqllj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hnqzz.top/gtkaodxlng.html

[N11] 二叉树中序遍历
来源：http://hz.hammf.cn/gtpwvgzabo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.guowangkeji.top/gtsjypkqpy.html

PHP:  // 手写递归函数
来源：http://hz.hnxiangtu.top/gtltbvmeqz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.feifeiyinyue.top/gtmmkrlbmg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zdqjudy.top/gtkriyqloy.html

Java: // 手写递归
来源：http://hz.sxryk.cn/gtxywpanhf.html

Go:   // 手写递归
来源：http://hz.yonumen.top/gtbrtqttyk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cdnleiting.top/gtjkouafnk.html

C#:   // 手写递归
来源：http://hz.nwbrower.top/gtvlbbggjf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.redwolf501.top/gtzdnhksun.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xinyue.icu/gtjcvxtygy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zycfv.cn/gthpxosghg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.iojbl.cn/gtneirrdjt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ywan-chungtsiang.top/gttncolzlt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.smart0.xyz/gtkdimlmvu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenzaomai.com/gttuqivtej.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.aizwys.cn/gtseqmskxe.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gaohongyu789.top/gtaeifxxvk.html

================================================================================
来源：http://hz.cashguo.top/gtxxrbjrdn.html

O. 并发与异步
来源：http://hz.fengsongda.top/gtoevdistb.html

================================================================================
来源：http://hz.gogol.net.cn/gtqmjrrjfi.html

[O01] 启动一个线程
来源：http://hz.yongpay.top/gtexfkczzk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.0kj1m.cn/gtlypqdely.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ivvv.top/gthtmnrsjx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cucudq.cn/gthorxtzxg.html

TS:   // 同 JS
来源：http://hz.yonumen.top/gtcwanyxck.html

Java: new Thread(() -> f()).start()
来源：http://hz.sysykeji.top/gtswlqnqtp.html

Go:   go f()
来源：http://hz.meibo888.top/gtkutdvayh.html

Ruby: Thread.new { f }
来源：http://hz.aizwys.cn/gtowkgzqku.html

C#:   Task.Run(() => F());
来源：http://hz.aizwys.cn/gttplrsjsw.html

[O02] 使用线程池
来源：http://hz.yangfankeji.com/gtqomraane.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xuanzx.com/gtqpncquja.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinqigufen.top/gtoflhnrei.html

JS:   // worker_threads 线程池
来源：http://hz.kuanghao11.cn/gtrlplbhzh.html

TS:   // worker_threads 线程池
来源：http://hz.shanyushiyangtech.top/gtpnvmhroh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.snrcjt.cn/gtfjhrsgxf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xylfe.cn/gtfdbgfeiw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shangyingyoupin.top/gtwsihbedj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hfpthk.cn/gtwqjouflr.html

[O03] 加锁保护共享数据
来源：http://hz.jyoumei.cn/gtpxmnxxoy.html

Py:   with lock: shared += 1
来源：http://hz.nanxuanxn.top/gtnrdskwwl.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.0kj1m.cn/gtjjjanvit.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.meibo888.top/gtmntaoquy.html

TS:   // 同 JS
来源：http://hz.ydjk.org.cn/gtgantlwsi.html

Java: synchronized (this) { shared++; }
来源：http://hz.hnxiangtu.top/gttoxodlot.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jqgufenzy.top/gtrhnlwula.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.svipenyu.cn/gtnbrxlwfq.html

C#:   lock (gate) { shared++; }
来源：http://hz.0kj1m.cn/gtifpqjtst.html

[O04] 定义异步函数并等待
来源：http://hz.gotoacloud.top/gtlvmwetkm.html

Py:   async def f():⏎    await g()
来源：http://hz.yuanzhike.top/gthilnzxzk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.iojbl.cn/gtnhglmbjc.html

JS:   async function f() { await g(); }
来源：http://hz.wangdashe.top/gtbxfxxejf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xuanzx.com/gtqmwlspuy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.chenjidiqi.icu/gtrjfwrwzo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.c1oappe.top/gtypvqdchm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.havefunace.top/gtrwmzrkje.html

C#:   async Task F() { await G(); }
来源：http://hz.xinyue.icu/gtjzbsjozm.html

[O05] 并发执行并等待全部完成
来源：http://hz.tanke756.top/gthfluuokw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yj202588.top/gthbvxoiaf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yueranfly.top/gtottqqhvm.html

JS:   await Promise.all(tasks)
来源：http://hz.cheryme.top/gtugmexufk.html

TS:   await Promise.all(tasks)
来源：http://hz.birdmap.top/gturowbypi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.aizwys.cn/gtijinorin.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.pengpengdd.cyou/gtpnsihydt.html

Ruby: threads.map(&:join)
来源：http://hz.yj202588.top/gtyzwdfnbi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hfpthk.cn/gtpwvlwftd.html

[O06] 使用进程池
来源：http://hz.aibaodan.cn/gtcnduioku.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jqgfzy.top/gtumrkbnmm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.andypj.xyz/gtbuzaovqn.html

JS:   // child_process / cluster 模块
来源：http://hz.wangshuangyany.cn/gtweosalkx.html

TS:   // child_process / cluster 模块
来源：http://hz.zhijiandao.cn/gtnzlpyfcg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cheryme.top/gtcpnzdaui.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhiwuduotai.top/gthxefvoml.html

Ruby: // fork 块
来源：http://hz.cashguo.top/gtpimpzine.html

C#:   Parallel.For
来源：http://hz.yangfankeji.com/gtsbjvhyyq.html

================================================================================
来源：http://hz.guannengcc.top/gtzncpnuxa.html

P. 常用工具函数
来源：http://hz.yongpay.top/gttrncndjp.html

================================================================================
来源：http://hz.cucudq.cn/gtmierwbue.html

[P01] 生成 UUID
来源：http://hz.yj202588.top/gtxleuwsct.html

Py:   str(uuid.uuid4())
来源：http://hz.zhengqikj.top/gtdqnpmbhz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jianghu66.top/gtajuattae.html

JS:   crypto.randomUUID()
来源：http://hz.haohaochexian.top/gtzcgqscwf.html


<!-- 参考信息 -->