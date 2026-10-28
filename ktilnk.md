代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hfpthk.cn/gtrhlghvvt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinqigfzy.top/gtsmnyjwqi.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jianghu66.top/gtolpvegny.html

Py:   pickle.dumps(obj)
来源：http://hz.zhoulong.xyz/gtwhxmuvkh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.52xcode.cn/gtfeficdcf.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.fengsongda.top/gtgcqypfaf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jyoumei.cn/gtdnukirdk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.bjfxy.top/gtagvpfgcy.html

Go:   encoding/gob
来源：http://hz.dashuyun.cn/gtjuqrfdbj.html

Ruby: Marshal.dump(obj)
来源：http://hz.ybcxt.top/gtqrfggfvd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shanyushiyangtech.top/gtbztrpcjq.html

================================================================================
来源：http://hz.pengpengdd.cyou/gthfxdduqp.html

L. 网络请求
来源：http://hz.cdnleiting.top/gtmwhkpkqw.html

================================================================================
来源：http://hz.ydzc1.top/gtsdfjatqp.html

[L01] 发送 GET 请求
来源：http://hz.nanxuanxn.top/gthihibdgd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.andypj.xyz/gtceunnkfc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhengqikj.top/gtuwrcvkmx.html

JS:   await fetch(url)
来源：http://hz.gotoacloud.top/gtsluckwzh.html

TS:   await fetch(url)
来源：http://hz.zhijiandao.cn/gtdbvadsxt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.guowangkeji.top/gtkvoqxmls.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhoulong.xyz/gtnixiozhe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jqgufenzy.top/gtaqejcngc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj20258.top/gtrmfshwbp.html

[L02] 发送 POST JSON
来源：http://hz.jiagoushi.top/gtytfccpzq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.kuanghao11.cn/gtjsftpvuu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ehwqpu.com/gtggnzqnpf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxuanxn.top/gtsrcmifbs.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cdnleiting.top/gtfihnfiek.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.chenlongwang.top/gtjggtzequ.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.wangdashe.top/gtfvfnezun.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cdnleiting.top/gtroqcncgw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.meibo888.top/gtkbjyello.html

[L03] 设置自定义请求头
来源：http://hz.shanyushiyangkeji.top/gtgwxaaxwu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.vqdsnc.cn/gtpshspleu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ivvv.top/gtdsrgmvtk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ppjwa.cn/gtrfjlwjto.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.birdmap.top/gtoozatjcv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinqigfzy.top/gtuhosdzbs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sweek.top/gtqsxvepgl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.pycfn.com/gtndaoaohy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.iojbl.cn/gtyiuudlhr.html

[L04] 设置超时
来源：http://hz.fengsongda.top/gtazdsrnsu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yueranfly.top/gtksfaczyt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.vqdsnc.cn/gtjfwcozjf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.pengpengdd.cyou/gtbreysbqy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.pengpengdd.cyou/gtmnlegndq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhongyouzk.top/gtlbzivbvl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hammf.cn/gtmztftemo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ydzc1.top/gtlwzddkta.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jqgufenzy.top/gtbcvgtojx.html

[L05] 上传文件（multipart）
来源：http://hz.vqdsnc.cn/gtropetsgk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.guannengcc.top/gtiamajgom.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cdnleiting.top/gtbucspgnu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.mhx1999.top/gtimtswwxa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258888.top/gtgprbwklv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.meibo888.top/gtyfreigmj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.dianchejie.cn/gtuhcvxnvt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.dianchejie.cn/gtmrvajyye.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gzhubu.top/gtxevyxmuz.html

[L06] 解析响应为 JSON
来源：http://hz.chenzaomai.com/gtffalwdbr.html

Py:   resp.json()
来源：http://hz.shzxlz.cn/gtjcxayhyx.html

PHP:  json_decode($body, true);
来源：http://hz.aibaodan.cn/gtoqkdeydd.html

JS:   await resp.json()
来源：http://hz.ppjwa.cn/gtsufoyraw.html

TS:   await resp.json()
来源：http://hz.yvedp.cn/gttagmdlrj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhongyouzk.top/gtpvorpmeq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sufxvd.cn/gttaarhftv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hywenlv.cn/gtatbcdrsq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yanxiufei.cn/gtlkceqiii.html

[L07] 处理 HTTP 状态码
来源：http://hz.zdqjudy.top/gtodwrvbag.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cqqwz.cn/gtnietdjdy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinyuanbaomall.cn/gtlyshljwl.html

JS:   resp.ok;  resp.status
来源：http://hz.quarkkingdee.top/gtprmoxenl.html

TS:   resp.ok;  resp.status
来源：http://hz.c1oappe.top/gtkkqrntwu.html

Java: resp.statusCode()
来源：http://hz.smart0.xyz/gttqmimoyq.html

Go:   resp.StatusCode
来源：http://hz.guannengcc.top/gtohxilwta.html

Ruby: resp.code.to_i
来源：http://hz.gogol.net.cn/gtxsxkmpbj.html

C#:   (int)resp.StatusCode
来源：http://hz.jqgufenzy.top/gtwwflfgsi.html

[L08] 并发请求多个地址
来源：http://hz.zhiwuduotai.top/gtonrasiql.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.aibaodan.cn/gtcrkocblg.html

PHP:  curl_multi_init() 系列
来源：http://hz.hfpthk.cn/gtnbwhbxij.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.9152youxi.cn/gtvcnxusme.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhoulong.xyz/gtjrhorxgq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yj202588.top/gtwokdjibn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.aizwys.cn/gtebiqbplx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.fzhhl.top/gtouflsohr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cheryme.top/gtxauvsrmc.html

================================================================================
来源：http://hz.jinqigfzy.top/gtxizbptrf.html

M. 命令行 / 进程 / 环境
来源：http://hz.shanyushiyangkeji.top/gtibeujgyg.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtupwhhcnd.html

[M01] 读取命令行参数
来源：http://hz.kuanghao11.cn/gtfguyvskf.html

Py:   sys.argv[1:]
来源：http://hz.wangdashe.top/gtgkjfvxwc.html

PHP:  $argv;  $argc;
来源：http://hz.tianlin.xyz/gttuolxvxr.html

JS:   process.argv.slice(2)
来源：http://hz.ppjwa.cn/gtaovkkwpb.html

TS:   process.argv.slice(2)
来源：http://hz.zdqjudy.top/gtaqqpyyba.html

Java: args 数组（main 方法参数）
来源：http://hz.haohaochexian.top/gtpjoxmruo.html

Go:   os.Args[1:]
来源：http://hz.hfpthk.cn/gtrwurirux.html

Ruby: ARGV
来源：http://hz.yvedp.cn/gtxpmsoorj.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jlsjyb.cn/gtgdzqqghj.html

[M02] 读取环境变量
来源：http://hz.gaohongyu789.top/gtttghwodb.html

Py:   os.environ.get("HOME")
来源：http://hz.shanyushiyangkeji.top/gtcccqousl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ywan-chungtsiang.top/gtxeaqrrqt.html

JS:   process.env.HOME
来源：http://hz.yangfankeji.com/gtpyqfylud.html

TS:   process.env.HOME
来源：http://hz.jyoumei.cn/gtvmvgnuiq.html

Java: System.getenv("HOME")
来源：http://hz.ydzc1.top/gtmnpkmyzh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jqgufenzy.top/gtwxrnacnr.html

Ruby: ENV["HOME"]
来源：http://hz.cqqwz.cn/gtqnambper.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gogol.net.cn/gtnfptbsvw.html

[M03] 执行外部命令
来源：http://hz.daria6918.cn/gtxdorhxsm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cqqwz.cn/gtfhxbscre.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ppjwa.cn/gtaquqaign.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hysaishi.cn/gteeiszicw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cheryme.top/gtuvdhnidf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ppjwa.cn/gtwtshvfgz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shuidangran.top/gtpuxyiedk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhoulong.xyz/gtclytzyns.html

C#:   Process.Start("ls", "-l");
来源：http://hz.guowangkeji.top/gtxezmicsd.html

[M04] 获取当前工作目录
来源：http://hz.c1oappe.top/gthyctnrug.html

Py:   os.getcwd()
来源：http://hz.cqqwz.cn/gtcyyfmrcb.html

PHP:  getcwd();
来源：http://hz.zhiwuduotai.top/gtseqeeoaw.html

JS:   process.cwd()
来源：http://hz.havefunace.top/gtcikwrbej.html

TS:   process.cwd()
来源：http://hz.svipenyu.cn/gtdzxqeyph.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shanyushiyangtech.top/gtolrceint.html

Go:   os.Getwd()
来源：http://hz.yongpay.top/gthqlqfbcs.html

Ruby: Dir.pwd
来源：http://hz.hnxiangtu.top/gtbjmtctif.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zdqjudy.top/gtppggnxsu.html

[M05] 设置退出码
来源：http://hz.fzhhl.top/gtomwhebny.html

Py:   sys.exit(1)
来源：http://hz.guannengcc.top/gtgonxoasf.html

PHP:  exit(1);
来源：http://hz.tanke756.top/gtijgjomvc.html

JS:   process.exit(1)
来源：http://hz.ydzc1.top/gtuqlunwuz.html

TS:   process.exit(1)
来源：http://hz.vqdsnc.cn/gtuyvxojmw.html

Java: System.exit(1)
来源：http://hz.jianghu66.top/gtlocxnrhg.html

Go:   os.Exit(1)
来源：http://hz.dianchejie.cn/gtddltldlk.html

Ruby: exit 1
来源：http://hz.yueranfly.top/gtuxqwbfqd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinyuanbaomall.cn/gtjuhjtpyf.html

[M06] 向标准错误输出
来源：http://hz.ehwqpu.com/gtgjnmdchr.html

Py:   print("err", file=sys.stderr)
来源：http://hz.snrcjt.cn/gtwbsrybhd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhiwuduotai.top/gtnruvgefs.html

JS:   console.error("err")
来源：http://hz.zhiwuduotai.top/gtcakztrjf.html

TS:   console.error("err")
来源：http://hz.jinqigfzy.top/gtmlfhsnhv.html

Java: System.err.println("err")
来源：http://hz.jinqigufen.top/gtzuahjcaq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.fzhhl.top/gtbrpzulke.html

Ruby: warn "err"
来源：http://hz.yuanzhike.top/gtymfucldb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yongpay.top/gteruzodnv.html

[M07] 判断是否为主入口
来源：http://hz.xylfe.cn/gtkeabvxmc.html

Py:   if __name__ == "__main__":
来源：http://hz.shangyingyoupin.top/gtoiggzypl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhiwuduotai.top/gtnizjmshp.html

JS:   require.main === module
来源：http://hz.cqqwz.cn/gtjzcptmot.html

TS:   require.main === module
来源：http://hz.cucudq.cn/gtkmygwcvq.html

Java: public static void main(String[] args)
来源：http://hz.jinqigfzy.top/gteoqdhxyk.html

Go:   func main()
来源：http://hz.9152youxi.cn/gtmwiwedwz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.nanxuanxn.top/gtvpyhtvch.html

C#:   static void Main(string[] args)
来源：http://hz.shuidangran.top/gthjnocpal.html

[M08] 获取系统与运行时信息
来源：http://hz.sufxvd.cn/gtdzxkxiam.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jianghu66.top/gtrifueoyj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jqgufenzy.top/gtmngljxgc.html

JS:   process.platform;  process.version
来源：http://hz.yj20258888.top/gthicixpfe.html

TS:   process.platform;  process.version
来源：http://hz.redwolf501.top/gtojfqlpez.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinqigufen.top/gtgckqpswo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.daxiang520.top/gtppdrrfei.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yuxming.cn/gtoflfsddd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.0kj1m.cn/gtnwdzoaqc.html

================================================================================
来源：http://hz.gaohongyu789.top/gtyorlibtg.html

N. 数据结构与算法
来源：http://hz.hywenlv.cn/gtmjtyjjfi.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtzknttmrk.html

[N01] 二分查找（有序数组）
来源：http://hz.xingfuxueyuan.xyz/gtyehcmbgc.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj202588.top/gtlfodylgf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.chenjidiqi.icu/gtxoofrqqf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuanzx.com/gtlykjnktk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.quarkkingdee.top/gtdcjvqeyj.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xylfe.cn/gtsfpqfnup.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.c1oappe.top/gtpwqhpeew.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sweek.top/gtpmfsithw.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gzhubu.top/gtbojdqcfo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ybcxt.top/gthdsetmrr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jqgfzy.top/gtrfounnkc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.kuanghao11.cn/gtshwwnmqt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenlongwang.top/gtswwqjajf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenlongwang.top/gtdcsunmyy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yongpay.top/gtrmcnnvsk.html

Go:   slices.Sort(arr)
来源：http://hz.ywan-chungtsiang.top/gtxahqpunf.html

Ruby: arr.sort
来源：http://hz.zhiwuduotai.top/gtjuxfplnl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yj20258888.top/gtrmerjkew.html

[N03] 快速排序（分治示例）
来源：http://hz.cucudq.cn/gtmqfxgoef.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.tian-w.cn/gtpojcshdy.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shuidangran.top/gtfwtjphok.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pengpengdd.cyou/gtcmoysily.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tanke756.top/gtyvdgvkiv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.chenjidiqi.icu/gticrykrwl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhaomingkeji.xyz/gtbolodctr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xinyue.icu/gtcyprfspa.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ybcxt.top/gtrjdscagr.html

[N04] 斐波那契数列
来源：http://hz.chenzaomai.com/gtoduuqugx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.snrcjt.cn/gtianfqeti.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yonumen.top/gtpxfujbyx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.c1oappe.top/gtcftxyosc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pengpengdd.cyou/gtrszbplcq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jqgufenzy.top/gtbpczlnbi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.c1oappe.top/gthnvldldy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigufen.top/gtyfdjueuv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jiagoushi.top/gthoauxake.html

[N05] 最大公约数
来源：http://hz.zycfv.cn/gtzxtctuxe.html

Py:   math.gcd(a, b)
来源：http://hz.ywan-chungtsiang.top/gtdfcgckvy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhiwuduotai.top/gtgdjcmvjw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.havefunace.top/gtasawskht.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.quarkkingdee.top/gtoxqbidsb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.snrcjt.cn/gttzdlxsjn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinyuanbaomall.cn/gtxzagobow.html

Ruby: a.gcd(b)
来源：http://hz.316326.xyz/gtvrkszwml.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.c1oappe.top/gtzifvlsgp.html

[N06] 判断回文字符串
来源：http://hz.shanyushiyangtech.top/gtixwdddre.html

Py:   s == s[::-1]
来源：http://hz.pengpengdd.cyou/gthvgzmazc.html

PHP:  $s === strrev($s);
来源：http://hz.hywenlv.cn/gtyvvdpphm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zycfv.cn/gtkxyfzypm.html

TS:   s === [...s].reverse().join("")
来源：http://hz.c1oappe.top/gttthoaunv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jyoumei.cn/gtiuavfawn.html

Go:   // 双指针从两端比较
来源：http://hz.jqgfzy.top/gtuotxwvyp.html

Ruby: s == s.reverse
来源：http://hz.hywenlv.cn/gtxcrtdngx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.iojbl.cn/gtjgmdgckk.html

[N07] 两数之和（返回下标）
来源：http://hz.hnxiangtu.top/gtpomjpfaa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.daria6918.cn/gtnscyteem.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.snrcjt.cn/gtatpqyzmn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xingfuxueyuan.xyz/gtubeylcfg.html

TS:   // 手写 Map<string, number>
来源：http://hz.jqgufenzy.top/gtytgdppvx.html

Java: // 手写 HashMap
来源：http://hz.xingfuxueyuan.xyz/gtqztbicdo.html

Go:   // 手写 map[int]int
来源：http://hz.tanke756.top/gtytxgbali.html

Ruby: // 手写 Hash
来源：http://hz.xingfuxueyuan.xyz/gtvxbzqclz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.tian-w.cn/gtdwjblzww.html

[N08] 生成全排列
来源：http://hz.jyoumei.cn/gtbgajehca.html

Py:   itertools.permutations(arr)
来源：http://hz.hongshengwenyu.top/gthfllunlt.html

PHP:  // 手写递归交换
来源：http://hz.c1oappe.top/gttmfayjnr.html

JS:   // 手写回溯递归
来源：http://hz.52xcode.cn/gtinxeomed.html

TS:   // 手写回溯递归
来源：http://hz.ivvv.top/gtucnukfkq.html

Java: // 手写回溯递归
来源：http://hz.ydzc1.top/gtehgzbggp.html

Go:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtyytegcwn.html

Ruby: arr.permutation.to_a
来源：http://hz.c1oappe.top/gtivoboych.html

C#:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtzmbrxtqz.html

[N09] 栈与队列
来源：http://hz.ehwqpu.com/gtqzklxtna.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ybcxt.top/gtfbsumdxw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ehwqpu.com/gtukmcwfiu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.feifeiyinyue.top/gthbmfrbro.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.gotoacloud.top/gtbsbfxsgg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.bjfxy.top/gtfhvddoqs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ybcxt.top/gtgmtzvivc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yuxming.cn/gtfdutexpa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cdnleiting.top/gtdvisvggg.html

[N10] 链表节点定义
来源：http://hz.snrcjt.cn/gtcpujgbqk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.pengpengdd.cyou/gtgwqbsbgq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sweek.top/gtoyiypsyt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hfpthk.cn/gtkadmrzvy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yvedp.cn/gtgodqpzkw.html

Java: class Node { int v; Node next; }
来源：http://hz.yonumen.top/gtksdrkfzu.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ivvv.top/gtmrxoijkt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shangyingyoupin.top/gtppnjinrj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zdqjudy.top/gtpeuldicj.html

[N11] 二叉树中序遍历
来源：http://hz.snrcjt.cn/gtzoobjvok.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sufxvd.cn/gtmvuqjizl.html

PHP:  // 手写递归函数
来源：http://hz.hywenlv.cn/gtrammivwy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydzc1.top/gtwjmylevk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenlongwang.top/gtyhkejgus.html

Java: // 手写递归
来源：http://hz.yueranfly.top/gtjkksqvww.html

Go:   // 手写递归
来源：http://hz.feifeiyinyue.top/gtmiwfophd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.snrcjt.cn/gtdfzjunnz.html

C#:   // 手写递归
来源：http://hz.zhengqikj.top/gtyzspfllk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.havefunace.top/gtxhjvqoog.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jiagoushi.top/gtttilpxmq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jiagoushi.top/gtlnbynuai.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cdnleiting.top/gtqazjijul.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.c1oappe.top/gtpjxhwerz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ybcxt.top/gtkzkbumth.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.fzhhl.top/gtfyiigoaq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sxryk.cn/gtgvfmdogo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgfzy.top/gtfcmezidv.html

================================================================================
来源：http://hz.cheryme.top/gtvexhcprl.html

O. 并发与异步
来源：http://hz.fengsongda.top/gtovgfgbwg.html

================================================================================
来源：http://hz.sufxvd.cn/gtmedmssom.html

[O01] 启动一个线程
来源：http://hz.ydzc1.top/gtgafalojf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.dashuyun.cn/gtygtdjsyj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.kuanghao11.cn/gtmxarsbze.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hongshengwenyu.top/gthvodwbgx.html

TS:   // 同 JS
来源：http://hz.guowangkeji.top/gtbtwsawwg.html

Java: new Thread(() -> f()).start()
来源：http://hz.yuxming.cn/gtujyipivg.html

Go:   go f()
来源：http://hz.meibo888.top/gtvjwwyhuh.html

Ruby: Thread.new { f }
来源：http://hz.ivvv.top/gthytalkwc.html

C#:   Task.Run(() => F());
来源：http://hz.gzhubu.top/gthckdxcoh.html

[O02] 使用线程池
来源：http://hz.yongpay.top/gtyonzslwc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.gogol.net.cn/gtjrigrlem.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.tian-w.cn/gtkpbjycfq.html

JS:   // worker_threads 线程池
来源：http://hz.xylfe.cn/gtnafwfjur.html

TS:   // worker_threads 线程池
来源：http://hz.316326.xyz/gtudxuxsqj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ehwqpu.com/gtnbgcyjja.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gaohongyu789.top/gtfmtqcmks.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yangfankeji.com/gtufgtuxag.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hywenlv.cn/gtxyrgoldi.html

[O03] 加锁保护共享数据
来源：http://hz.jqgufenzy.top/gtrzaorboo.html

Py:   with lock: shared += 1
来源：http://hz.xylfe.cn/gtgtwyieda.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jiagoushi.top/gtcoiteidc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.sweek.top/gtkbgzqhse.html

TS:   // 同 JS
来源：http://hz.yanxiufei.cn/gtggjxbkjz.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhaomingkeji.xyz/gtxosejuxh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.vqdsnc.cn/gtgldehyhy.html


<!-- 参考信息 -->