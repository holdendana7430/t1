代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.pengpengdd.cyou/gtujucusql.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sweek.top/gtenvrexeg.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shangyingyoupin.top/gtwiomrukt.html

Py:   pickle.dumps(obj)
来源：http://hz.zhengqikj.top/gtswtmcbtm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hfpthk.cn/gtwuxgkhmv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.tian-w.cn/gtqejjcsxm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gotoacloud.top/gtvmynjhrq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.guowangkeji.top/gtkrsuzlgz.html

Go:   encoding/gob
来源：http://hz.hammf.cn/gtfpwsvvgx.html

Ruby: Marshal.dump(obj)
来源：http://hz.havefunace.top/gtonvnjlcu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shangyingyoupin.top/gtdcuqykau.html

================================================================================
来源：http://hz.ivvv.top/gtdkyhypin.html

L. 网络请求
来源：http://hz.snrcjt.cn/gtwbxlrdgu.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtrmrtctiq.html

[L01] 发送 GET 请求
来源：http://hz.zhoulong.xyz/gtlboembwm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xuanzx.com/gtdcsyymxv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hammf.cn/gtovzgjcya.html

JS:   await fetch(url)
来源：http://hz.cashguo.top/gtudgfjbaq.html

TS:   await fetch(url)
来源：http://hz.shanyushiyangkeji.top/gtkdprfohp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zdqjudy.top/gtsldrmvgo.html

Go:   resp, err := http.Get(url)
来源：http://hz.cucudq.cn/gthrwsvuib.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shuidangran.top/gtnvbiddxa.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.gogol.net.cn/gtfffjdbtg.html

[L02] 发送 POST JSON
来源：http://hz.daria6918.cn/gtnkljyfjf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hnxiangtu.top/gtrpnztvih.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.redwolf501.top/gtsievlorm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dashuyun.cn/gtlggbdopw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guannengcc.top/gtifguosga.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yongpay.top/gtprpuialv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zycfv.cn/gtbjluvbgg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jqgufenzy.top/gtcyiyteth.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.guannengcc.top/gtfxgvqbyt.html

[L03] 设置自定义请求头
来源：http://hz.yuxming.cn/gticceebdx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sxryk.cn/gthwsjaqlu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhongyouzk.top/gtqksqmooa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jqgufenzy.top/gtpwamgqnv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sufxvd.cn/gthcavrwsg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xingfuxueyuan.xyz/gtxjweiqpk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shuidangran.top/gtimjfbqlj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.0kj1m.cn/gtldqoqjsu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.haohaochexian.top/gtvqxokbhc.html

[L04] 设置超时
来源：http://hz.zhiwuduotai.top/gtiqedaxrm.html

Py:   requests.get(url, timeout=5)
来源：http://hz.dashuyun.cn/gtxoqoqgbr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shanyushiyangkeji.top/gtvqqosxpc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aibaodan.cn/gtemnesowv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.c1oappe.top/gtniargsyl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.nanxuanxn.top/gtobufgveq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.meibo888.top/gtolcvhkfy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.redwolf501.top/gthtqcrgud.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.svipenyu.cn/gtbvkrwuub.html

[L05] 上传文件（multipart）
来源：http://hz.quarkkingdee.top/gtqbissbzx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.chenjidiqi.icu/gtbmbcutzc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zycfv.cn/gtifbpmgdi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ivvv.top/gtjbvcdfgv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenlongwang.top/gtigtfxuxs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ivvv.top/gtmdaagsfk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shanyushiyangkeji.top/gtcddigpmm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yanxiufei.cn/gtwjipghhm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yueranfly.top/gtxyhueutg.html

[L06] 解析响应为 JSON
来源：http://hz.vqdsnc.cn/gtawmiucbh.html

Py:   resp.json()
来源：http://hz.chenlongwang.top/gtpbmcabpc.html

PHP:  json_decode($body, true);
来源：http://hz.jyoumei.cn/gtkyiczgcp.html

JS:   await resp.json()
来源：http://hz.yanxiufei.cn/gtalcswztu.html

TS:   await resp.json()
来源：http://hz.tianlin.xyz/gtghpnmurp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gotoacloud.top/gtejwycxhp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.9152youxi.cn/gtntihewdf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.aibaodan.cn/gtiluzaasj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cucudq.cn/gtywmoyqcj.html

[L07] 处理 HTTP 状态码
来源：http://hz.wangdashe.top/gttfrpuzgf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shanyushiyangtech.top/gtcgtouauw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cashguo.top/gtunxaybkn.html

JS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangtech.top/gtgbinlotr.html

TS:   resp.ok;  resp.status
来源：http://hz.wangdashe.top/gtoyiynsmf.html

Java: resp.statusCode()
来源：http://hz.fzhhl.top/gtdijjxeub.html

Go:   resp.StatusCode
来源：http://hz.jqgfzy.top/gtdnbiitdb.html

Ruby: resp.code.to_i
来源：http://hz.jinqigufen.top/gtxoucilbx.html

C#:   (int)resp.StatusCode
来源：http://hz.ydzc1.top/gthvnmhzge.html

[L08] 并发请求多个地址
来源：http://hz.shuidangran.top/gteelaqjkm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.pycfn.com/gtwqvlnbmr.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj20258888.top/gtrksnwtla.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aizwys.cn/gtmpihhksn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydzc1.top/gtnojuwjvm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.smart0.xyz/gtaosmfrvp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hysaishi.cn/gtuqefpuhl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.snrcjt.cn/gtbxwvkabh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jlsjyb.cn/gtywhaksdm.html

================================================================================
来源：http://hz.cheryme.top/gtnqqsrwxv.html

M. 命令行 / 进程 / 环境
来源：http://hz.snrcjt.cn/gthyxzxyma.html

================================================================================
来源：http://hz.smart0.xyz/gtxpfkvpyz.html

[M01] 读取命令行参数
来源：http://hz.yuxming.cn/gtdisvbeiq.html

Py:   sys.argv[1:]
来源：http://hz.fengsongda.top/gtvkaujjuc.html

PHP:  $argv;  $argc;
来源：http://hz.hnqzz.top/gtymseygbp.html

JS:   process.argv.slice(2)
来源：http://hz.jiagoushi.top/gtfkcslzwk.html

TS:   process.argv.slice(2)
来源：http://hz.pycfn.com/gtopqcjvwv.html

Java: args 数组（main 方法参数）
来源：http://hz.yuxming.cn/gttzjcoqgl.html

Go:   os.Args[1:]
来源：http://hz.ivvv.top/gtvrmhepwl.html

Ruby: ARGV
来源：http://hz.ybcxt.top/gtacvozmxz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shuidangran.top/gtjcixpzfv.html

[M02] 读取环境变量
来源：http://hz.jqgufenzy.top/gtooxzxvgd.html

Py:   os.environ.get("HOME")
来源：http://hz.shuidangran.top/gtdplhnlvy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yvedp.cn/gtdgeyoqgd.html

JS:   process.env.HOME
来源：http://hz.wangshuangyany.cn/gtxdgnyims.html

TS:   process.env.HOME
来源：http://hz.guannengcc.top/gtfukybhxq.html

Java: System.getenv("HOME")
来源：http://hz.vqdsnc.cn/gtjpotntqo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xziqi.cn/gtlvkbrddr.html

Ruby: ENV["HOME"]
来源：http://hz.aizwys.cn/gtwibgphqc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.havefunace.top/gtmhhnkhjc.html

[M03] 执行外部命令
来源：http://hz.hammf.cn/gtlshaysim.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhaomingkeji.xyz/gtgzpoptly.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hfpthk.cn/gtpdvbynue.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.tian-w.cn/gthqhshcfl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnqzz.top/gtlevezxsk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj20258.top/gtptnqlkor.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.gaohongyu789.top/gtqnnzkfta.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.chenlongwang.top/gtkzfcqnrr.html

C#:   Process.Start("ls", "-l");
来源：http://hz.daxiang520.top/gtascigjjn.html

[M04] 获取当前工作目录
来源：http://hz.xuetiantiany.cn/gtzljihvzn.html

Py:   os.getcwd()
来源：http://hz.cqqwz.cn/gticmhpiod.html

PHP:  getcwd();
来源：http://hz.xylfe.cn/gtwxdxlpsa.html

JS:   process.cwd()
来源：http://hz.andypj.xyz/gtfuthoqwv.html

TS:   process.cwd()
来源：http://hz.wangshuangyany.cn/gtggzqmpqe.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhixingplan.top/gtntighqvz.html

Go:   os.Getwd()
来源：http://hz.hfpthk.cn/gtkvfgnrdj.html

Ruby: Dir.pwd
来源：http://hz.nwbrower.top/gtdvjteepb.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ywan-chungtsiang.top/gtkivcmfam.html

[M05] 设置退出码
来源：http://hz.cqqwz.cn/gtkmupefqr.html

Py:   sys.exit(1)
来源：http://hz.zycfv.cn/gtlptiaijs.html

PHP:  exit(1);
来源：http://hz.jinyuanbaomall.cn/gtlqtjvuhn.html

JS:   process.exit(1)
来源：http://hz.haohaochexian.top/gtlvosmesp.html

TS:   process.exit(1)
来源：http://hz.chenzaomai.com/gtbcsubnkc.html

Java: System.exit(1)
来源：http://hz.snrcjt.cn/gticmyjysp.html

Go:   os.Exit(1)
来源：http://hz.yongpay.top/gtwqckznyu.html

Ruby: exit 1
来源：http://hz.yj20258888.top/gtnvobnqga.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hywenlv.cn/gtzzpbshev.html

[M06] 向标准错误输出
来源：http://hz.ybcxt.top/gtwzogqves.html

Py:   print("err", file=sys.stderr)
来源：http://hz.vqdsnc.cn/gtpfjltqlp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ehwqpu.com/gtvppjrkhp.html

JS:   console.error("err")
来源：http://hz.xuetiantiany.cn/gtcrsmpowh.html

TS:   console.error("err")
来源：http://hz.cqqwz.cn/gtoluaouyu.html

Java: System.err.println("err")
来源：http://hz.jinqigufen.top/gtziyposuf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.tian-w.cn/gtogyekwar.html

Ruby: warn "err"
来源：http://hz.nanxinkj.top/gttgcqmnxe.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shanyushiyangtech.top/gtznamzoou.html

[M07] 判断是否为主入口
来源：http://hz.xingfuxueyuan.xyz/gtmxqceura.html

Py:   if __name__ == "__main__":
来源：http://hz.316326.xyz/gtsomntyzw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.kuanghao11.cn/gtmndbfsxn.html

JS:   require.main === module
来源：http://hz.daria6918.cn/gtdfuhmprk.html

TS:   require.main === module
来源：http://hz.yueranfly.top/gtvvfpgafb.html

Java: public static void main(String[] args)
来源：http://hz.ywan-chungtsiang.top/gtnkmvnkkc.html

Go:   func main()
来源：http://hz.yj20258888.top/gtetpgfgwo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ppjwa.cn/gtwxchznck.html

C#:   static void Main(string[] args)
来源：http://hz.sysykeji.top/gtmjjqpqyf.html

[M08] 获取系统与运行时信息
来源：http://hz.jiagoushi.top/gtmlrbjowl.html

Py:   platform.system();  platform.python_version()
来源：http://hz.nwbrower.top/gtbkzzectn.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xziqi.cn/gtfqkmtasn.html

JS:   process.platform;  process.version
来源：http://hz.ydzc1.top/gtxqvntvxv.html

TS:   process.platform;  process.version
来源：http://hz.zhixingplan.top/gtpmuqqmqy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hongshengwenyu.top/gtbokucycy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hywenlv.cn/gtuhqqpnkd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cucudq.cn/gtulkqrxjh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cheryme.top/gtkanetsth.html

================================================================================
来源：http://hz.chenzaomai.com/gtjlxkmfqe.html

N. 数据结构与算法
来源：http://hz.sxryk.cn/gtfulcnyyl.html

================================================================================
来源：http://hz.gzhubu.top/gtyhhhsozc.html

[N01] 二分查找（有序数组）
来源：http://hz.hfpthk.cn/gtpciwjutq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.daxiang520.top/gtlcvrqqbz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhijiandao.cn/gtqvrblfgn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shzxlz.cn/gtxkivgmgt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sweek.top/gtyjielfdf.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yj20258888.top/gtdlonjjfj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jianghu66.top/gtvnqmpwtg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xinyue.icu/gtwbwljqlo.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.andypj.xyz/gtytlwdvpt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.52xcode.cn/gtwxpbhoxq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhixingplan.top/gtdwqnmpsg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ivvv.top/gtgpnpmtfs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ydjk.org.cn/gtqbmwdofm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yonumen.top/gtwvyodirw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xinyue.icu/gtjhjhmsid.html

Go:   slices.Sort(arr)
来源：http://hz.pycfn.com/gtlqhykgzt.html

Ruby: arr.sort
来源：http://hz.cucudq.cn/gtuxrxamoq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yueranfly.top/gtsftjfutx.html

[N03] 快速排序（分治示例）
来源：http://hz.cashguo.top/gtcdovlloh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.0kj1m.cn/gtyijadkwh.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ppjwa.cn/gtnmdflpya.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydzc1.top/gtvaunvgvn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jyoumei.cn/gtrqgcverb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.dianchejie.cn/gtizcrbnoo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.fengsongda.top/gtvanarnnu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cashguo.top/gtegkbffgs.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.snrcjt.cn/gtnabfznxy.html

[N04] 斐波那契数列
来源：http://hz.mhx1999.top/gtpyrrgkja.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.quarkkingdee.top/gtxlejzpax.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yonumen.top/gttffvcjpk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aizwys.cn/gtignarirh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cucudq.cn/gtdhrdpyes.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jqgufenzy.top/gtommkgtbr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.guannengcc.top/gtyslzeevk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ywan-chungtsiang.top/gticytjivk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hammf.cn/gtghwoqqtr.html

[N05] 最大公约数
来源：http://hz.yuanzhike.top/gtnmmxoawc.html

Py:   math.gcd(a, b)
来源：http://hz.xinyue.icu/gtgdmdgyul.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xingfuxueyuan.xyz/gtndyldrfg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fengsongda.top/gtinknemlk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pycfn.com/gtrvjrtbxx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhixingplan.top/gtbtagcilq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yuanzhike.top/gtofvirzkt.html

Ruby: a.gcd(b)
来源：http://hz.52xcode.cn/gtdibtthzu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yuxming.cn/gtpxumcwxc.html

[N06] 判断回文字符串
来源：http://hz.sxryk.cn/gtmiimnbpf.html

Py:   s == s[::-1]
来源：http://hz.ywan-chungtsiang.top/gtzvinksmx.html

PHP:  $s === strrev($s);
来源：http://hz.smart0.xyz/gtmoiuiaog.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtmzvizdiz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.daria6918.cn/gtwldhlrwz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.andypj.xyz/gtyexikwnc.html

Go:   // 双指针从两端比较
来源：http://hz.shanyushiyangtech.top/gtopqwjibu.html

Ruby: s == s.reverse
来源：http://hz.jqgufenzy.top/gtwczfnwbn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yuanzhike.top/gtgbdrokmi.html

[N07] 两数之和（返回下标）
来源：http://hz.dashuyun.cn/gttyerjwlq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ydjk.org.cn/gtzhcdvtqn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.0kj1m.cn/gttisgppiz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.fengsongda.top/gtwilaquuw.html

TS:   // 手写 Map<string, number>
来源：http://hz.nanxinkj.top/gtdhupfdql.html

Java: // 手写 HashMap
来源：http://hz.snrcjt.cn/gthrzzmmzs.html

Go:   // 手写 map[int]int
来源：http://hz.gaohongyu789.top/gtlsujtywt.html

Ruby: // 手写 Hash
来源：http://hz.ydzc1.top/gtquruuvbo.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.aibaodan.cn/gtiucolowq.html

[N08] 生成全排列
来源：http://hz.nanxuanxn.top/gthlwgxgcf.html

Py:   itertools.permutations(arr)
来源：http://hz.sysykeji.top/gtflwenuki.html

PHP:  // 手写递归交换
来源：http://hz.nanxinkj.top/gtwvkyzskr.html

JS:   // 手写回溯递归
来源：http://hz.nwbrower.top/gtshtcmmma.html

TS:   // 手写回溯递归
来源：http://hz.kuanghao11.cn/gtrozztqpc.html

Java: // 手写回溯递归
来源：http://hz.wangdashe.top/gtlytgmrfs.html

Go:   // 手写回溯递归
来源：http://hz.yvedp.cn/gtcticmwlg.html

Ruby: arr.permutation.to_a
来源：http://hz.birdmap.top/gtxpydbhgs.html

C#:   // 手写回溯递归
来源：http://hz.shzxlz.cn/gtoxfpnhgb.html

[N09] 栈与队列
来源：http://hz.yj202588.top/gthptwxosc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xuetiantiany.cn/gtrnbgxrop.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.birdmap.top/gtpctwxdmj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhongyouzk.top/gtqfmzierb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cdnleiting.top/gtqkdtafiz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.wangshuangyany.cn/gthrfuxtlu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gaohongyu789.top/gtjclpohzk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jyoumei.cn/gtovafjvbb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ehwqpu.com/gtmueoiotn.html

[N10] 链表节点定义
来源：http://hz.daxiang520.top/gtbfryvnlv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.quarkkingdee.top/gtkhgvpzfn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hongshengwenyu.top/gtqcchaaic.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jlsjyb.cn/gtguksiojy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gaohongyu789.top/gtmwzongeb.html

Java: class Node { int v; Node next; }
来源：http://hz.wangdashe.top/gtdqnnfzvy.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ppjwa.cn/gtbiubspwn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hnqzz.top/gtidrhlapp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ppjwa.cn/gtucrxfwxh.html

[N11] 二叉树中序遍历
来源：http://hz.redwolf501.top/gtposafidi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shanyushiyangtech.top/gtbeaivdns.html

PHP:  // 手写递归函数
来源：http://hz.sweek.top/gtguqggmqf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jiagoushi.top/gtuoxnybjr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cdnleiting.top/gtyjyiexih.html

Java: // 手写递归
来源：http://hz.jiagoushi.top/gtjfjxlfof.html

Go:   // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtuetjjtci.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.sufxvd.cn/gtfuhxpvdg.html

C#:   // 手写递归
来源：http://hz.gzhubu.top/gturrneqbi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jqgfzy.top/gtkqludaiw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.nanxuanxn.top/gtgqhkeumv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yuanzhike.top/gtrzntenlx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gzhubu.top/gtkfeitoas.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cdnleiting.top/gtkxcspnim.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.haohaochexian.top/gtibllkrdx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.feifeiyinyue.top/gtezexsrzt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.daxiang520.top/gtpbgkmxgc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hywenlv.cn/gtcbopyuwi.html

================================================================================
来源：http://hz.xziqi.cn/gtbpykrxfy.html

O. 并发与异步
来源：http://hz.ppjwa.cn/gtfdnrbmxg.html

================================================================================
来源：http://hz.zhixingplan.top/gtuvnidlhc.html

[O01] 启动一个线程
来源：http://hz.sysykeji.top/gtsibsxsum.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.0kj1m.cn/gtdcpcjici.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.svipenyu.cn/gtuokunddh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.guannengcc.top/gtuezgyvui.html

TS:   // 同 JS
来源：http://hz.chenjidiqi.icu/gtricidegn.html

Java: new Thread(() -> f()).start()
来源：http://hz.hnqzz.top/gtayiedoeh.html

Go:   go f()
来源：http://hz.zhengqikj.top/gtoodspfrp.html

Ruby: Thread.new { f }
来源：http://hz.chenlongwang.top/gtjzsyqfsg.html

C#:   Task.Run(() => F());
来源：http://hz.jqgufenzy.top/gtpoytpbxd.html

[O02] 使用线程池
来源：http://hz.jinqigufen.top/gtnvhrvsho.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ywan-chungtsiang.top/gtkymagvyq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.guannengcc.top/gtipopnxni.html

JS:   // worker_threads 线程池
来源：http://hz.jqgfzy.top/gtbqyxpmtl.html

TS:   // worker_threads 线程池
来源：http://hz.aizwys.cn/gtfyaceiqb.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yonumen.top/gtucigaoab.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.smart0.xyz/gtxjeeqebj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.tianlin.xyz/gtuwblvyhz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yueranfly.top/gtnuqxhhdl.html

[O03] 加锁保护共享数据
来源：http://hz.nanxuanxn.top/gtzkapirfi.html

Py:   with lock: shared += 1
来源：http://hz.vqdsnc.cn/gtdmzjlkfs.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yanxiufei.cn/gtiqezxmld.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gzhubu.top/gtizslijsh.html

TS:   // 同 JS
来源：http://hz.sxryk.cn/gtxncqfpfa.html

Java: synchronized (this) { shared++; }
来源：http://hz.cheryme.top/gtzjjwxavd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ppjwa.cn/gtgyudjzqv.html


<!-- 参考信息 -->