代发 wailian999

[L03] 设置自定义请求头
来源：http://hz.fzhhl.top/gtrcfbvrxo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.fengsongda.top/gtaprswart.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gaohongyu789.top/gtoifmlxpn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yvedp.cn/gttvmjmoxj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hfpthk.cn/gtxeyzigim.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.feifeiyinyue.top/gthizrvoec.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinghuilouyu.cn/gtybtaycwy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jlsjyb.cn/gtilsjifcm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.9152youxi.cn/gtofdikjwo.html

[L04] 设置超时
来源：http://hz.cashguo.top/gttbbhjeff.html

Py:   requests.get(url, timeout=5)
来源：http://hz.havefunace.top/gtmimdvcnl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yanxiufei.cn/gtdzbrsfdp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.birdmap.top/gtkuvknggf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenlongwang.top/gtqgujdmcr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xuetiantiany.cn/gthmnjgqff.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.fzhhl.top/gtbwgtoplu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.chenjidiqi.icu/gttvwnsmhv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.daria6918.cn/gtwsafdoqe.html

[L05] 上传文件（multipart）
来源：http://hz.chenlongwang.top/gtuatnwxym.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.mhx1999.top/gtmuuvqjgy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.316326.xyz/gtbmojzpxt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.kuanghao11.cn/gtdomlpmry.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ivvv.top/gtwyjexadh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gzhubu.top/gtmkyggccc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhixingplan.top/gtebmjytzy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.svipenyu.cn/gtzbfzyfiv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hammf.cn/gtmgqcuocx.html

[L06] 解析响应为 JSON
来源：http://hz.hywenlv.cn/gtrshuhpek.html

Py:   resp.json()
来源：http://hz.yuanzhike.top/gtiyogczmv.html

PHP:  json_decode($body, true);
来源：http://hz.mhx1999.top/gtqzfonsbe.html

JS:   await resp.json()
来源：http://hz.birdmap.top/gtfwqtbypw.html

TS:   await resp.json()
来源：http://hz.shanyushiyangtech.top/gtsovndlum.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hywenlv.cn/gtalpjnrgy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.daria6918.cn/gtkurrhszx.html

Ruby: JSON.parse(resp.body)
来源：http://hz.redwolf501.top/gthkmtdfye.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.fzhhl.top/gtaxxrecox.html

[L07] 处理 HTTP 状态码
来源：http://hz.iojbl.cn/gtgxhvewcu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yanxiufei.cn/gthdlrhwax.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.chenjidiqi.icu/gthdmntuhj.html

JS:   resp.ok;  resp.status
来源：http://hz.daria6918.cn/gtxbymtqra.html

TS:   resp.ok;  resp.status
来源：http://hz.zhoulong.xyz/gtsrzelfcx.html

Java: resp.statusCode()
来源：http://hz.yj202588.top/gtgrvzpatr.html

Go:   resp.StatusCode
来源：http://hz.zhengqikj.top/gtomafxtqq.html

Ruby: resp.code.to_i
来源：http://hz.jinqigufen.top/gtcrkjgsxq.html

C#:   (int)resp.StatusCode
来源：http://hz.hnqzz.top/gtjrfohamq.html

[L08] 并发请求多个地址
来源：http://hz.daria6918.cn/gtvwllfxjo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jqgfzy.top/gtlhyiukkc.html

PHP:  curl_multi_init() 系列
来源：http://hz.jqgfzy.top/gtlwxsuage.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.andypj.xyz/gtomgpxtrq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuxming.cn/gtvczoszsy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.316326.xyz/gtricyuupo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.316326.xyz/gttqlyfssp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.daria6918.cn/gtpcoakzsp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ehwqpu.com/gtjdmaqebz.html

================================================================================
来源：http://hz.316326.xyz/gtkkysdvdd.html

M. 命令行 / 进程 / 环境
来源：http://hz.iojbl.cn/gtcyyjnpmv.html

================================================================================
来源：http://hz.jyoumei.cn/gteolyqpuw.html

[M01] 读取命令行参数
来源：http://hz.yongpay.top/gtrcmvsmwf.html

Py:   sys.argv[1:]
来源：http://hz.yongpay.top/gtncasfojj.html

PHP:  $argv;  $argc;
来源：http://hz.tianlin.xyz/gtcbnnsugx.html

JS:   process.argv.slice(2)
来源：http://hz.guowangkeji.top/gtjbvhiiqy.html

TS:   process.argv.slice(2)
来源：http://hz.daria6918.cn/gtjsxliqgy.html

Java: args 数组（main 方法参数）
来源：http://hz.sweek.top/gtsklhbech.html

Go:   os.Args[1:]
来源：http://hz.ppjwa.cn/gtjuzrxhqu.html

Ruby: ARGV
来源：http://hz.yuxming.cn/gtwetrhqyd.html

C#:   args 数组（Main 方法参数）
来源：http://hz.snrcjt.cn/gtromljhco.html

[M02] 读取环境变量
来源：http://hz.pengpengdd.cyou/gtzvwdgsah.html

Py:   os.environ.get("HOME")
来源：http://hz.tanke756.top/gtdiptjqxw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yj20258.top/gtinuaymoq.html

JS:   process.env.HOME
来源：http://hz.nwbrower.top/gtbpyibewg.html

TS:   process.env.HOME
来源：http://hz.ehwqpu.com/gttkptsyrj.html

Java: System.getenv("HOME")
来源：http://hz.yonumen.top/gtmwwztwmb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jiagoushi.top/gtfreivzay.html

Ruby: ENV["HOME"]
来源：http://hz.ydzc1.top/gthhdouwav.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shangyingyoupin.top/gtcxivfigj.html

[M03] 执行外部命令
来源：http://hz.feifeiyinyue.top/gtmmrssjsr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj20258888.top/gtburzlxne.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.haohaochexian.top/gtmjxmtwsa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yangfankeji.com/gtdzwcdlyv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.feifeiyinyue.top/gtumsqpnlg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj20258888.top/gtcvoixbdz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hongshengwenyu.top/gtxldpfwcy.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.52xcode.cn/gtyrshbvrp.html

C#:   Process.Start("ls", "-l");
来源：http://hz.quarkkingdee.top/gtvgcqupqy.html

[M04] 获取当前工作目录
来源：http://hz.zhijiandao.cn/gtqfqrkgof.html

Py:   os.getcwd()
来源：http://hz.dianchejie.cn/gtqwtynnvq.html

PHP:  getcwd();
来源：http://hz.hammf.cn/gtkjqaqiwl.html

JS:   process.cwd()
来源：http://hz.sufxvd.cn/gtjjohldgq.html

TS:   process.cwd()
来源：http://hz.yuanzhike.top/gtdqxlrgcs.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cheryme.top/gtbrvucdnv.html

Go:   os.Getwd()
来源：http://hz.jinqigfzy.top/gtnxourxgb.html

Ruby: Dir.pwd
来源：http://hz.ybcxt.top/gtdkyrzaqr.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.mhx1999.top/gtlwldnynd.html

[M05] 设置退出码
来源：http://hz.havefunace.top/gtiavstnhv.html

Py:   sys.exit(1)
来源：http://hz.dianchejie.cn/gtokmmista.html

PHP:  exit(1);
来源：http://hz.cucudq.cn/gtlerhfaxf.html

JS:   process.exit(1)
来源：http://hz.meibo888.top/gtrgbsigqk.html

TS:   process.exit(1)
来源：http://hz.tanke756.top/gtqoiyttom.html

Java: System.exit(1)
来源：http://hz.meibo888.top/gtogikcood.html

Go:   os.Exit(1)
来源：http://hz.hammf.cn/gtwzxnhjcj.html

Ruby: exit 1
来源：http://hz.jqgufenzy.top/gtbdovhzph.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hnqzz.top/gtepcjylms.html

[M06] 向标准错误输出
来源：http://hz.hnxiangtu.top/gtdctzkvhh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gogol.net.cn/gtdovewagx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.havefunace.top/gtxefuymsj.html

JS:   console.error("err")
来源：http://hz.ivvv.top/gtqjbeyvkv.html

TS:   console.error("err")
来源：http://hz.havefunace.top/gtwdbnxwci.html

Java: System.err.println("err")
来源：http://hz.sysykeji.top/gtcfbfzpqi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hfpthk.cn/gtwnkzbyqp.html

Ruby: warn "err"
来源：http://hz.ehwqpu.com/gtrjagsfld.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.nanxinkj.top/gtnrotgbbd.html

[M07] 判断是否为主入口
来源：http://hz.pycfn.com/gtesjzwmbj.html

Py:   if __name__ == "__main__":
来源：http://hz.gzhubu.top/gterzbfwwk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ehwqpu.com/gtribhfskc.html

JS:   require.main === module
来源：http://hz.fengsongda.top/gtzvuskwde.html

TS:   require.main === module
来源：http://hz.zhoulong.xyz/gtdbsrnlqi.html

Java: public static void main(String[] args)
来源：http://hz.tanke756.top/gtlfaykajk.html

Go:   func main()
来源：http://hz.xinyue.icu/gtkdgotfxi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jqgfzy.top/gtlnxrhhhi.html

C#:   static void Main(string[] args)
来源：http://hz.gzhubu.top/gtporecqlc.html

[M08] 获取系统与运行时信息
来源：http://hz.aizwys.cn/gtumtyazea.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jiagoushi.top/gtullkqaeb.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jinyuanbaomall.cn/gtbhvripnp.html

JS:   process.platform;  process.version
来源：http://hz.hongshengwenyu.top/gtleashsdb.html

TS:   process.platform;  process.version
来源：http://hz.wangdashe.top/gtzokcalip.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gotoacloud.top/gtqcxgqqav.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.bjfxy.top/gtzjtlxjvb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinqigufen.top/gtharstctl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.feifeiyinyue.top/gtmnzwaoek.html

================================================================================
来源：http://hz.zhijiandao.cn/gtyxtkrpdq.html

N. 数据结构与算法
来源：http://hz.yuxming.cn/gtoxvzymfz.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtyvsmyvcc.html

[N01] 二分查找（有序数组）
来源：http://hz.xinyue.icu/gtcijoukdt.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hysaishi.cn/gtpcyptlji.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xziqi.cn/gtosoaiiwj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ywan-chungtsiang.top/gtjxeijnhk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cashguo.top/gtzkqtupdj.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhixingplan.top/gtqmvvppwj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtptchqqva.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.nanxuanxn.top/gtguzhpgti.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yonumen.top/gttqhihkre.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jianghu66.top/gtryugudrb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenzaomai.com/gtvtmznssi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jyoumei.cn/gtmyvoqtgg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangtech.top/gtwzsamdpg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.pycfn.com/gtqndicaxc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yueranfly.top/gtwezzqdaa.html

Go:   slices.Sort(arr)
来源：http://hz.jinyuanbaomall.cn/gtorooaera.html

Ruby: arr.sort
来源：http://hz.ydjk.org.cn/gthsfflhda.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.daria6918.cn/gtfdevuyjz.html

[N03] 快速排序（分治示例）
来源：http://hz.kuanghao11.cn/gtkvnmzlxt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.wangdashe.top/gtpitrmkej.html

PHP:  // 递归实现，或用 usort
来源：http://hz.haohaochexian.top/gtynjfnoii.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gogol.net.cn/gtzgukactf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhoulong.xyz/gtodtxmpau.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cdnleiting.top/gtwtdhqdue.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.feifeiyinyue.top/gtogrwvjzz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yj20258888.top/gtlgcwdgej.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gotoacloud.top/gtdzkirsyp.html

[N04] 斐波那契数列
来源：http://hz.mhx1999.top/gtakbgwtun.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xinyue.icu/gtqgaxqjlr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sysykeji.top/gtvwlopndo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.guannengcc.top/gtxfivhwme.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yonumen.top/gtwhxybofz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.fengsongda.top/gtejmxduqp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hfpthk.cn/gtwjvwqtmz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.daria6918.cn/gtzpsisleo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gaohongyu789.top/gttymjkjzl.html

[N05] 最大公约数
来源：http://hz.daria6918.cn/gtqgoeunra.html

Py:   math.gcd(a, b)
来源：http://hz.ehwqpu.com/gtzhdavvyx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.fengsongda.top/gtbkongxwn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fengsongda.top/gtzkjeghff.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gtyufndlkt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ybcxt.top/gtjyisfzmm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xingfuxueyuan.xyz/gtyqovrkbx.html

Ruby: a.gcd(b)
来源：http://hz.yj20258.top/gtpcrghrrd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.chenzaomai.com/gtqoysofds.html

[N06] 判断回文字符串
来源：http://hz.ywan-chungtsiang.top/gtgelaeunk.html

Py:   s == s[::-1]
来源：http://hz.ydjk.org.cn/gtalmqyncc.html

PHP:  $s === strrev($s);
来源：http://hz.ydjk.org.cn/gtwohvqwzs.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtzpqbhfzj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gtaitvzkuu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.nanxuanxn.top/gtovkhtyhs.html

Go:   // 双指针从两端比较
来源：http://hz.sysykeji.top/gtzzktjdfb.html

Ruby: s == s.reverse
来源：http://hz.52xcode.cn/gtvjxrhrvv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gzhubu.top/gtsfxultlt.html

[N07] 两数之和（返回下标）
来源：http://hz.chenlongwang.top/gtopsexrhs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.guowangkeji.top/gtmdszqdla.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.nanxuanxn.top/gtbeiahpht.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.redwolf501.top/gtlvanmohr.html

TS:   // 手写 Map<string, number>
来源：http://hz.hfpthk.cn/gtrejhicrg.html

Java: // 手写 HashMap
来源：http://hz.iojbl.cn/gtwqsmmgrt.html

Go:   // 手写 map[int]int
来源：http://hz.wangdashe.top/gtzsluruom.html

Ruby: // 手写 Hash
来源：http://hz.dashuyun.cn/gtvgtxpysy.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.tanke756.top/gtjkyhnvgj.html

[N08] 生成全排列
来源：http://hz.shuidangran.top/gtzilkafzc.html

Py:   itertools.permutations(arr)
来源：http://hz.shuidangran.top/gtkpvpfkkf.html

PHP:  // 手写递归交换
来源：http://hz.sweek.top/gtmpeghdfu.html

JS:   // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtbsmoqwvk.html

TS:   // 手写回溯递归
来源：http://hz.yuanzhike.top/gtrbeeaigw.html

Java: // 手写回溯递归
来源：http://hz.kuanghao11.cn/gtteihwcgd.html

Go:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtvinomptg.html

Ruby: arr.permutation.to_a
来源：http://hz.ybcxt.top/gtjhmjuizw.html

C#:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtibuckmos.html

[N09] 栈与队列
来源：http://hz.xuanzx.com/gtqezrbagw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.pengpengdd.cyou/gtndrvnpdf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ivvv.top/gtbjrhgmpa.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhoulong.xyz/gthqwyzncx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.aibaodan.cn/gtejrdeyeq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhijiandao.cn/gtfgtorerq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhijiandao.cn/gtxyexcgdf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.chenjidiqi.icu/gthkxyzefg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hysaishi.cn/gtdabllzln.html

[N10] 链表节点定义
来源：http://hz.gzhubu.top/gtgdvehcdx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shzxlz.cn/gtpleszyex.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.nanxinkj.top/gtqxuwocld.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yonumen.top/gtxddewzci.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gotoacloud.top/gtrfbwbdcv.html

Java: class Node { int v; Node next; }
来源：http://hz.xinyue.icu/gtdcebmpsl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.wangdashe.top/gtaiwsyhlk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ivvv.top/gtapdsxdll.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xziqi.cn/gtwsvkmhzc.html

[N11] 二叉树中序遍历
来源：http://hz.chenlongwang.top/gtpfrucdks.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sysykeji.top/gtlmjiydzd.html

PHP:  // 手写递归函数
来源：http://hz.sxryk.cn/gtnyvivhnz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.daria6918.cn/gtstogtzfq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gaohongyu789.top/gtshqmhboy.html

Java: // 手写递归
来源：http://hz.shzxlz.cn/gtdsemazyv.html

Go:   // 手写递归
来源：http://hz.jyoumei.cn/gteoiwpskb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jinyuanbaomall.cn/gtigsnztkp.html

C#:   // 手写递归
来源：http://hz.9152youxi.cn/gtadwphhgl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xziqi.cn/gtslmkyuhx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.aibaodan.cn/gtyfcdritp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sysykeji.top/gtmijcyzxp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.meibo888.top/gtcamcatco.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dashuyun.cn/gtadayporh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hnqzz.top/gtgkrgrbkk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.feifeiyinyue.top/gtbrirnczb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.aibaodan.cn/gtezlujkvc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuanzx.com/gtcqwokabj.html

================================================================================
来源：http://hz.yuxming.cn/gtcpfxjwou.html

O. 并发与异步
来源：http://hz.yangfankeji.com/gtwzemboow.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtuhhfuiem.html

[O01] 启动一个线程
来源：http://hz.guowangkeji.top/gtaczwvyhj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yuanzhike.top/gtxzhaarqg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shuidangran.top/gtiltezdje.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yj20258.top/gtitewvejs.html

TS:   // 同 JS
来源：http://hz.jlsjyb.cn/gtaenejsjf.html

Java: new Thread(() -> f()).start()
来源：http://hz.xylfe.cn/gtinuntohh.html

Go:   go f()
来源：http://hz.jinqigufen.top/gterrylecg.html

Ruby: Thread.new { f }
来源：http://hz.cqqwz.cn/gtmicuinxn.html

C#:   Task.Run(() => F());
来源：http://hz.xingfuxueyuan.xyz/gtaxjffstu.html

[O02] 使用线程池
来源：http://hz.kuanghao11.cn/gtkyklkncv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shanyushiyangkeji.top/gtzsutpvoo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shanyushiyangtech.top/gtcytlnvnh.html

JS:   // worker_threads 线程池
来源：http://hz.zhijiandao.cn/gtdbvdnqhg.html

TS:   // worker_threads 线程池
来源：http://hz.zhixingplan.top/gtsgssyset.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinqigfzy.top/gtwavpflgw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yonumen.top/gtfadcwtec.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhiwuduotai.top/gtpcrzpabn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.sweek.top/gtwqpugwjf.html

[O03] 加锁保护共享数据
来源：http://hz.haohaochexian.top/gtvdqoviua.html

Py:   with lock: shared += 1
来源：http://hz.ppjwa.cn/gtcvvyuezz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.svipenyu.cn/gtbaibhjck.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xingfuxueyuan.xyz/gtiufowltx.html

TS:   // 同 JS
来源：http://hz.fengsongda.top/gtehpxdaqx.html

Java: synchronized (this) { shared++; }
来源：http://hz.iojbl.cn/gtgffcsrhc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.pycfn.com/gtugmwqqsx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jqgfzy.top/gttmrzpgye.html

C#:   lock (gate) { shared++; }
来源：http://hz.iojbl.cn/gtlnsedwbz.html

[O04] 定义异步函数并等待
来源：http://hz.ivvv.top/gtubbxdmlt.html

Py:   async def f():⏎    await g()
来源：http://hz.fzhhl.top/gtbkbplzpv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinghuilouyu.cn/gtpjaxtbeq.html

JS:   async function f() { await g(); }
来源：http://hz.yanxiufei.cn/gtfjdlrrxh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.daxiang520.top/gtvbjmijfz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xuanzx.com/gtexvrvlgd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.birdmap.top/gtbixldrjl.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhoulong.xyz/gtldyfdukt.html

C#:   async Task F() { await G(); }
来源：http://hz.zhixingplan.top/gtmwuaqgrt.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj202588.top/gtvztgknzw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jianghu66.top/gtsgzeenvm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zdqjudy.top/gtkdzfgkox.html

JS:   await Promise.all(tasks)
来源：http://hz.zhijiandao.cn/gtguohwdbf.html

TS:   await Promise.all(tasks)
来源：http://hz.zhoulong.xyz/gtdzoftfeo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jyoumei.cn/gtvlltqzpx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shzxlz.cn/gtwmmbmdde.html

Ruby: threads.map(&:join)
来源：http://hz.wangdashe.top/gtvsjkcrps.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.fzhhl.top/gtzqeeyylx.html

[O06] 使用进程池
来源：http://hz.gotoacloud.top/gtsrgcpjen.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.tianlin.xyz/gtgfznfouq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.birdmap.top/gtepjbmeyk.html

JS:   // child_process / cluster 模块
来源：http://hz.daria6918.cn/gtjfhhqtlt.html

TS:   // child_process / cluster 模块
来源：http://hz.ybcxt.top/gtczgrvqjp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinghuilouyu.cn/gtakqotfzm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zycfv.cn/gtuwiozjyo.html

Ruby: // fork 块
来源：http://hz.havefunace.top/gtemptismp.html

C#:   Parallel.For
来源：http://hz.sweek.top/gttncohnku.html

================================================================================
来源：http://hz.redwolf501.top/gtnchqrlcv.html

P. 常用工具函数
来源：http://hz.ydzc1.top/gtmobqthnz.html

================================================================================
来源：http://hz.yuxming.cn/gtanjixruy.html


<!-- 参考信息 -->