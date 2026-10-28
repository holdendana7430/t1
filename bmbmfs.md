代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.andypj.xyz/gtldompwyz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sysykeji.top/gtvqulbuao.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yuanzhike.top/gthzrwwgxc.html

Py:   pickle.dumps(obj)
来源：http://hz.dianchejie.cn/gtokxhtkzl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xylfe.cn/gtdvtzsyfn.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.daria6918.cn/gtyabxafft.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.wangdashe.top/gtrkecqvjz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.snrcjt.cn/gtetzewozq.html

Go:   encoding/gob
来源：http://hz.yongpay.top/gtrdxuowyo.html

Ruby: Marshal.dump(obj)
来源：http://hz.birdmap.top/gtolxopnxg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenjidiqi.icu/gtggerqzak.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtbxmwwemi.html

L. 网络请求
来源：http://hz.pycfn.com/gtylzmfufl.html

================================================================================
来源：http://hz.aibaodan.cn/gtusvcnzes.html

[L01] 发送 GET 请求
来源：http://hz.pycfn.com/gtdvphobda.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tian-w.cn/gtmcnlbyyh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hongshengwenyu.top/gtqfcsvzpi.html

JS:   await fetch(url)
来源：http://hz.52xcode.cn/gtxoacvyqm.html

TS:   await fetch(url)
来源：http://hz.yueranfly.top/gtxaqggaep.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hongshengwenyu.top/gtssyojxad.html

Go:   resp, err := http.Get(url)
来源：http://hz.yonumen.top/gtfnpcpiii.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hammf.cn/gthygteeug.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xziqi.cn/gtlqxmtzef.html

[L02] 发送 POST JSON
来源：http://hz.pengpengdd.cyou/gtgtrngqlw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hongshengwenyu.top/gtzwsuohdh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cqqwz.cn/gtuvizxjqp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhijiandao.cn/gtgrlrfidp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.kuanghao11.cn/gtkbhicvlr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.meibo888.top/gtlbdcevgy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.birdmap.top/gtrqpqsgvl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.chenzaomai.com/gtdorjfbel.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.chenjidiqi.icu/gtkxfchyxw.html

[L03] 设置自定义请求头
来源：http://hz.fengsongda.top/gtoxwqziay.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.daxiang520.top/gtesqjizcx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.52xcode.cn/gtzaspxwcb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.smart0.xyz/gtnebehhrw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnqzz.top/gtaqpcyvok.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xylfe.cn/gtkrdasdgh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.kuanghao11.cn/gtbzcstbey.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yvedp.cn/gtxqvnxggf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ydzc1.top/gtcacbulgj.html

[L04] 设置超时
来源：http://hz.jqgufenzy.top/gtoalffvue.html

Py:   requests.get(url, timeout=5)
来源：http://hz.pengpengdd.cyou/gtjmelxcxu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinyuanbaomall.cn/gtqqucsadv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.andypj.xyz/gtmbagqsjj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenjidiqi.icu/gtzgisjbrk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hammf.cn/gtpgqqoglj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sxryk.cn/gtzaklfrri.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhoulong.xyz/gtaxowkevx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zycfv.cn/gtbsynocwr.html

[L05] 上传文件（multipart）
来源：http://hz.aizwys.cn/gtoxwbschb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.svipenyu.cn/gtlmykmged.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hysaishi.cn/gtcpienuph.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigfzy.top/gtddadzxrx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.havefunace.top/gtitngwbef.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhiwuduotai.top/gtyyzdmbpi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yonumen.top/gtgobyrfdc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.dashuyun.cn/gtruzqaaym.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ywan-chungtsiang.top/gtqotykcbf.html

[L06] 解析响应为 JSON
来源：http://hz.cdnleiting.top/gtjoymgtvj.html

Py:   resp.json()
来源：http://hz.daria6918.cn/gtpboxxlmo.html

PHP:  json_decode($body, true);
来源：http://hz.yuanzhike.top/gtfltzakyp.html

JS:   await resp.json()
来源：http://hz.hywenlv.cn/gttffexumj.html

TS:   await resp.json()
来源：http://hz.feifeiyinyue.top/gtkbfgvwsz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yonumen.top/gtzbpkwysb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sweek.top/gtlalsyjjz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yuxming.cn/gtsvnyedsy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yj20258.top/gtpfhqudcb.html

[L07] 处理 HTTP 状态码
来源：http://hz.ybcxt.top/gteitbztzl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jiagoushi.top/gtwdaakvmm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.guowangkeji.top/gtsfuuweqo.html

JS:   resp.ok;  resp.status
来源：http://hz.vqdsnc.cn/gtvtjvvjle.html

TS:   resp.ok;  resp.status
来源：http://hz.xylfe.cn/gtflsilpij.html

Java: resp.statusCode()
来源：http://hz.c1oappe.top/gtwhsevbhb.html

Go:   resp.StatusCode
来源：http://hz.pengpengdd.cyou/gtamrmcazb.html

Ruby: resp.code.to_i
来源：http://hz.xylfe.cn/gteqttuqti.html

C#:   (int)resp.StatusCode
来源：http://hz.xuetiantiany.cn/gtebwsarwe.html

[L08] 并发请求多个地址
来源：http://hz.ydjk.org.cn/gtgzwpnhsv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zdqjudy.top/gtztuhozak.html

PHP:  curl_multi_init() 系列
来源：http://hz.xylfe.cn/gtizzbponc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuanzx.com/gtkjzyrlhr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hysaishi.cn/gtgoaeqjyx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sysykeji.top/gtdawjxvwk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhixingplan.top/gtuthmwtml.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.vqdsnc.cn/gtjpmyypjj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ybcxt.top/gtlptyxgce.html

================================================================================
来源：http://hz.cheryme.top/gthmzlpppo.html

M. 命令行 / 进程 / 环境
来源：http://hz.iojbl.cn/gtnilelysd.html

================================================================================
来源：http://hz.cucudq.cn/gtllqgptod.html

[M01] 读取命令行参数
来源：http://hz.ehwqpu.com/gtxuyehoeb.html

Py:   sys.argv[1:]
来源：http://hz.yvedp.cn/gtsfbpcfpb.html

PHP:  $argv;  $argc;
来源：http://hz.sufxvd.cn/gtbmmkkyyw.html

JS:   process.argv.slice(2)
来源：http://hz.xziqi.cn/gtpctibaek.html

TS:   process.argv.slice(2)
来源：http://hz.guowangkeji.top/gtihvtzgui.html

Java: args 数组（main 方法参数）
来源：http://hz.yj202588.top/gtepseotik.html

Go:   os.Args[1:]
来源：http://hz.guannengcc.top/gtdzjcipvh.html

Ruby: ARGV
来源：http://hz.bjfxy.top/gtoxfxatco.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenzaomai.com/gtstwrrldi.html

[M02] 读取环境变量
来源：http://hz.yj202588.top/gtcuxzbxym.html

Py:   os.environ.get("HOME")
来源：http://hz.yvedp.cn/gtbtevntwf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenjidiqi.icu/gtcynglmkr.html

JS:   process.env.HOME
来源：http://hz.cheryme.top/gtnjcqamkj.html

TS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtfqcgyzjp.html

Java: System.getenv("HOME")
来源：http://hz.tian-w.cn/gtparquxup.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cashguo.top/gtjacqsbni.html

Ruby: ENV["HOME"]
来源：http://hz.chenjidiqi.icu/gtljmxvelk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.guannengcc.top/gtzlatdgoe.html

[M03] 执行外部命令
来源：http://hz.jinyuanbaomall.cn/gtehxmasit.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj20258.top/gtokvwdojb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.snrcjt.cn/gtexjylzwp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangtech.top/gtrwongdmf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shuidangran.top/gtvdodmbom.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.dianchejie.cn/gtjhvmdolj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ybcxt.top/gtkmirnyjn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sweek.top/gtaxkxjlte.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yj202588.top/gtmvcclgit.html

[M04] 获取当前工作目录
来源：http://hz.yj20258.top/gtmjinwheb.html

Py:   os.getcwd()
来源：http://hz.shangyingyoupin.top/gtgxtonqke.html

PHP:  getcwd();
来源：http://hz.shangyingyoupin.top/gtmxnztfdr.html

JS:   process.cwd()
来源：http://hz.pycfn.com/gtwjxsuqwt.html

TS:   process.cwd()
来源：http://hz.bjfxy.top/gtrjoujrsp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.vqdsnc.cn/gteyezrkfe.html

Go:   os.Getwd()
来源：http://hz.wangdashe.top/gtmpxstypd.html

Ruby: Dir.pwd
来源：http://hz.snrcjt.cn/gtpefzvyem.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.guowangkeji.top/gtwyeyjimx.html

[M05] 设置退出码
来源：http://hz.ppjwa.cn/gtpmffaisu.html

Py:   sys.exit(1)
来源：http://hz.jinyuanbaomall.cn/gttkfzuzck.html

PHP:  exit(1);
来源：http://hz.nwbrower.top/gtfxwmaddi.html

JS:   process.exit(1)
来源：http://hz.yj202588.top/gtkmvywvzk.html

TS:   process.exit(1)
来源：http://hz.yuanzhike.top/gtrrrcujla.html

Java: System.exit(1)
来源：http://hz.c1oappe.top/gthfrlyidf.html

Go:   os.Exit(1)
来源：http://hz.hnxiangtu.top/gtfpvinojv.html

Ruby: exit 1
来源：http://hz.vqdsnc.cn/gtkgbsaeei.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xziqi.cn/gtmqyzpluk.html

[M06] 向标准错误输出
来源：http://hz.guannengcc.top/gtfqprthgl.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shangyingyoupin.top/gtasudbtmm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xuanzx.com/gtarxdnwsg.html

JS:   console.error("err")
来源：http://hz.hnqzz.top/gtnnrdbumj.html

TS:   console.error("err")
来源：http://hz.kuanghao11.cn/gtqiyakarx.html

Java: System.err.println("err")
来源：http://hz.mhx1999.top/gtqvytzqqi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.c1oappe.top/gtdayvgpfs.html

Ruby: warn "err"
来源：http://hz.jyoumei.cn/gtoapthepb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.snrcjt.cn/gtmqmlsiob.html

[M07] 判断是否为主入口
来源：http://hz.jianghu66.top/gtcsyebfdt.html

Py:   if __name__ == "__main__":
来源：http://hz.iojbl.cn/gtbzznxors.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gogol.net.cn/gtimumqfov.html

JS:   require.main === module
来源：http://hz.yj20258.top/gtuswaerke.html

TS:   require.main === module
来源：http://hz.nanxuanxn.top/gtnkemiyqz.html

Java: public static void main(String[] args)
来源：http://hz.jqgufenzy.top/gtpsggvzju.html

Go:   func main()
来源：http://hz.zhiwuduotai.top/gthalnhpti.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hongshengwenyu.top/gtplynczhx.html

C#:   static void Main(string[] args)
来源：http://hz.daxiang520.top/gtgpdcgpmk.html

[M08] 获取系统与运行时信息
来源：http://hz.nanxinkj.top/gtatnwfbpa.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinghuilouyu.cn/gtghnjkpgy.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.dashuyun.cn/gthmahmjmz.html

JS:   process.platform;  process.version
来源：http://hz.yongpay.top/gtyiqanqyw.html

TS:   process.platform;  process.version
来源：http://hz.yongpay.top/gtujxdxiix.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.dianchejie.cn/gtzkefakep.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xingfuxueyuan.xyz/gtwldfmpms.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cqqwz.cn/gtkdvircsj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ivvv.top/gtpvsogoqw.html

================================================================================
来源：http://hz.aizwys.cn/gtnmfoffxk.html

N. 数据结构与算法
来源：http://hz.cheryme.top/gtbwlbakli.html

================================================================================
来源：http://hz.yueranfly.top/gtqrdslalr.html

[N01] 二分查找（有序数组）
来源：http://hz.yvedp.cn/gtgkhwshbj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shzxlz.cn/gtiboxzgzn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shangyingyoupin.top/gtyxvxehej.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhiwuduotai.top/gtovsriffk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sweek.top/gtsltegefw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.iojbl.cn/gtinlgbdet.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.daxiang520.top/gtbcrwbrfd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.guannengcc.top/gtvqlhzzqv.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.wangshuangyany.cn/gtdfotfmuv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jyoumei.cn/gthvxaoyus.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jqgufenzy.top/gtqobctmbl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xuetiantiany.cn/gtkgfrlyqm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daria6918.cn/gtezqwyzte.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jlsjyb.cn/gtwnpdncnr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yonumen.top/gttomvvbnm.html

Go:   slices.Sort(arr)
来源：http://hz.tanke756.top/gtholbbkrm.html

Ruby: arr.sort
来源：http://hz.yanxiufei.cn/gtwanyowet.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zdqjudy.top/gthnmvdzxo.html

[N03] 快速排序（分治示例）
来源：http://hz.svipenyu.cn/gthvjgqbll.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jianghu66.top/gtijfouhyu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cucudq.cn/gthnzdylik.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yvedp.cn/gtzhnzweps.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.redwolf501.top/gtjnhzoqjn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tian-w.cn/gtbdzhisma.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jiagoushi.top/gtbgxraqpy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.meibo888.top/gtkfezhwra.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.quarkkingdee.top/gtdphtdjhe.html

[N04] 斐波那契数列
来源：http://hz.birdmap.top/gtufqdvevb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hywenlv.cn/gtccolvgux.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.vqdsnc.cn/gtahxguzby.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ybcxt.top/gtvvmysbkp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenjidiqi.icu/gtmhdwrtzs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xinyue.icu/gtqoaatovn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xziqi.cn/gtralulfku.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jqgufenzy.top/gtpgohbekx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xylfe.cn/gtkrzmbdsz.html

[N05] 最大公约数
来源：http://hz.yj20258.top/gtgmuzsgyw.html

Py:   math.gcd(a, b)
来源：http://hz.fzhhl.top/gtnfjjdnik.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yangfankeji.com/gttgvhfkqd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pycfn.com/gtfzsxeplv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.svipenyu.cn/gtmuxrmkan.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.wangshuangyany.cn/gtjsumnerg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenlongwang.top/gthuuzfemh.html

Ruby: a.gcd(b)
来源：http://hz.zhongyouzk.top/gtxcnbtekq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhengqikj.top/gtvtuntwwg.html

[N06] 判断回文字符串
来源：http://hz.ivvv.top/gteuaxctmz.html

Py:   s == s[::-1]
来源：http://hz.nwbrower.top/gtccrjspen.html

PHP:  $s === strrev($s);
来源：http://hz.cqqwz.cn/gtxzuzgjib.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtizhlojtq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtyiriiaqh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jqgfzy.top/gtgahkhiuu.html

Go:   // 双指针从两端比较
来源：http://hz.zhongyouzk.top/gtidppzgkm.html

Ruby: s == s.reverse
来源：http://hz.0kj1m.cn/gthohnbnmd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ppjwa.cn/gtjuexverf.html

[N07] 两数之和（返回下标）
来源：http://hz.jqgufenzy.top/gtivkyndwk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.guannengcc.top/gtfedfmvjb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shanyushiyangtech.top/gtlyqywmsc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.svipenyu.cn/gtknaozoes.html

TS:   // 手写 Map<string, number>
来源：http://hz.yvedp.cn/gtrydhtvhq.html

Java: // 手写 HashMap
来源：http://hz.dianchejie.cn/gtjldwolyv.html

Go:   // 手写 map[int]int
来源：http://hz.gaohongyu789.top/gtkwewgbga.html

Ruby: // 手写 Hash
来源：http://hz.haohaochexian.top/gttnfyasrw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cucudq.cn/gtlylummgb.html

[N08] 生成全排列
来源：http://hz.hongshengwenyu.top/gtygdlswjr.html

Py:   itertools.permutations(arr)
来源：http://hz.yj202588.top/gtxwlgobya.html

PHP:  // 手写递归交换
来源：http://hz.yanxiufei.cn/gtziucamke.html

JS:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtiejvcsfa.html

TS:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtzmpufmcq.html

Java: // 手写回溯递归
来源：http://hz.zhongyouzk.top/gtcfcajhyv.html

Go:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtmfkvmxhc.html

Ruby: arr.permutation.to_a
来源：http://hz.yj202588.top/gtdsjlgpil.html

C#:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtsenslsvw.html

[N09] 栈与队列
来源：http://hz.ehwqpu.com/gtheeaowyz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.chenlongwang.top/gtykniddzp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.shzxlz.cn/gtthqzssnn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.meibo888.top/gtupfgtstk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj20258.top/gtjiyuerek.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhengqikj.top/gthxvzfmdy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zycfv.cn/gtuproiads.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jinyuanbaomall.cn/gtiffsthas.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shanyushiyangtech.top/gtenfjqwkk.html

[N10] 链表节点定义
来源：http://hz.pycfn.com/gthqpczapz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shanyushiyangkeji.top/gtwoznlgyz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.svipenyu.cn/gtlbkvjqbf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhoulong.xyz/gtbqydnmgx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.nwbrower.top/gtidtxmjkj.html

Java: class Node { int v; Node next; }
来源：http://hz.ybcxt.top/gtlmigqldx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.9152youxi.cn/gtukogqdwi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.svipenyu.cn/gtlvxymwvb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.tanke756.top/gtdhotjgah.html

[N11] 二叉树中序遍历
来源：http://hz.hywenlv.cn/gtvfrwhvax.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhongyouzk.top/gtsezvxvzw.html

PHP:  // 手写递归函数
来源：http://hz.tanke756.top/gtlalzguov.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ivvv.top/gtekemeijy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.52xcode.cn/gtayjzdmjz.html

Java: // 手写递归
来源：http://hz.ydjk.org.cn/gtzbbkohbc.html

Go:   // 手写递归
来源：http://hz.xuetiantiany.cn/gtivdqdqpf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhijiandao.cn/gtgfmyzkdz.html

C#:   // 手写递归
来源：http://hz.gotoacloud.top/gtivqhbpdi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.svipenyu.cn/gtuzveifxt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jyoumei.cn/gtkvocohuf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cheryme.top/gttivabqsw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhiwuduotai.top/gtkvliymrn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.c1oappe.top/gtpmqtqpxt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258.top/gtrwkknfas.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ydzc1.top/gtnlnjyofk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zdqjudy.top/gtciazxcid.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pycfn.com/gtahtelbpd.html

================================================================================
来源：http://hz.yj20258888.top/gtigcwdhyw.html

O. 并发与异步
来源：http://hz.kuanghao11.cn/gtiwyoupzv.html

================================================================================
来源：http://hz.yongpay.top/gtskkllzwt.html

[O01] 启动一个线程
来源：http://hz.tian-w.cn/gtaueekore.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.kuanghao11.cn/gtxjakhjyv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shanyushiyangkeji.top/gtkvturykm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.sxryk.cn/gtegfxothl.html

TS:   // 同 JS
来源：http://hz.jinqigufen.top/gtwjobjoys.html

Java: new Thread(() -> f()).start()
来源：http://hz.daxiang520.top/gtnjxbzbon.html

Go:   go f()
来源：http://hz.yvedp.cn/gtlgtckciu.html

Ruby: Thread.new { f }
来源：http://hz.shzxlz.cn/gtnsxvylle.html

C#:   Task.Run(() => F());
来源：http://hz.jianghu66.top/gtjohjpcfe.html

[O02] 使用线程池
来源：http://hz.xuanzx.com/gtzadaphif.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ivvv.top/gtldzbzhsh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yuxming.cn/gtlcequicn.html

JS:   // worker_threads 线程池
来源：http://hz.tian-w.cn/gtxilbdblv.html

TS:   // worker_threads 线程池
来源：http://hz.sufxvd.cn/gtjqaaaeuj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cheryme.top/gtrcxtujuf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ydjk.org.cn/gtfdresycf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.dianchejie.cn/gtemdjfvak.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hongshengwenyu.top/gtzdwvhbjz.html

[O03] 加锁保护共享数据
来源：http://hz.zycfv.cn/gtizzuevyq.html

Py:   with lock: shared += 1
来源：http://hz.xziqi.cn/gtjgyksbhi.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.daria6918.cn/gtsmxlbvoo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.nwbrower.top/gtxdprndxr.html

TS:   // 同 JS
来源：http://hz.jinghuilouyu.cn/gtoljktggc.html

Java: synchronized (this) { shared++; }
来源：http://hz.wangdashe.top/gtbimzklps.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.mhx1999.top/gtnzfrnlws.html


<!-- 参考信息 -->