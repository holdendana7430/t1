代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.feifeiyinyue.top/gtncyfqktq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nwbrower.top/gtsaobdchj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gzhubu.top/gtvfuapfov.html

Py:   pickle.dumps(obj)
来源：http://hz.jlsjyb.cn/gttouxvonm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.nanxuanxn.top/gtrdzmbqgy.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gotoacloud.top/gtlfglauxf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jinghuilouyu.cn/gtpwmprqyd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.dashuyun.cn/gthkfbrwwe.html

Go:   encoding/gob
来源：http://hz.jinqigfzy.top/gtvmqskzus.html

Ruby: Marshal.dump(obj)
来源：http://hz.guannengcc.top/gtebfnfhlc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.dashuyun.cn/gtytpduzci.html

================================================================================
来源：http://hz.zdqjudy.top/gtutjpyquf.html

L. 网络请求
来源：http://hz.gogol.net.cn/gtndyqjqsn.html

================================================================================
来源：http://hz.hysaishi.cn/gtqgjdmobi.html

[L01] 发送 GET 请求
来源：http://hz.shzxlz.cn/gtmxveppgc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jqgufenzy.top/gtydlnkhwd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hnqzz.top/gtehhnmprt.html

JS:   await fetch(url)
来源：http://hz.redwolf501.top/gtacrhalgk.html

TS:   await fetch(url)
来源：http://hz.xinyue.icu/gtrliyceyf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cheryme.top/gtdywxhgfa.html

Go:   resp, err := http.Get(url)
来源：http://hz.xziqi.cn/gtrxoocchh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenjidiqi.icu/gtfshbcnma.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj20258.top/gtxwfruhjq.html

[L02] 发送 POST JSON
来源：http://hz.c1oappe.top/gtmaciwgkd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jinyuanbaomall.cn/gtvedmgopg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.shangyingyoupin.top/gtlddttglk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jqgufenzy.top/gtvjjvryhk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.kuanghao11.cn/gtebcstekh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.guowangkeji.top/gtthgioijp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhoulong.xyz/gtwnnhkjtm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ivvv.top/gtekfmdsqi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.andypj.xyz/gttugdprvp.html

[L03] 设置自定义请求头
来源：http://hz.nanxuanxn.top/gtdaayxplk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nwbrower.top/gtruppufzh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhoulong.xyz/gtozfskaqg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.9152youxi.cn/gtqcnhrxvp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cheryme.top/gtbrvttede.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yanxiufei.cn/gtgqftgdmy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinqigfzy.top/gtrfzbseqr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.vqdsnc.cn/gtfgmzpnpx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jyoumei.cn/gtznuhluqb.html

[L04] 设置超时
来源：http://hz.xuanzx.com/gtnrhgcmeq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hywenlv.cn/gtynsavqcg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.daria6918.cn/gtcswxtrqd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinghuilouyu.cn/gtscbghnps.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fengsongda.top/gttapgfqkb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.kuanghao11.cn/gtlgndvgro.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sxryk.cn/gtsiomukhw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jianghu66.top/gtdrtyycbf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhengqikj.top/gtlcssngtb.html

[L05] 上传文件（multipart）
来源：http://hz.smart0.xyz/gtacoarlen.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ivvv.top/gtazopamhg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.tian-w.cn/gtyrsomsca.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangdashe.top/gtrcvqticp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhongyouzk.top/gtsjxokluy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.meibo888.top/gtkqsfmrnt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ybcxt.top/gtjtkfrizs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhixingplan.top/gtkpvoscrg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yueranfly.top/gtvpxfjrot.html

[L06] 解析响应为 JSON
来源：http://hz.quarkkingdee.top/gtyelqvatu.html

Py:   resp.json()
来源：http://hz.wangdashe.top/gtnfmjhiih.html

PHP:  json_decode($body, true);
来源：http://hz.yvedp.cn/gtqtsxdpqn.html

JS:   await resp.json()
来源：http://hz.gaohongyu789.top/gtyrnfuzvp.html

TS:   await resp.json()
来源：http://hz.zhoulong.xyz/gttcnunufj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.tian-w.cn/gtfqoanffp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.kuanghao11.cn/gtuxqneuzs.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hammf.cn/gtijxbvydq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cdnleiting.top/gtbflreffn.html

[L07] 处理 HTTP 状态码
来源：http://hz.shanyushiyangtech.top/gtunbwedop.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hnqzz.top/gtmnayvzfu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinghuilouyu.cn/gtrsqwlbcq.html

JS:   resp.ok;  resp.status
来源：http://hz.havefunace.top/gtadeubrmo.html

TS:   resp.ok;  resp.status
来源：http://hz.yonumen.top/gtfzkziogh.html

Java: resp.statusCode()
来源：http://hz.cheryme.top/gtfoeabtbi.html

Go:   resp.StatusCode
来源：http://hz.sxryk.cn/gtmsueoyvi.html

Ruby: resp.code.to_i
来源：http://hz.haohaochexian.top/gtqnokaeug.html

C#:   (int)resp.StatusCode
来源：http://hz.hfpthk.cn/gtgvancqff.html

[L08] 并发请求多个地址
来源：http://hz.ybcxt.top/gtxckawrlk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ybcxt.top/gtmwvwjkmy.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhijiandao.cn/gtkbqstbfr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.bjfxy.top/gtjgceduuz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gthtjczaia.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhiwuduotai.top/gtntsdtwxp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jlsjyb.cn/gtqkrdpdcc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.9152youxi.cn/gtevjpnqcz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ppjwa.cn/gtvoovnzgv.html

================================================================================
来源：http://hz.gogol.net.cn/gtxajcpqsr.html

M. 命令行 / 进程 / 环境
来源：http://hz.smart0.xyz/gtdejmxmlg.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtxmmizzla.html

[M01] 读取命令行参数
来源：http://hz.xinyue.icu/gtfqnydmap.html

Py:   sys.argv[1:]
来源：http://hz.daria6918.cn/gtpbfkntlw.html

PHP:  $argv;  $argc;
来源：http://hz.cqqwz.cn/gtnpafctur.html

JS:   process.argv.slice(2)
来源：http://hz.xylfe.cn/gthkmhiiwq.html

TS:   process.argv.slice(2)
来源：http://hz.nwbrower.top/gtrsvumfwp.html

Java: args 数组（main 方法参数）
来源：http://hz.snrcjt.cn/gtmtighmoe.html

Go:   os.Args[1:]
来源：http://hz.daria6918.cn/gtabyvrenh.html

Ruby: ARGV
来源：http://hz.jianghu66.top/gttexqksdb.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinghuilouyu.cn/gtrdbdbbgm.html

[M02] 读取环境变量
来源：http://hz.nwbrower.top/gtrafbgind.html

Py:   os.environ.get("HOME")
来源：http://hz.ywan-chungtsiang.top/gtyqbutqcx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenlongwang.top/gtsppglnnm.html

JS:   process.env.HOME
来源：http://hz.tianlin.xyz/gtumoehzri.html

TS:   process.env.HOME
来源：http://hz.yj20258888.top/gthccdlhgd.html

Java: System.getenv("HOME")
来源：http://hz.yj202588.top/gtefyidasu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cdnleiting.top/gtfvqmjntp.html

Ruby: ENV["HOME"]
来源：http://hz.ydjk.org.cn/gtpmyirigy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.wangdashe.top/gtpedavzaj.html

[M03] 执行外部命令
来源：http://hz.iojbl.cn/gtbqhorduf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xuetiantiany.cn/gtpohpzawh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cqqwz.cn/gtdiwwxpix.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.mhx1999.top/gtolfswkha.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.meibo888.top/gtxxmyafnn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sxryk.cn/gtnxzlaxok.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.9152youxi.cn/gtwribtsfr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.dianchejie.cn/gtlxsyhbiy.html

C#:   Process.Start("ls", "-l");
来源：http://hz.nanxuanxn.top/gtyxmrgpll.html

[M04] 获取当前工作目录
来源：http://hz.birdmap.top/gtjxywnbky.html

Py:   os.getcwd()
来源：http://hz.iojbl.cn/gtzecfvahv.html

PHP:  getcwd();
来源：http://hz.jiagoushi.top/gtpfwmmvdf.html

JS:   process.cwd()
来源：http://hz.yvedp.cn/gtaowtjswr.html

TS:   process.cwd()
来源：http://hz.cucudq.cn/gtkivdyhva.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.aibaodan.cn/gtstgmkzvs.html

Go:   os.Getwd()
来源：http://hz.snrcjt.cn/gtyvntallj.html

Ruby: Dir.pwd
来源：http://hz.yj20258888.top/gtqcmrigoj.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gaohongyu789.top/gtvjfglldt.html

[M05] 设置退出码
来源：http://hz.dianchejie.cn/gtikmfmytx.html

Py:   sys.exit(1)
来源：http://hz.jinqigfzy.top/gtuefpgjrf.html

PHP:  exit(1);
来源：http://hz.jqgfzy.top/gtroeujypd.html

JS:   process.exit(1)
来源：http://hz.ppjwa.cn/gtidberkpu.html

TS:   process.exit(1)
来源：http://hz.jlsjyb.cn/gtpcvkpyqj.html

Java: System.exit(1)
来源：http://hz.zycfv.cn/gtfoybzzne.html

Go:   os.Exit(1)
来源：http://hz.cheryme.top/gtzbgoerwz.html

Ruby: exit 1
来源：http://hz.dianchejie.cn/gtuarsubzx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sxryk.cn/gtqcesgyaq.html

[M06] 向标准错误输出
来源：http://hz.jinyuanbaomall.cn/gtyygwlues.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shangyingyoupin.top/gthenjugyt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yuxming.cn/gtuhmfbsyp.html

JS:   console.error("err")
来源：http://hz.vqdsnc.cn/gtyllpywbp.html

TS:   console.error("err")
来源：http://hz.xinyue.icu/gtorqhbfue.html

Java: System.err.println("err")
来源：http://hz.yangfankeji.com/gtycozdkbw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.smart0.xyz/gtbinlemsg.html

Ruby: warn "err"
来源：http://hz.hfpthk.cn/gtakvqlokn.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.fengsongda.top/gtjhuihbec.html

[M07] 判断是否为主入口
来源：http://hz.snrcjt.cn/gtbqnelqip.html

Py:   if __name__ == "__main__":
来源：http://hz.xinyue.icu/gtqlktygym.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jianghu66.top/gtacdfryvx.html

JS:   require.main === module
来源：http://hz.hnqzz.top/gtfkuqnzou.html

TS:   require.main === module
来源：http://hz.feifeiyinyue.top/gtipdgpihp.html

Java: public static void main(String[] args)
来源：http://hz.birdmap.top/gtwfoezrke.html

Go:   func main()
来源：http://hz.daria6918.cn/gtuhezfkgh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ydzc1.top/gtmqczgptx.html

C#:   static void Main(string[] args)
来源：http://hz.chenjidiqi.icu/gtsvyxhepj.html

[M08] 获取系统与运行时信息
来源：http://hz.jlsjyb.cn/gtkikmkmxh.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yuanzhike.top/gtdxbgipxj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xylfe.cn/gtxpzpvmff.html

JS:   process.platform;  process.version
来源：http://hz.xingfuxueyuan.xyz/gtsobfxaal.html

TS:   process.platform;  process.version
来源：http://hz.jyoumei.cn/gtpbhxigkn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.nanxinkj.top/gtbcvcqcem.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zycfv.cn/gtqjulitfe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cucudq.cn/gtptpsqjan.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ydzc1.top/gtuxrcfcuz.html

================================================================================
来源：http://hz.zhongyouzk.top/gtrmcwsokp.html

N. 数据结构与算法
来源：http://hz.zhongyouzk.top/gtspwuetec.html

================================================================================
来源：http://hz.yj20258888.top/gttbbmmevd.html

[N01] 二分查找（有序数组）
来源：http://hz.shangyingyoupin.top/gtijufovnu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zdqjudy.top/gtwtkyprzn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cucudq.cn/gtvxtqriwa.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hammf.cn/gtftplwhgq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ybcxt.top/gtlsfljtjs.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hnqzz.top/gtpfgpnuze.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtstuhnren.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinqigufen.top/gtxzjurpxq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.tian-w.cn/gtzlzcuizd.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhengqikj.top/gtpnjwultb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenjidiqi.icu/gtvcsgtcgx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.snrcjt.cn/gtkhgwrznh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guannengcc.top/gtlujofakl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gtrqdfbomc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinyuanbaomall.cn/gtljeofzwh.html

Go:   slices.Sort(arr)
来源：http://hz.ywan-chungtsiang.top/gthtdpvmzb.html

Ruby: arr.sort
来源：http://hz.pengpengdd.cyou/gtbbgwprwu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.tanke756.top/gtnrrdskll.html

[N03] 快速排序（分治示例）
来源：http://hz.yvedp.cn/gtdfxiqovm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.andypj.xyz/gtqmzdldym.html

PHP:  // 递归实现，或用 usort
来源：http://hz.c1oappe.top/gtciuncvxz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydzc1.top/gtuurqqpnd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sufxvd.cn/gtajlcpvjz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cheryme.top/gtyptxsovi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hammf.cn/gtyzhnhriw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenlongwang.top/gtooshxaut.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhoulong.xyz/gtaqxqsdes.html

[N04] 斐波那契数列
来源：http://hz.guannengcc.top/gtthzuljug.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shangyingyoupin.top/gtqrvolwsa.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.wangshuangyany.cn/gttocjkbga.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenjidiqi.icu/gtckbfcncv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jianghu66.top/gtgulcfmnb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xziqi.cn/gtrzygfvsu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.tianlin.xyz/gtaewjafva.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.haohaochexian.top/gtbxcdcqpu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ppjwa.cn/gtixziraxi.html

[N05] 最大公约数
来源：http://hz.hammf.cn/gtcfwcapwa.html

Py:   math.gcd(a, b)
来源：http://hz.ydjk.org.cn/gteumebgfp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ehwqpu.com/gtvzresjib.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.kuanghao11.cn/gtvfijxprh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cheryme.top/gtdweiemrk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ybcxt.top/gtrcteoowv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jlsjyb.cn/gtrggxrxbr.html

Ruby: a.gcd(b)
来源：http://hz.xylfe.cn/gtuoopdchj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhoulong.xyz/gtrtnpbrkx.html

[N06] 判断回文字符串
来源：http://hz.hywenlv.cn/gtazrnggvr.html

Py:   s == s[::-1]
来源：http://hz.zdqjudy.top/gtymnesopq.html

PHP:  $s === strrev($s);
来源：http://hz.gaohongyu789.top/gtchlzjyhp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenjidiqi.icu/gtbhtapxms.html

TS:   s === [...s].reverse().join("")
来源：http://hz.meibo888.top/gtrtehntzt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.chenzaomai.com/gtxflcytge.html

Go:   // 双指针从两端比较
来源：http://hz.tian-w.cn/gtottlvvfc.html

Ruby: s == s.reverse
来源：http://hz.xinyue.icu/gtnnkjxdfm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yj202588.top/gtqvhxtqti.html

[N07] 两数之和（返回下标）
来源：http://hz.iojbl.cn/gtbfgmubok.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gotoacloud.top/gtibezqmvh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xylfe.cn/gtogdbyenf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shzxlz.cn/gtpjmevnpp.html

TS:   // 手写 Map<string, number>
来源：http://hz.pengpengdd.cyou/gtylnaunco.html

Java: // 手写 HashMap
来源：http://hz.yj20258888.top/gtteugjhkv.html

Go:   // 手写 map[int]int
来源：http://hz.hywenlv.cn/gtelpzidru.html

Ruby: // 手写 Hash
来源：http://hz.zhengqikj.top/gtnpfbenjz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ywan-chungtsiang.top/gtmfksjwmb.html

[N08] 生成全排列
来源：http://hz.daria6918.cn/gtlbyfpcdy.html

Py:   itertools.permutations(arr)
来源：http://hz.hnqzz.top/gtlcdmoryu.html

PHP:  // 手写递归交换
来源：http://hz.hfpthk.cn/gtkknnawbf.html

JS:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtroolvmsj.html

TS:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtciofmaqb.html

Java: // 手写回溯递归
来源：http://hz.xylfe.cn/gtildieuxx.html

Go:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtabxbgnxo.html

Ruby: arr.permutation.to_a
来源：http://hz.zycfv.cn/gtcrldegak.html

C#:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtaseqkrqd.html

[N09] 栈与队列
来源：http://hz.ehwqpu.com/gtkhvptwid.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shangyingyoupin.top/gtcwssbesg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yvedp.cn/gtpdjacvfm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.sweek.top/gtpvxbiwuz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cheryme.top/gtwpridozo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hnxiangtu.top/gtiakidekc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhengqikj.top/gtprmvltxc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.dashuyun.cn/gtarndtoiu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhaomingkeji.xyz/gthklgybts.html

[N10] 链表节点定义
来源：http://hz.sysykeji.top/gtwiawazic.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.52xcode.cn/gtrazhqbka.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.andypj.xyz/gthtzbptkv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hnqzz.top/gtvxjjaugv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.wangshuangyany.cn/gtnketdaci.html

Java: class Node { int v; Node next; }
来源：http://hz.dianchejie.cn/gtytrmbjhd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.snrcjt.cn/gtijemrbkc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.nwbrower.top/gtmihhelhy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.c1oappe.top/gtdbivhnxr.html

[N11] 二叉树中序遍历
来源：http://hz.aibaodan.cn/gtvydpwefl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.kuanghao11.cn/gtouixtodp.html

PHP:  // 手写递归函数
来源：http://hz.yvedp.cn/gttbqzjkiv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydjk.org.cn/gtoxmjzrdq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinqigfzy.top/gtakipkekw.html

Java: // 手写递归
来源：http://hz.ywan-chungtsiang.top/gtkpggjgum.html

Go:   // 手写递归
来源：http://hz.hongshengwenyu.top/gteyfzrfyq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.havefunace.top/gtsnntkpho.html

C#:   // 手写递归
来源：http://hz.xuanzx.com/gtqawbofiu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ywan-chungtsiang.top/gtghrafnlx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenzaomai.com/gtujieilan.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.pycfn.com/gtflollefp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ehwqpu.com/gtyhrysdjm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shuidangran.top/gtbcporemb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuetiantiany.cn/gtoshnlzef.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jyoumei.cn/gtieflmcgu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.smart0.xyz/gtrfdprddk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fengsongda.top/gtgphbfehe.html

================================================================================
来源：http://hz.chenlongwang.top/gthteiewnm.html

O. 并发与异步
来源：http://hz.gogol.net.cn/gtumbcgxvc.html

================================================================================
来源：http://hz.iojbl.cn/gtlpaukkpu.html

[O01] 启动一个线程
来源：http://hz.shangyingyoupin.top/gtccgvvhvt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.quarkkingdee.top/gtwfoikbae.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.wangshuangyany.cn/gtuogsswzd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ydjk.org.cn/gtcsjpldfw.html

TS:   // 同 JS
来源：http://hz.daria6918.cn/gtemybpxmd.html

Java: new Thread(() -> f()).start()
来源：http://hz.hfpthk.cn/gtqnvzdfkk.html

Go:   go f()
来源：http://hz.mhx1999.top/gtqxbmggnr.html

Ruby: Thread.new { f }
来源：http://hz.zhoulong.xyz/gttmvvwhre.html

C#:   Task.Run(() => F());
来源：http://hz.kuanghao11.cn/gtfekpbsvs.html

[O02] 使用线程池
来源：http://hz.gaohongyu789.top/gtmfwwqiow.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.fzhhl.top/gtpsnrbcjt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jqgufenzy.top/gtnbaqmmyr.html

JS:   // worker_threads 线程池
来源：http://hz.gaohongyu789.top/gtlzhuvuaa.html

TS:   // worker_threads 线程池
来源：http://hz.guannengcc.top/gtlkegmdiq.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.316326.xyz/gtaqklmlzu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xuanzx.com/gtckdldtra.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinghuilouyu.cn/gtolqnymly.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.chenzaomai.com/gtrioetmux.html

[O03] 加锁保护共享数据
来源：http://hz.xinyue.icu/gttkwbleam.html

Py:   with lock: shared += 1
来源：http://hz.vqdsnc.cn/gtelkndaqr.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jianghu66.top/gthreukrlq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenzaomai.com/gtkuaeiatz.html

TS:   // 同 JS
来源：http://hz.nwbrower.top/gtboisknqs.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhongyouzk.top/gtucmenvcd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zdqjudy.top/gtndvkgytb.html


<!-- 参考信息 -->