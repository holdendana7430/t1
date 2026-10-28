代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.redwolf501.top/gtifozwduh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jqgufenzy.top/gtlkahlras.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jyoumei.cn/gtsoufajtc.html

Py:   pickle.dumps(obj)
来源：http://hz.zdqjudy.top/gtxhqpvuus.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tian-w.cn/gtxdjgdquh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ywan-chungtsiang.top/gtkhwcbprp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shzxlz.cn/gtarddjfwl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xylfe.cn/gtyqnqrezx.html

Go:   encoding/gob
来源：http://hz.zhijiandao.cn/gtgxgiyaca.html

Ruby: Marshal.dump(obj)
来源：http://hz.andypj.xyz/gttppaawna.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gogol.net.cn/gtizdowofb.html

================================================================================
来源：http://hz.jlsjyb.cn/gtthlfjzay.html

L. 网络请求
来源：http://hz.sufxvd.cn/gtgdfjubqb.html

================================================================================
来源：http://hz.yangfankeji.com/gtquaygpkf.html

[L01] 发送 GET 请求
来源：http://hz.chenjidiqi.icu/gtshlguzuy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinghuilouyu.cn/gtxdqlnugy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhiwuduotai.top/gtzbvvqkbt.html

JS:   await fetch(url)
来源：http://hz.yonumen.top/gtjltfacpv.html

TS:   await fetch(url)
来源：http://hz.yj202588.top/gtpgnxlicu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jqgfzy.top/gtpahmplpw.html

Go:   resp, err := http.Get(url)
来源：http://hz.ppjwa.cn/gtamcbsxdz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhixingplan.top/gtcdbwvzmr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.andypj.xyz/gtiyvobjsp.html

[L02] 发送 POST JSON
来源：http://hz.gzhubu.top/gtvqqnwjhj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hfpthk.cn/gtsnzcsufs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.aibaodan.cn/gtseixytmt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.c1oappe.top/gttcwipjub.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.smart0.xyz/gtblccoihd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cheryme.top/gtnvlmvyyy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xuetiantiany.cn/gtqrygecjn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cashguo.top/gtsmyhyanl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cheryme.top/gtxgpspkfv.html

[L03] 设置自定义请求头
来源：http://hz.shanyushiyangkeji.top/gthvzuokbx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gzhubu.top/gtvalabsup.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jiagoushi.top/gtxjedvrnn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ydzc1.top/gtzjkuswln.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ywan-chungtsiang.top/gtvzxxikuz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.mhx1999.top/gtjwdkcrpb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sweek.top/gtyqmypqaq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.nanxuanxn.top/gtsyanfbst.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.0kj1m.cn/gtjmdwtrmd.html

[L04] 设置超时
来源：http://hz.tianlin.xyz/gtirbqmpqe.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xuanzx.com/gticcutddt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.wangshuangyany.cn/gtyvsdzdqw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shuidangran.top/gtctuolpvf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxinkj.top/gtoihwxduj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hnxiangtu.top/gtwbifysds.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cqqwz.cn/gtpjodshma.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.chenjidiqi.icu/gtpuihgglb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhiwuduotai.top/gtixtafyaz.html

[L05] 上传文件（multipart）
来源：http://hz.xinyue.icu/gtudxyxqmg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ppjwa.cn/gtkkudlwzm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xuetiantiany.cn/gtwfsbhcfy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.guannengcc.top/gtgiqmlmxe.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sweek.top/gtjustdqjp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zycfv.cn/gtdpkcmanb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.smart0.xyz/gtjwivtndr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yj20258.top/gttptpmwcp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhengqikj.top/gtifaxngoi.html

[L06] 解析响应为 JSON
来源：http://hz.aibaodan.cn/gtjvtxtwoi.html

Py:   resp.json()
来源：http://hz.yueranfly.top/gtmnsloyhz.html

PHP:  json_decode($body, true);
来源：http://hz.daria6918.cn/gtzywjkpkb.html

JS:   await resp.json()
来源：http://hz.fengsongda.top/gtqxrdhszb.html

TS:   await resp.json()
来源：http://hz.dashuyun.cn/gtfrjbwvss.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhengqikj.top/gtdrdjfohv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jlsjyb.cn/gthrdcjdle.html

Ruby: JSON.parse(resp.body)
来源：http://hz.52xcode.cn/gtyywkcppk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.redwolf501.top/gtndzcjzyq.html

[L07] 处理 HTTP 状态码
来源：http://hz.shangyingyoupin.top/gtpexwpmmp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jqgufenzy.top/gtpyxpkwsr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.tian-w.cn/gtmczgcdsn.html

JS:   resp.ok;  resp.status
来源：http://hz.nanxuanxn.top/gtaistcbti.html

TS:   resp.ok;  resp.status
来源：http://hz.sufxvd.cn/gtzdrcrkyl.html

Java: resp.statusCode()
来源：http://hz.jyoumei.cn/gtamvfebzr.html

Go:   resp.StatusCode
来源：http://hz.tianlin.xyz/gtnuazcupb.html

Ruby: resp.code.to_i
来源：http://hz.9152youxi.cn/gtoucjrjri.html

C#:   (int)resp.StatusCode
来源：http://hz.hongshengwenyu.top/gtworruuhy.html

[L08] 并发请求多个地址
来源：http://hz.tian-w.cn/gtgkcpzbor.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cdnleiting.top/gtukkksnxp.html

PHP:  curl_multi_init() 系列
来源：http://hz.haohaochexian.top/gtmitdgost.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shangyingyoupin.top/gtjxswvetf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dianchejie.cn/gtvdvsmoxz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hammf.cn/gtzbfvpesz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zdqjudy.top/gtbsqyrhdx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xziqi.cn/gtchuptmff.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.haohaochexian.top/gtwjxilmzt.html

================================================================================
来源：http://hz.daria6918.cn/gtikaevgey.html

M. 命令行 / 进程 / 环境
来源：http://hz.gzhubu.top/gtqnkmdvcn.html

================================================================================
来源：http://hz.dianchejie.cn/gtyacxxbec.html

[M01] 读取命令行参数
来源：http://hz.zdqjudy.top/gtfzcbixvs.html

Py:   sys.argv[1:]
来源：http://hz.jlsjyb.cn/gtdzkrzdvy.html

PHP:  $argv;  $argc;
来源：http://hz.zhengqikj.top/gtpwsykque.html

JS:   process.argv.slice(2)
来源：http://hz.hammf.cn/gtvdmcgvrr.html

TS:   process.argv.slice(2)
来源：http://hz.yuanzhike.top/gtjacvvrog.html

Java: args 数组（main 方法参数）
来源：http://hz.xziqi.cn/gttxbzqaxz.html

Go:   os.Args[1:]
来源：http://hz.zhoulong.xyz/gtiobqqqbg.html

Ruby: ARGV
来源：http://hz.tian-w.cn/gtphuujmtb.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ppjwa.cn/gtgjkrllhl.html

[M02] 读取环境变量
来源：http://hz.ydjk.org.cn/gtdmpidkdy.html

Py:   os.environ.get("HOME")
来源：http://hz.jlsjyb.cn/gtbhlnisos.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shangyingyoupin.top/gtxajcmrdh.html

JS:   process.env.HOME
来源：http://hz.ivvv.top/gtmeurmchl.html

TS:   process.env.HOME
来源：http://hz.jinqigufen.top/gtdktoejuo.html

Java: System.getenv("HOME")
来源：http://hz.quarkkingdee.top/gtypwtzfnt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yuxming.cn/gtkhcwzchq.html

Ruby: ENV["HOME"]
来源：http://hz.dashuyun.cn/gteloclmfo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhongyouzk.top/gtfhpejgnw.html

[M03] 执行外部命令
来源：http://hz.hysaishi.cn/gtofhnnkxv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shanyushiyangtech.top/gtzfxgrorc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.tianlin.xyz/gtuyjlcfpa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.daxiang520.top/gtxnixyxmn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj20258888.top/gtqofhddoa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.chenjidiqi.icu/gtdjejqcsp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jianghu66.top/gtptcwqgxu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.9152youxi.cn/gtdyghweip.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cheryme.top/gttapgbptx.html

[M04] 获取当前工作目录
来源：http://hz.sxryk.cn/gtavgymkxo.html

Py:   os.getcwd()
来源：http://hz.sxryk.cn/gtfkorawfl.html

PHP:  getcwd();
来源：http://hz.chenlongwang.top/gtkbrltymj.html

JS:   process.cwd()
来源：http://hz.iojbl.cn/gtqgxxwexh.html

TS:   process.cwd()
来源：http://hz.quarkkingdee.top/gtyynyviei.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ybcxt.top/gttyydbrch.html

Go:   os.Getwd()
来源：http://hz.zhixingplan.top/gtagaflltp.html

Ruby: Dir.pwd
来源：http://hz.guowangkeji.top/gtsweuksxk.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.kuanghao11.cn/gthfubmxsy.html

[M05] 设置退出码
来源：http://hz.jinqigfzy.top/gtoczifqjc.html

Py:   sys.exit(1)
来源：http://hz.zdqjudy.top/gtpwpktlhe.html

PHP:  exit(1);
来源：http://hz.sxryk.cn/gtmucbzite.html

JS:   process.exit(1)
来源：http://hz.jqgufenzy.top/gtbgvebcys.html

TS:   process.exit(1)
来源：http://hz.sysykeji.top/gtlkldmgix.html

Java: System.exit(1)
来源：http://hz.wangdashe.top/gterksahhe.html

Go:   os.Exit(1)
来源：http://hz.zhengqikj.top/gtfyqawegd.html

Ruby: exit 1
来源：http://hz.yuxming.cn/gttbsceher.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ydzc1.top/gtltmpjmqr.html

[M06] 向标准错误输出
来源：http://hz.xingfuxueyuan.xyz/gtaifppiwz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yj202588.top/gtcjukydde.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.316326.xyz/gtgfqjzmwl.html

JS:   console.error("err")
来源：http://hz.hnxiangtu.top/gtsdejaazn.html

TS:   console.error("err")
来源：http://hz.xziqi.cn/gtwarmgpgr.html

Java: System.err.println("err")
来源：http://hz.sxryk.cn/gtzttpirdx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.52xcode.cn/gturpydcll.html

Ruby: warn "err"
来源：http://hz.sxryk.cn/gtqofowasy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shzxlz.cn/gtcaylurei.html

[M07] 判断是否为主入口
来源：http://hz.aizwys.cn/gtxvtviukd.html

Py:   if __name__ == "__main__":
来源：http://hz.xziqi.cn/gttpklsgin.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.redwolf501.top/gtcxrmknee.html

JS:   require.main === module
来源：http://hz.zhengqikj.top/gtndnqmcls.html

TS:   require.main === module
来源：http://hz.yvedp.cn/gtuzjnxves.html

Java: public static void main(String[] args)
来源：http://hz.quarkkingdee.top/gtqfzgffdb.html

Go:   func main()
来源：http://hz.jqgufenzy.top/gtrypnjnag.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cashguo.top/gtcohhjniw.html

C#:   static void Main(string[] args)
来源：http://hz.havefunace.top/gtxaaeuhoz.html

[M08] 获取系统与运行时信息
来源：http://hz.zdqjudy.top/gtelsdynby.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zdqjudy.top/gtmizycnka.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.dashuyun.cn/gtunfmyntw.html

JS:   process.platform;  process.version
来源：http://hz.sweek.top/gtxwirocpj.html

TS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtlkabrhqq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.chenzaomai.com/gtsawgnkcx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hongshengwenyu.top/gtkpgnufjk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xingfuxueyuan.xyz/gtqucbigcv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yuxming.cn/gtcrjxkncq.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtekjvtego.html

N. 数据结构与算法
来源：http://hz.tian-w.cn/gtmycmipfu.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtkgeiekvw.html

[N01] 二分查找（有序数组）
来源：http://hz.9152youxi.cn/gtmajxgjig.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.tianlin.xyz/gttfiewcye.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.9152youxi.cn/gttrengxfo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hammf.cn/gtiqvgglyp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnqzz.top/gtdsbrhavm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.9152youxi.cn/gtdczgwqym.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.9152youxi.cn/gtkvmqrsmy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xuetiantiany.cn/gtvwbsqtfl.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.dianchejie.cn/gtvktwlkdw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.snrcjt.cn/gtjcxeigeg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigufen.top/gtvspkxpyo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shanyushiyangtech.top/gttlvgsywj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jlsjyb.cn/gtuhtcropm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.feifeiyinyue.top/gtezvcdppc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.meibo888.top/gtckomgcws.html

Go:   slices.Sort(arr)
来源：http://hz.tian-w.cn/gthftnbwrf.html

Ruby: arr.sort
来源：http://hz.gotoacloud.top/gtddakkvpy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ydzc1.top/gtclgfrxbd.html

[N03] 快速排序（分治示例）
来源：http://hz.cheryme.top/gtfyrmzglf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xziqi.cn/gtynunmklb.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinqigfzy.top/gtdexkuzbk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shzxlz.cn/gttsxdbqbq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aizwys.cn/gthxzsetoq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cdnleiting.top/gthhcdesrf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yongpay.top/gtzhwztamb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sxryk.cn/gtljmpojni.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhongyouzk.top/gtbanlhqsm.html

[N04] 斐波那契数列
来源：http://hz.xylfe.cn/gttmmarlfl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hongshengwenyu.top/gtgggcinhw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jiagoushi.top/gtntrcyyan.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigfzy.top/gthoxjvltn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gtndleuipf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.9152youxi.cn/gtbbbxwexy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.smart0.xyz/gtxnvjrrmp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cashguo.top/gttykclhzy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.52xcode.cn/gtbzfwmnyq.html

[N05] 最大公约数
来源：http://hz.hammf.cn/gtwxyjkgxv.html

Py:   math.gcd(a, b)
来源：http://hz.chenzaomai.com/gtkjfwdybt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.feifeiyinyue.top/gtgyhxdeaz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guannengcc.top/gtgwxopeed.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gtrdsrqwor.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenlongwang.top/gteqgoknas.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhijiandao.cn/gtolvjapdk.html

Ruby: a.gcd(b)
来源：http://hz.jianghu66.top/gtanrmndrc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.haohaochexian.top/gtwfiuoday.html

[N06] 判断回文字符串
来源：http://hz.redwolf501.top/gtknjcwhkr.html

Py:   s == s[::-1]
来源：http://hz.zycfv.cn/gtpfanyfbu.html

PHP:  $s === strrev($s);
来源：http://hz.xuetiantiany.cn/gtcooyidyx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cashguo.top/gtpjlbcqld.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gtkdjqsgqw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xuetiantiany.cn/gtqyicvgnb.html

Go:   // 双指针从两端比较
来源：http://hz.aizwys.cn/gtrsdnidek.html

Ruby: s == s.reverse
来源：http://hz.sxryk.cn/gtkqtcgjxk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tianlin.xyz/gtbrahzcmk.html

[N07] 两数之和（返回下标）
来源：http://hz.xuetiantiany.cn/gttzzklvoz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yangfankeji.com/gtxiikgfbk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hnqzz.top/gtxfohoxpq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.tanke756.top/gtffxylemp.html

TS:   // 手写 Map<string, number>
来源：http://hz.xingfuxueyuan.xyz/gtykhhxakk.html

Java: // 手写 HashMap
来源：http://hz.jlsjyb.cn/gtvbqzxwba.html

Go:   // 手写 map[int]int
来源：http://hz.316326.xyz/gtrectbmrt.html

Ruby: // 手写 Hash
来源：http://hz.sweek.top/gtfffbfuji.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hysaishi.cn/gthrlazbjj.html

[N08] 生成全排列
来源：http://hz.guowangkeji.top/gttfzwlcnj.html

Py:   itertools.permutations(arr)
来源：http://hz.sufxvd.cn/gtwqafyjox.html

PHP:  // 手写递归交换
来源：http://hz.zhiwuduotai.top/gtqgkdwmsx.html

JS:   // 手写回溯递归
来源：http://hz.yj202588.top/gtygyofjbo.html

TS:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtypclaajp.html

Java: // 手写回溯递归
来源：http://hz.smart0.xyz/gthdxvpyrc.html

Go:   // 手写回溯递归
来源：http://hz.wangdashe.top/gtyebcxcbu.html

Ruby: arr.permutation.to_a
来源：http://hz.gotoacloud.top/gtswlyqwnm.html

C#:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtfnnfccgc.html

[N09] 栈与队列
来源：http://hz.jinqigfzy.top/gtanvigvxi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.0kj1m.cn/gtofiyjzxd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ydjk.org.cn/gtelgxqfzn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.gaohongyu789.top/gtfhwxfiyd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hywenlv.cn/gtjhxcwrtp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sysykeji.top/gtjinadeji.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.wangshuangyany.cn/gtfjukkocu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.316326.xyz/gtzexgixfi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cashguo.top/gtxoyvjmna.html

[N10] 链表节点定义
来源：http://hz.sysykeji.top/gttjhobspo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.sysykeji.top/gtasznckvt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.dianchejie.cn/gtccngnyta.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ydjk.org.cn/gtohtrbmxa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yonumen.top/gtqoafdmkl.html

Java: class Node { int v; Node next; }
来源：http://hz.cdnleiting.top/gtumvmwmlk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jiagoushi.top/gtrmqwxibn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.chenjidiqi.icu/gtvmkwvgar.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yonumen.top/gthxclcfro.html

[N11] 二叉树中序遍历
来源：http://hz.xinyue.icu/gtutxkarbx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ydjk.org.cn/gtqrvpjddo.html

PHP:  // 手写递归函数
来源：http://hz.ybcxt.top/gtcefcimjk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.9152youxi.cn/gtmwtgomdi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shanyushiyangtech.top/gtjpapuniw.html

Java: // 手写递归
来源：http://hz.svipenyu.cn/gtmllgugwr.html

Go:   // 手写递归
来源：http://hz.havefunace.top/gtsvsjmlqe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.0kj1m.cn/gtshqygdpu.html

C#:   // 手写递归
来源：http://hz.xziqi.cn/gtecwxhahj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shanyushiyangkeji.top/gtczjertpn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cdnleiting.top/gtprlgnoku.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shanyushiyangkeji.top/gtxisdvfpt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.daxiang520.top/gttbfdlwfs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangkeji.top/gtiazuefct.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yangfankeji.com/gtcvvcydya.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xuanzx.com/gttggprccl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ppjwa.cn/gtavhnyrjn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.kuanghao11.cn/gtsxkgqqif.html

================================================================================
来源：http://hz.cucudq.cn/gtdorvbzof.html

O. 并发与异步
来源：http://hz.hywenlv.cn/gtgtlcyphr.html

================================================================================
来源：http://hz.gzhubu.top/gtwqnemzce.html

[O01] 启动一个线程
来源：http://hz.316326.xyz/gtdnehcigq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yuxming.cn/gtghhgotnp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xuanzx.com/gtptdtlseu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.tian-w.cn/gtcysqlyfy.html

TS:   // 同 JS
来源：http://hz.zdqjudy.top/gtfxgzzhru.html

Java: new Thread(() -> f()).start()
来源：http://hz.hammf.cn/gtdemslmfz.html

Go:   go f()
来源：http://hz.jyoumei.cn/gteubesvmx.html

Ruby: Thread.new { f }
来源：http://hz.zycfv.cn/gtqdnmyjte.html

C#:   Task.Run(() => F());
来源：http://hz.bjfxy.top/gthujxhcks.html

[O02] 使用线程池
来源：http://hz.fengsongda.top/gtfysazzqo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jiagoushi.top/gttzmtyqov.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.bjfxy.top/gtmozidajm.html

JS:   // worker_threads 线程池
来源：http://hz.yongpay.top/gtzybjvefh.html

TS:   // worker_threads 线程池
来源：http://hz.cheryme.top/gtwagfczvg.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yvedp.cn/gtlfcvejfr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hywenlv.cn/gtfiuzxxiu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xingfuxueyuan.xyz/gtsvuoqzeo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.dashuyun.cn/gtdsidgepn.html

[O03] 加锁保护共享数据
来源：http://hz.sxryk.cn/gtmmtneonn.html

Py:   with lock: shared += 1
来源：http://hz.gzhubu.top/gtmjxoyulc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cqqwz.cn/gtwmrfdnux.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jqgufenzy.top/gtxbalixib.html

TS:   // 同 JS
来源：http://hz.yonumen.top/gtnqtdgfas.html

Java: synchronized (this) { shared++; }
来源：http://hz.cqqwz.cn/gtehkgfvcl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cucudq.cn/gtbhiflrmb.html


<!-- 参考信息 -->