代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtzecdrtwp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.tanke756.top/gtvkrewidc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shangyingyoupin.top/gtkkgqxeci.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cashguo.top/gtmixcxpql.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yonumen.top/gtikhvergi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hysaishi.cn/gtaahzixjf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.meibo888.top/gtzqsfmmzq.html

Py:   pickle.dumps(obj)
来源：http://hz.chenjidiqi.icu/gttcepusej.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.0kj1m.cn/gtmslhibsy.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sxryk.cn/gtpyxwcfez.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.sxryk.cn/gtjzzjsouk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.daria6918.cn/gtpeusbrtu.html

Go:   encoding/gob
来源：http://hz.hfpthk.cn/gtamivieam.html

Ruby: Marshal.dump(obj)
来源：http://hz.jiagoushi.top/gtvatucwph.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.bjfxy.top/gtohaltjse.html

================================================================================
来源：http://hz.andypj.xyz/gthtmdgzjz.html

L. 网络请求
来源：http://hz.ehwqpu.com/gttlcskyak.html

================================================================================
来源：http://hz.wangshuangyany.cn/gthsyggber.html

[L01] 发送 GET 请求
来源：http://hz.yuanzhike.top/gtiwheeruf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.redwolf501.top/gtvvytgxsh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zdqjudy.top/gtrqlrigwr.html

JS:   await fetch(url)
来源：http://hz.zycfv.cn/gtisewuqzw.html

TS:   await fetch(url)
来源：http://hz.shzxlz.cn/gtathxebaw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sxryk.cn/gtsgsyhjnx.html

Go:   resp, err := http.Get(url)
来源：http://hz.jianghu66.top/gtzbjgecmr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shanyushiyangtech.top/gtjovcrchv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.birdmap.top/gtedfvvntr.html

[L02] 发送 POST JSON
来源：http://hz.wangshuangyany.cn/gtbovrqdis.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zdqjudy.top/gtjtrhmplp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sufxvd.cn/gtgzpwedrs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xingfuxueyuan.xyz/gtlmsvpisq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangkeji.top/gtlrmggwtu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gzhubu.top/gtikwcpxbu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xuetiantiany.cn/gtveclzdcf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xylfe.cn/gtcsaycyib.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cucudq.cn/gtfdfkuicr.html

[L03] 设置自定义请求头
来源：http://hz.jianghu66.top/gtbhrhhpzi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sysykeji.top/gtnwaazagi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hfpthk.cn/gtohkfztdj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.kuanghao11.cn/gtzdvggxzq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhijiandao.cn/gtqaazrvja.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yvedp.cn/gtlxlxyjbd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.dianchejie.cn/gtpoebxusb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yuanzhike.top/gtuqnmjseq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shuidangran.top/gtvdaebeej.html

[L04] 设置超时
来源：http://hz.zhijiandao.cn/gtyvoqcpzp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jqgufenzy.top/gtqfgeokbr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cucudq.cn/gtaebbdykl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuanzx.com/gtewfhepbo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhoulong.xyz/gtvgovzqir.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hnqzz.top/gtrpwuohuw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zycfv.cn/gtagoqoeyb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yj202588.top/gtqesoeczd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jqgufenzy.top/gtiouqkgle.html

[L05] 上传文件（multipart）
来源：http://hz.0kj1m.cn/gtpdmgkrth.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shangyingyoupin.top/gtelqqlgor.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hnqzz.top/gtczhrlcuq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.birdmap.top/gtkxjvmjpn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cqqwz.cn/gtbnjxgnrf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.havefunace.top/gtgqrdpjqe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinqigfzy.top/gthtemenia.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.haohaochexian.top/gtgtoancmn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yongpay.top/gteugefgog.html

[L06] 解析响应为 JSON
来源：http://hz.cdnleiting.top/gtclkwohyg.html

Py:   resp.json()
来源：http://hz.cdnleiting.top/gtvsmffvqj.html

PHP:  json_decode($body, true);
来源：http://hz.ppjwa.cn/gtkdpynonf.html

JS:   await resp.json()
来源：http://hz.ydjk.org.cn/gtjgpsrqis.html

TS:   await resp.json()
来源：http://hz.pycfn.com/gtgcojdqcz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.vqdsnc.cn/gtasnzayry.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.haohaochexian.top/gtqlxujbci.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jiagoushi.top/gtwkygrmrf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhiwuduotai.top/gtjftaerjn.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhijiandao.cn/gtcigrmdtc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.birdmap.top/gtexgewnzu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hnxiangtu.top/gtwvkktbro.html

JS:   resp.ok;  resp.status
来源：http://hz.yj20258.top/gtmcjuyrws.html

TS:   resp.ok;  resp.status
来源：http://hz.wangdashe.top/gtboexwnvo.html

Java: resp.statusCode()
来源：http://hz.mhx1999.top/gtllpzkjoc.html

Go:   resp.StatusCode
来源：http://hz.cqqwz.cn/gtvvrqcadr.html

Ruby: resp.code.to_i
来源：http://hz.vqdsnc.cn/gtbttvlswk.html

C#:   (int)resp.StatusCode
来源：http://hz.tian-w.cn/gtwdrxaaql.html

[L08] 并发请求多个地址
来源：http://hz.zdqjudy.top/gtdwzsmljs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yuanzhike.top/gtcbgiplxd.html

PHP:  curl_multi_init() 系列
来源：http://hz.shanyushiyangkeji.top/gtlywzspii.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgfzy.top/gtsgeevewi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pengpengdd.cyou/gtxjatnxhp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zdqjudy.top/gtriwtznjm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gogol.net.cn/gtzecwegkf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jlsjyb.cn/gtsmdoimif.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.fzhhl.top/gtihnucpbq.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtnzthjnzr.html

M. 命令行 / 进程 / 环境
来源：http://hz.52xcode.cn/gtpgofhzrx.html

================================================================================
来源：http://hz.gogol.net.cn/gtrepwtocb.html

[M01] 读取命令行参数
来源：http://hz.sysykeji.top/gtncbeukuv.html

Py:   sys.argv[1:]
来源：http://hz.hywenlv.cn/gtidqpupuv.html

PHP:  $argv;  $argc;
来源：http://hz.yangfankeji.com/gtowivnhjt.html

JS:   process.argv.slice(2)
来源：http://hz.hongshengwenyu.top/gtycxmwrnv.html

TS:   process.argv.slice(2)
来源：http://hz.yanxiufei.cn/gtkzkewyws.html

Java: args 数组（main 方法参数）
来源：http://hz.xingfuxueyuan.xyz/gttesyturr.html

Go:   os.Args[1:]
来源：http://hz.hongshengwenyu.top/gtgsoalehs.html

Ruby: ARGV
来源：http://hz.nanxinkj.top/gtifkqachx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.pengpengdd.cyou/gtjzavsaqi.html

[M02] 读取环境变量
来源：http://hz.hywenlv.cn/gtuqwvymyo.html

Py:   os.environ.get("HOME")
来源：http://hz.jyoumei.cn/gtaduuawfk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.fzhhl.top/gtmmxbbdtg.html

JS:   process.env.HOME
来源：http://hz.xuetiantiany.cn/gtnsftnbyr.html

TS:   process.env.HOME
来源：http://hz.ppjwa.cn/gtrocriorh.html

Java: System.getenv("HOME")
来源：http://hz.jyoumei.cn/gthhwwndaq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.pengpengdd.cyou/gtiznnpluf.html

Ruby: ENV["HOME"]
来源：http://hz.ehwqpu.com/gthukgqhzl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.haohaochexian.top/gtxcsifbxm.html

[M03] 执行外部命令
来源：http://hz.yvedp.cn/gtttjxmgqx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yangfankeji.com/gtydngoxlp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yangfankeji.com/gtlzxlgpga.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuetiantiany.cn/gtjhpewjpz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangshuangyany.cn/gtohuclhib.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.redwolf501.top/gtkotviwdy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.nanxuanxn.top/gtjjoeffgy.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.vqdsnc.cn/gtbeopygqb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cucudq.cn/gtvpfnjuih.html

[M04] 获取当前工作目录
来源：http://hz.jqgfzy.top/gtmvqmufbs.html

Py:   os.getcwd()
来源：http://hz.xziqi.cn/gtgfbjdlsy.html

PHP:  getcwd();
来源：http://hz.zhixingplan.top/gtqblbikym.html

JS:   process.cwd()
来源：http://hz.yj20258888.top/gteisprlsk.html

TS:   process.cwd()
来源：http://hz.ppjwa.cn/gtfqrdlzwg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhixingplan.top/gtsihyzkhw.html

Go:   os.Getwd()
来源：http://hz.guannengcc.top/gtoahrtwzo.html

Ruby: Dir.pwd
来源：http://hz.ehwqpu.com/gtehtnsavh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ywan-chungtsiang.top/gtbyfzffne.html

[M05] 设置退出码
来源：http://hz.hammf.cn/gtmiksdvit.html

Py:   sys.exit(1)
来源：http://hz.feifeiyinyue.top/gtguflhrax.html

PHP:  exit(1);
来源：http://hz.snrcjt.cn/gtrmczkgme.html

JS:   process.exit(1)
来源：http://hz.hfpthk.cn/gtmpjtcejn.html

TS:   process.exit(1)
来源：http://hz.zhengqikj.top/gtnpkohbwo.html

Java: System.exit(1)
来源：http://hz.hammf.cn/gtzzgipzyb.html

Go:   os.Exit(1)
来源：http://hz.zhixingplan.top/gtwzroxmdk.html

Ruby: exit 1
来源：http://hz.cdnleiting.top/gtfcaexgna.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ydzc1.top/gtqfqzsywa.html

[M06] 向标准错误输出
来源：http://hz.xylfe.cn/gtuhmullak.html

Py:   print("err", file=sys.stderr)
来源：http://hz.feifeiyinyue.top/gtoedfvkec.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.aizwys.cn/gtglgdvemz.html

JS:   console.error("err")
来源：http://hz.mhx1999.top/gtopmapcwb.html

TS:   console.error("err")
来源：http://hz.chenzaomai.com/gtxqgaitbl.html

Java: System.err.println("err")
来源：http://hz.kuanghao11.cn/gtmbhbnyax.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jqgufenzy.top/gtzrverpuq.html

Ruby: warn "err"
来源：http://hz.andypj.xyz/gtobnwqwfv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xingfuxueyuan.xyz/gtnxlvmnzs.html

[M07] 判断是否为主入口
来源：http://hz.jqgufenzy.top/gthhimlezm.html

Py:   if __name__ == "__main__":
来源：http://hz.kuanghao11.cn/gtkwxtbkwn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.haohaochexian.top/gtjihmbbtx.html

JS:   require.main === module
来源：http://hz.hfpthk.cn/gtbtitpmry.html

TS:   require.main === module
来源：http://hz.daxiang520.top/gtbepjvpkq.html

Java: public static void main(String[] args)
来源：http://hz.xylfe.cn/gtyamcstyt.html

Go:   func main()
来源：http://hz.andypj.xyz/gtppcykphl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shangyingyoupin.top/gtbdupghjx.html

C#:   static void Main(string[] args)
来源：http://hz.jyoumei.cn/gtvqgvtoht.html

[M08] 获取系统与运行时信息
来源：http://hz.hywenlv.cn/gtnjpcwvrj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.sxryk.cn/gtkngngcqh.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hnxiangtu.top/gterlwwdfo.html

JS:   process.platform;  process.version
来源：http://hz.guannengcc.top/gtuabviqbu.html

TS:   process.platform;  process.version
来源：http://hz.smart0.xyz/gtfizrcaav.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ppjwa.cn/gtrdsacmoc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhongyouzk.top/gtgzfncckq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hnxiangtu.top/gtlcjzmqqn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.vqdsnc.cn/gtwldazige.html

================================================================================
来源：http://hz.aibaodan.cn/gtiybntkqd.html

N. 数据结构与算法
来源：http://hz.sufxvd.cn/gtamqhdpxe.html

================================================================================
来源：http://hz.hfpthk.cn/gtpltxesdw.html

[N01] 二分查找（有序数组）
来源：http://hz.svipenyu.cn/gtxervoycp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yuxming.cn/gteuprtvwt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gotoacloud.top/gteitlxkxt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daxiang520.top/gtyldguulu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tanke756.top/gtjwhjxumd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.tian-w.cn/gtipxsrmkx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.guannengcc.top/gtkixkiyos.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.redwolf501.top/gtlhdhdvsr.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.chenlongwang.top/gteacbwemg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xinyue.icu/gtqdungehw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gaohongyu789.top/gtcunvjqhd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shanyushiyangkeji.top/gtuobxxcbg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fzhhl.top/gtflmxlrtc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuanzhike.top/gtiftqhglk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jyoumei.cn/gtwcurdivi.html

Go:   slices.Sort(arr)
来源：http://hz.chenzaomai.com/gtvqqypoxn.html

Ruby: arr.sort
来源：http://hz.yongpay.top/gthhlskboq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.tian-w.cn/gtowjppvco.html

[N03] 快速排序（分治示例）
来源：http://hz.mhx1999.top/gtcktggpyc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gogol.net.cn/gtkxtziviw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jlsjyb.cn/gtmcxmemkx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ywan-chungtsiang.top/gtcnyxhkvx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zycfv.cn/gtjyjarlxz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jlsjyb.cn/gtvaaripep.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.wangshuangyany.cn/gtgftmoobx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shanyushiyangtech.top/gtvkmfikwy.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.c1oappe.top/gtdbmcbuio.html

[N04] 斐波那契数列
来源：http://hz.hywenlv.cn/gtelrzshqo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.guannengcc.top/gtmuatxtis.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.chenjidiqi.icu/gtdcbiabrg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258888.top/gthnsccdts.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxinkj.top/gthlanxfyw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.316326.xyz/gtfbzdqgwb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.iojbl.cn/gtujojhgux.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hnxiangtu.top/gtbrxfarbe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.dashuyun.cn/gtfdvvgifn.html

[N05] 最大公约数
来源：http://hz.andypj.xyz/gtnhltcllj.html

Py:   math.gcd(a, b)
来源：http://hz.fengsongda.top/gtxneerwwd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jiagoushi.top/gtvxawpyvn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.smart0.xyz/gtkvujqpdi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.meibo888.top/gtnyisurdp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenzaomai.com/gtsexficem.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenlongwang.top/gtonmpzvuo.html

Ruby: a.gcd(b)
来源：http://hz.feifeiyinyue.top/gtrjjllusp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yanxiufei.cn/gtgfeoatad.html

[N06] 判断回文字符串
来源：http://hz.yongpay.top/gtunjhivre.html

Py:   s == s[::-1]
来源：http://hz.gotoacloud.top/gtdpjprumb.html

PHP:  $s === strrev($s);
来源：http://hz.chenjidiqi.icu/gtosdlmusf.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtdsrccijr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yanxiufei.cn/gtmaxklwnr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yj202588.top/gtepbdzabk.html

Go:   // 双指针从两端比较
来源：http://hz.c1oappe.top/gtfspnlczx.html

Ruby: s == s.reverse
来源：http://hz.bjfxy.top/gtrxamblim.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.sufxvd.cn/gtzijytjjb.html

[N07] 两数之和（返回下标）
来源：http://hz.redwolf501.top/gtqjvrkmhs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.redwolf501.top/gtoiesthbm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hnxiangtu.top/gtqbednmbk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.tanke756.top/gtziknjqti.html

TS:   // 手写 Map<string, number>
来源：http://hz.shuidangran.top/gtlddmxhyj.html

Java: // 手写 HashMap
来源：http://hz.sufxvd.cn/gtymjisnjc.html

Go:   // 手写 map[int]int
来源：http://hz.cucudq.cn/gtuyrspzhd.html

Ruby: // 手写 Hash
来源：http://hz.hnxiangtu.top/gtegqlbcoy.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.fzhhl.top/gtzwvtxrtq.html

[N08] 生成全排列
来源：http://hz.smart0.xyz/gtsqreculd.html

Py:   itertools.permutations(arr)
来源：http://hz.hnxiangtu.top/gtyogjcuep.html

PHP:  // 手写递归交换
来源：http://hz.havefunace.top/gtyddtrflw.html

JS:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtiwqnmubc.html

TS:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtkthayyoh.html

Java: // 手写回溯递归
来源：http://hz.fzhhl.top/gtejphektr.html

Go:   // 手写回溯递归
来源：http://hz.52xcode.cn/gtmruxuusa.html

Ruby: arr.permutation.to_a
来源：http://hz.daxiang520.top/gthupoanzb.html

C#:   // 手写回溯递归
来源：http://hz.yuxming.cn/gtrdsnlsuw.html

[N09] 栈与队列
来源：http://hz.dashuyun.cn/gtvbjrwvau.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sysykeji.top/gtratdyngl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.birdmap.top/gtxlikrzfy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.shanyushiyangtech.top/gthuuhornr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.nanxuanxn.top/gtfkbqtdcs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hywenlv.cn/gtohpehwyf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.andypj.xyz/gtooasrxam.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jlsjyb.cn/gtwbqjgtxr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xingfuxueyuan.xyz/gttuphvzky.html

[N10] 链表节点定义
来源：http://hz.wangdashe.top/gtfcttvwyb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yj20258.top/gtcsbdpgzp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ppjwa.cn/gtiffzgods.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sufxvd.cn/gtrmixtyov.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hnqzz.top/gtsfhmtzre.html

Java: class Node { int v; Node next; }
来源：http://hz.zhiwuduotai.top/gtogqstzoo.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yj20258.top/gtkkimryzt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.dianchejie.cn/gtegznzdbd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.haohaochexian.top/gtikwrunbs.html

[N11] 二叉树中序遍历
来源：http://hz.shzxlz.cn/gtxlsjtayz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.chenzaomai.com/gtkaocqjso.html

PHP:  // 手写递归函数
来源：http://hz.meibo888.top/gtkqqmlljb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.havefunace.top/gtyxcprkhd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinghuilouyu.cn/gtmixoqwdx.html

Java: // 手写递归
来源：http://hz.ydzc1.top/gtzqeobemr.html

Go:   // 手写递归
来源：http://hz.jlsjyb.cn/gtvvtynkwx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.dianchejie.cn/gtsxbbvsny.html

C#:   // 手写递归
来源：http://hz.bjfxy.top/gtvwtdfdxf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yonumen.top/gtiovgiduq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.52xcode.cn/gtwimdyjur.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xziqi.cn/gtiljdxqtp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tanke756.top/gtfzecavbf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.feifeiyinyue.top/gtkbaxgpnx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yuanzhike.top/gtvopwrymu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shzxlz.cn/gtbqxjapvg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hysaishi.cn/gtqnygdecn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.smart0.xyz/gtygvfsqti.html

================================================================================
来源：http://hz.yongpay.top/gtwruiodbp.html

O. 并发与异步
来源：http://hz.dianchejie.cn/gtizkvkkra.html

================================================================================
来源：http://hz.yvedp.cn/gtczatuzit.html

[O01] 启动一个线程
来源：http://hz.zhongyouzk.top/gtuyqbynmm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinqigfzy.top/gtmsvdrvgr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ydjk.org.cn/gtlpxpzdtd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jinqigufen.top/gtykszkbxu.html

TS:   // 同 JS
来源：http://hz.dianchejie.cn/gterawsini.html

Java: new Thread(() -> f()).start()
来源：http://hz.aibaodan.cn/gtvtcatkne.html

Go:   go f()
来源：http://hz.nwbrower.top/gtfrcyyvyy.html

Ruby: Thread.new { f }
来源：http://hz.jianghu66.top/gtmskhopri.html

C#:   Task.Run(() => F());
来源：http://hz.svipenyu.cn/gtgektudny.html

[O02] 使用线程池
来源：http://hz.wangdashe.top/gtmkorcvmh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.mhx1999.top/gtovbojkrl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.0kj1m.cn/gtjkrbrimp.html

JS:   // worker_threads 线程池
来源：http://hz.hongshengwenyu.top/gtezzalvji.html

TS:   // worker_threads 线程池
来源：http://hz.xylfe.cn/gtdephjqcn.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yj20258888.top/gtojjhdhet.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yvedp.cn/gtoztggxxl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hnxiangtu.top/gtskenfnhd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jiagoushi.top/gtjdlnfusd.html

[O03] 加锁保护共享数据
来源：http://hz.smart0.xyz/gtuqdfsbpt.html

Py:   with lock: shared += 1
来源：http://hz.316326.xyz/gtcptxgcbz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jiagoushi.top/gtrwmfsqck.html


<!-- 参考信息 -->