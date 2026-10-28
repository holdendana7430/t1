代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xinyue.icu/gtkvwhcoxt.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.meibo888.top/gtncdmiudh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shzxlz.cn/gtlxsfbbly.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj20258.top/gtksmygqbn.html

Go:   encoding/gob
来源：http://hz.cheryme.top/gtdzadgpdl.html

Ruby: Marshal.dump(obj)
来源：http://hz.ydzc1.top/gtnpenfksj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenlongwang.top/gthzforrea.html

================================================================================
来源：http://hz.fengsongda.top/gtvcmxlgid.html

L. 网络请求
来源：http://hz.jyoumei.cn/gtkdedyfwr.html

================================================================================
来源：http://hz.zhongyouzk.top/gtjlxdlfnv.html

[L01] 发送 GET 请求
来源：http://hz.316326.xyz/gtkbmuqalh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jlsjyb.cn/gtlmdmpmdj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ywan-chungtsiang.top/gttltrfrfg.html

JS:   await fetch(url)
来源：http://hz.gaohongyu789.top/gtbppuliep.html

TS:   await fetch(url)
来源：http://hz.feifeiyinyue.top/gtaebzyrwr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.snrcjt.cn/gtzoygoozm.html

Go:   resp, err := http.Get(url)
来源：http://hz.gogol.net.cn/gtxvgdgkdr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gotoacloud.top/gtgbmewunt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sweek.top/gtobxrwzup.html

[L02] 发送 POST JSON
来源：http://hz.pengpengdd.cyou/gtqwxvnqyo.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.dianchejie.cn/gtafujvuzc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.smart0.xyz/gtjybuxbcx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hfpthk.cn/gthmgdjzke.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangshuangyany.cn/gtzcjsqlue.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shangyingyoupin.top/gtwpofqwti.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhengqikj.top/gtokgpwkbt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yuxming.cn/gthrfzoswk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.vqdsnc.cn/gtykpkxplq.html

[L03] 设置自定义请求头
来源：http://hz.gotoacloud.top/gtrurovvhc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.chenzaomai.com/gthnvmbskj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jyoumei.cn/gtgfshioio.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigfzy.top/gtstawwgek.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.redwolf501.top/gtnljcepni.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.havefunace.top/gtgzhjewrg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenlongwang.top/gtrvhiamgq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ydjk.org.cn/gtwlgpvjzl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.c1oappe.top/gtrmuxxycg.html

[L04] 设置超时
来源：http://hz.sufxvd.cn/gtsrgfoxoa.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hysaishi.cn/gtcnovmbkz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hywenlv.cn/gtraaxbmuo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnqzz.top/gtqfmbcyxj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangdashe.top/gterjfcjeo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jyoumei.cn/gtuuyohnfz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.iojbl.cn/gtirxckshn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xuanzx.com/gtidbdrgwx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.c1oappe.top/gtfnfoehxk.html

[L05] 上传文件（multipart）
来源：http://hz.birdmap.top/gtmtwhzsff.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.daria6918.cn/gtyuutuhgz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gzhubu.top/gtuwkfkbim.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.kuanghao11.cn/gtcoixrode.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.meibo888.top/gtxckuxxux.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.andypj.xyz/gtnzyvvmuj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xingfuxueyuan.xyz/gtvagwdfof.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yj20258888.top/gtiokjgwhc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinghuilouyu.cn/gtgckwfddz.html

[L06] 解析响应为 JSON
来源：http://hz.316326.xyz/gtjxfnvtbh.html

Py:   resp.json()
来源：http://hz.jyoumei.cn/gtcrzxxyog.html

PHP:  json_decode($body, true);
来源：http://hz.jiagoushi.top/gtgcsrcgbd.html

JS:   await resp.json()
来源：http://hz.shangyingyoupin.top/gtiqavppea.html

TS:   await resp.json()
来源：http://hz.ppjwa.cn/gtkdslltuj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hfpthk.cn/gtaksnmsxg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.dashuyun.cn/gtdvmjaeof.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shangyingyoupin.top/gthenpgjst.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hnqzz.top/gtdxtzattp.html

[L07] 处理 HTTP 状态码
来源：http://hz.hfpthk.cn/gtxamjskmd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.52xcode.cn/gtsrkksoso.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.chenlongwang.top/gtajjovciz.html

JS:   resp.ok;  resp.status
来源：http://hz.jlsjyb.cn/gtsevypasd.html

TS:   resp.ok;  resp.status
来源：http://hz.hongshengwenyu.top/gttfqkcujk.html

Java: resp.statusCode()
来源：http://hz.daxiang520.top/gtldmmqgrj.html

Go:   resp.StatusCode
来源：http://hz.tian-w.cn/gtvospicca.html

Ruby: resp.code.to_i
来源：http://hz.svipenyu.cn/gtciimlevj.html

C#:   (int)resp.StatusCode
来源：http://hz.cashguo.top/gtwgclowqh.html

[L08] 并发请求多个地址
来源：http://hz.chenlongwang.top/gtcdtiksvz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ppjwa.cn/gttfxchmeg.html

PHP:  curl_multi_init() 系列
来源：http://hz.guannengcc.top/gtpfpxyrhj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuanzhike.top/gtoriilejo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gtzwovawrt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shanyushiyangkeji.top/gtavuqrasq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cqqwz.cn/gtrloeqgda.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ivvv.top/gtqlnyovic.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.9152youxi.cn/gtpmisvjdo.html

================================================================================
来源：http://hz.tianlin.xyz/gtinkxgqnp.html

M. 命令行 / 进程 / 环境
来源：http://hz.cucudq.cn/gthjfokuol.html

================================================================================
来源：http://hz.fengsongda.top/gtuleoqsno.html

[M01] 读取命令行参数
来源：http://hz.redwolf501.top/gtisepmznq.html

Py:   sys.argv[1:]
来源：http://hz.pengpengdd.cyou/gtghcsrplv.html

PHP:  $argv;  $argc;
来源：http://hz.gotoacloud.top/gtxmzxpcst.html

JS:   process.argv.slice(2)
来源：http://hz.yvedp.cn/gtkeaycsde.html

TS:   process.argv.slice(2)
来源：http://hz.hfpthk.cn/gtzqytzrbl.html

Java: args 数组（main 方法参数）
来源：http://hz.jiagoushi.top/gtabdyaush.html

Go:   os.Args[1:]
来源：http://hz.tianlin.xyz/gtjptdnqtx.html

Ruby: ARGV
来源：http://hz.shanyushiyangkeji.top/gtsqislicc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.tian-w.cn/gtzmtjbkja.html

[M02] 读取环境变量
来源：http://hz.smart0.xyz/gtlxfqoxjb.html

Py:   os.environ.get("HOME")
来源：http://hz.yj202588.top/gttobmdtel.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ydjk.org.cn/gttjwtsldt.html

JS:   process.env.HOME
来源：http://hz.jlsjyb.cn/gtinnhwvlo.html

TS:   process.env.HOME
来源：http://hz.wangdashe.top/gtvktyfrbe.html

Java: System.getenv("HOME")
来源：http://hz.wangdashe.top/gtkjatzmfv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xingfuxueyuan.xyz/gtiwzzlbiw.html

Ruby: ENV["HOME"]
来源：http://hz.zhixingplan.top/gtahlfxjof.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yvedp.cn/gtpzomhgqf.html

[M03] 执行外部命令
来源：http://hz.hywenlv.cn/gtgmueaxbu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.snrcjt.cn/gtvrvpworv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.52xcode.cn/gtmmaqdugb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigufen.top/gtiqbenbby.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.svipenyu.cn/gtinytfkxf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.aizwys.cn/gtmqqbsnjt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.0kj1m.cn/gtmgfbnfbr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cdnleiting.top/gtgewbkviz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hammf.cn/gtixsjihji.html

[M04] 获取当前工作目录
来源：http://hz.yj20258888.top/gtiukquhpg.html

Py:   os.getcwd()
来源：http://hz.xziqi.cn/gtumackyua.html

PHP:  getcwd();
来源：http://hz.ywan-chungtsiang.top/gtjhjmdnhe.html

JS:   process.cwd()
来源：http://hz.shzxlz.cn/gtnkuuztxa.html

TS:   process.cwd()
来源：http://hz.bjfxy.top/gtrnlzomvi.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.aibaodan.cn/gtrpucafem.html

Go:   os.Getwd()
来源：http://hz.zhiwuduotai.top/gtcidlabsu.html

Ruby: Dir.pwd
来源：http://hz.shuidangran.top/gtcoxvwefs.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gzhubu.top/gtncaohslf.html

[M05] 设置退出码
来源：http://hz.snrcjt.cn/gtpblvzdoq.html

Py:   sys.exit(1)
来源：http://hz.iojbl.cn/gtfduflpck.html

PHP:  exit(1);
来源：http://hz.nanxuanxn.top/gtxevsnpcs.html

JS:   process.exit(1)
来源：http://hz.aizwys.cn/gtbsevbjma.html

TS:   process.exit(1)
来源：http://hz.jlsjyb.cn/gtuepovsxw.html

Java: System.exit(1)
来源：http://hz.xziqi.cn/gtrzbqkaoz.html

Go:   os.Exit(1)
来源：http://hz.zhoulong.xyz/gtjzofbjwl.html

Ruby: exit 1
来源：http://hz.hongshengwenyu.top/gtpzhsniyp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jiagoushi.top/gtjwocflzy.html

[M06] 向标准错误输出
来源：http://hz.chenjidiqi.icu/gtiarpdenw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yangfankeji.com/gtbdhesquq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yueranfly.top/gtcenybdih.html

JS:   console.error("err")
来源：http://hz.ydjk.org.cn/gtogqsryra.html

TS:   console.error("err")
来源：http://hz.fzhhl.top/gtvafvsbaq.html

Java: System.err.println("err")
来源：http://hz.yueranfly.top/gtixozqjph.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.tanke756.top/gtghftsxiz.html

Ruby: warn "err"
来源：http://hz.ppjwa.cn/gtblhyvamo.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.havefunace.top/gtzjgxnvga.html

[M07] 判断是否为主入口
来源：http://hz.yvedp.cn/gtfwmxeoev.html

Py:   if __name__ == "__main__":
来源：http://hz.jlsjyb.cn/gtkckhmvbu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinqigfzy.top/gtdyjmnsdh.html

JS:   require.main === module
来源：http://hz.guannengcc.top/gtqbarznqw.html

TS:   require.main === module
来源：http://hz.cucudq.cn/gtqocxkpop.html

Java: public static void main(String[] args)
来源：http://hz.ydzc1.top/gtgnvtrhho.html

Go:   func main()
来源：http://hz.redwolf501.top/gtdoisjlgy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.0kj1m.cn/gtcijmhenp.html

C#:   static void Main(string[] args)
来源：http://hz.jinqigfzy.top/gtujxetjfm.html

[M08] 获取系统与运行时信息
来源：http://hz.hfpthk.cn/gtrlxpncgg.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinyuanbaomall.cn/gtftfqnlvv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.nanxuanxn.top/gtxbxsfbzg.html

JS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtgljdjlpz.html

TS:   process.platform;  process.version
来源：http://hz.quarkkingdee.top/gtdzhrhrfg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cucudq.cn/gtbtcnnasg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hfpthk.cn/gtifxrypqo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yonumen.top/gtbjijtgdl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.iojbl.cn/gtxrmvmcon.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtjawatlfu.html

N. 数据结构与算法
来源：http://hz.nanxuanxn.top/gthbasbmrm.html

================================================================================
来源：http://hz.haohaochexian.top/gtiainozqr.html

[N01] 二分查找（有序数组）
来源：http://hz.mhx1999.top/gtbbavfkrj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.tian-w.cn/gtzkczgipw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cqqwz.cn/gtmzytcnjb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.52xcode.cn/gtddmixtek.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhijiandao.cn/gtohsatnpi.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtuqnfmniy.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.guannengcc.top/gtnbtqhehf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hongshengwenyu.top/gtbpnnjhds.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.andypj.xyz/gthawejxqp.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.nwbrower.top/gtfklqixjx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sufxvd.cn/gtxsbpwrro.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.daxiang520.top/gtkehueyvk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gtvxeajcdm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuetiantiany.cn/gtwjipasig.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cashguo.top/gttlxkppga.html

Go:   slices.Sort(arr)
来源：http://hz.yvedp.cn/gtziddfdej.html

Ruby: arr.sort
来源：http://hz.shzxlz.cn/gtaaivbchy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.haohaochexian.top/gtaehfkgpv.html

[N03] 快速排序（分治示例）
来源：http://hz.dashuyun.cn/gtvjunsvcn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shzxlz.cn/gtvphmoyrd.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shzxlz.cn/gthfwnbpex.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.c1oappe.top/gtahysyzaf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hammf.cn/gtwupcmtaw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.daria6918.cn/gtnxeqtwxs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.snrcjt.cn/gtlvxkomva.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ybcxt.top/gtdarjufmr.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ydjk.org.cn/gtuyaxfhjl.html

[N04] 斐波那契数列
来源：http://hz.pycfn.com/gtlpmwenon.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shangyingyoupin.top/gtgbttbreu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.smart0.xyz/gthnhumtyy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jianghu66.top/gtbjuoaxqy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.wangshuangyany.cn/gtxrqcoaef.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.svipenyu.cn/gtfvpgfscx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhiwuduotai.top/gtkcuixwhy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cheryme.top/gtuimajyls.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.haohaochexian.top/gtzdqrbejr.html

[N05] 最大公约数
来源：http://hz.ywan-chungtsiang.top/gtihtsdbmd.html

Py:   math.gcd(a, b)
来源：http://hz.hnxiangtu.top/gtkxmullow.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.aibaodan.cn/gtzynmdolk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xziqi.cn/gtedqdxrdq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.kuanghao11.cn/gtflqfgipr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jlsjyb.cn/gtiozejdqc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.andypj.xyz/gttygoponz.html

Ruby: a.gcd(b)
来源：http://hz.chenjidiqi.icu/gtnrepwhmi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.andypj.xyz/gtyqodhutm.html

[N06] 判断回文字符串
来源：http://hz.wangshuangyany.cn/gtxxatqvch.html

Py:   s == s[::-1]
来源：http://hz.pycfn.com/gtjqhihqus.html

PHP:  $s === strrev($s);
来源：http://hz.redwolf501.top/gtylxbevlt.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtjoyndzhf.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtfzuqlher.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yvedp.cn/gtscpsrwxx.html

Go:   // 双指针从两端比较
来源：http://hz.jinyuanbaomall.cn/gtuezyqwri.html

Ruby: s == s.reverse
来源：http://hz.haohaochexian.top/gtblltbcwg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ywan-chungtsiang.top/gtgetxnwwz.html

[N07] 两数之和（返回下标）
来源：http://hz.smart0.xyz/gtfcbhrinw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cqqwz.cn/gtwovvabnm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sysykeji.top/gtivvnbjvb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jianghu66.top/gtxojlutvh.html

TS:   // 手写 Map<string, number>
来源：http://hz.daria6918.cn/gtfbvatvkq.html

Java: // 手写 HashMap
来源：http://hz.guowangkeji.top/gtwisuxmzk.html

Go:   // 手写 map[int]int
来源：http://hz.gzhubu.top/gtanhrweul.html

Ruby: // 手写 Hash
来源：http://hz.aibaodan.cn/gtrgpftsqg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.kuanghao11.cn/gtdlzivvwq.html

[N08] 生成全排列
来源：http://hz.ydjk.org.cn/gtwfzstuda.html

Py:   itertools.permutations(arr)
来源：http://hz.wangshuangyany.cn/gthfvfljve.html

PHP:  // 手写递归交换
来源：http://hz.gogol.net.cn/gtjbvmwrym.html

JS:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtrkelrzuh.html

TS:   // 手写回溯递归
来源：http://hz.guowangkeji.top/gtdcjehghc.html

Java: // 手写回溯递归
来源：http://hz.ppjwa.cn/gtpsxyweyx.html

Go:   // 手写回溯递归
来源：http://hz.kuanghao11.cn/gtdtkmnwzg.html

Ruby: arr.permutation.to_a
来源：http://hz.zhongyouzk.top/gtujjziecb.html

C#:   // 手写回溯递归
来源：http://hz.pycfn.com/gthjibktqg.html

[N09] 栈与队列
来源：http://hz.hywenlv.cn/gtnrxrukcp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ehwqpu.com/gtupvhnicg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinyuanbaomall.cn/gtheczdapp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zdqjudy.top/gtnnerqxno.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jiagoushi.top/gtguqjmkmf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ivvv.top/gtnxfwiavr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhengqikj.top/gtcccrudim.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yj20258888.top/gtlskgfqff.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yangfankeji.com/gtmmeneshs.html

[N10] 链表节点定义
来源：http://hz.bjfxy.top/gtxozvuuyp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yangfankeji.com/gtnwsvpvqp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shzxlz.cn/gtygilgmcu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.snrcjt.cn/gtybjvilch.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhongyouzk.top/gtysepleix.html

Java: class Node { int v; Node next; }
来源：http://hz.zhaomingkeji.xyz/gtlfgjslfx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yvedp.cn/gtueavpfyt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.vqdsnc.cn/gtnhuwthqh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.haohaochexian.top/gtwckltvib.html

[N11] 二叉树中序遍历
来源：http://hz.gaohongyu789.top/gtjxhvejfc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hfpthk.cn/gtfgywtddr.html

PHP:  // 手写递归函数
来源：http://hz.chenlongwang.top/gtvuarqyvu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.redwolf501.top/gtjkgdpqfi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xuetiantiany.cn/gtnnqcwssw.html

Java: // 手写递归
来源：http://hz.ydzc1.top/gtlraondwk.html

Go:   // 手写递归
来源：http://hz.nanxinkj.top/gtbjnkdrjb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.aizwys.cn/gtkqqvkywi.html

C#:   // 手写递归
来源：http://hz.sufxvd.cn/gtrbflrhiw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.guowangkeji.top/gtibewzxll.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.mhx1999.top/gtfdxpujgs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ivvv.top/gtrrrcrgqv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sysykeji.top/gtxbzfkdnq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hammf.cn/gthwwkqyav.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinghuilouyu.cn/gtazzzqiqk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shanyushiyangkeji.top/gtusdcdwjb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hnqzz.top/gtcbdqtizf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenjidiqi.icu/gtzwdicbdm.html

================================================================================
来源：http://hz.nanxinkj.top/gtasqxxvsg.html

O. 并发与异步
来源：http://hz.smart0.xyz/gtzdtlzgne.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtwbzpgzds.html

[O01] 启动一个线程
来源：http://hz.xuanzx.com/gtzzgjanxv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cucudq.cn/gtzclqxmvz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zycfv.cn/gtebwsxtwl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.0kj1m.cn/gtuviadigx.html

TS:   // 同 JS
来源：http://hz.xinyue.icu/gtrrhamxqg.html

Java: new Thread(() -> f()).start()
来源：http://hz.jianghu66.top/gtzdynraok.html

Go:   go f()
来源：http://hz.ehwqpu.com/gtvytatsxs.html

Ruby: Thread.new { f }
来源：http://hz.zhijiandao.cn/gtkejuzyty.html

C#:   Task.Run(() => F());
来源：http://hz.c1oappe.top/gtndkqwzli.html

[O02] 使用线程池
来源：http://hz.cashguo.top/gtpfwbjkbe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yangfankeji.com/gtpfjerjap.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jqgfzy.top/gtajwpofml.html

JS:   // worker_threads 线程池
来源：http://hz.yuanzhike.top/gtfrkuhvds.html

TS:   // worker_threads 线程池
来源：http://hz.0kj1m.cn/gttzkmsypw.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yuxming.cn/gtimhqbhug.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shanyushiyangtech.top/gtckkjawrp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cucudq.cn/gtjnzkmeyw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hnqzz.top/gthleshbgn.html

[O03] 加锁保护共享数据
来源：http://hz.zhijiandao.cn/gthojylinh.html

Py:   with lock: shared += 1
来源：http://hz.yj20258.top/gtimshygfu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ehwqpu.com/gtcufqftqy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.daxiang520.top/gticgdzbxy.html

TS:   // 同 JS
来源：http://hz.xylfe.cn/gtwtbikfck.html

Java: synchronized (this) { shared++; }
来源：http://hz.vqdsnc.cn/gtotgnphdc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xinyue.icu/gtomtrmnds.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xinyue.icu/gtxyvdwncw.html

C#:   lock (gate) { shared++; }
来源：http://hz.hnxiangtu.top/gtmjozloiz.html

[O04] 定义异步函数并等待
来源：http://hz.zhixingplan.top/gtorhpyhsv.html

Py:   async def f():⏎    await g()
来源：http://hz.jianghu66.top/gtrgmikgos.html


<!-- 参考信息 -->