代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.wangshuangyany.cn/gtofbmttvd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xuetiantiany.cn/gtsivirhmc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yongpay.top/gtvuqqnqlm.html

Py:   pickle.dumps(obj)
来源：http://hz.redwolf501.top/gtsozszewt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinghuilouyu.cn/gtniugvbct.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.bjfxy.top/gtecxeqele.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jqgufenzy.top/gtyfueqfjw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hongshengwenyu.top/gtlcyyheju.html

Go:   encoding/gob
来源：http://hz.jlsjyb.cn/gtmrovkzar.html

Ruby: Marshal.dump(obj)
来源：http://hz.guannengcc.top/gtoduwtqxm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhiwuduotai.top/gtkpvxkunn.html

================================================================================
来源：http://hz.tanke756.top/gtzaavmwhv.html

L. 网络请求
来源：http://hz.shanyushiyangkeji.top/gtmxmpasnp.html

================================================================================
来源：http://hz.ivvv.top/gthypwyaga.html

[L01] 发送 GET 请求
来源：http://hz.bjfxy.top/gtrioiipqf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ydjk.org.cn/gtevtevxfg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.bjfxy.top/gtgcuxemsh.html

JS:   await fetch(url)
来源：http://hz.xinyue.icu/gtfrptdjdq.html

TS:   await fetch(url)
来源：http://hz.guannengcc.top/gtlatbplty.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yj20258.top/gtxwsvrthi.html

Go:   resp, err := http.Get(url)
来源：http://hz.hnqzz.top/gtjqdgwtwf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ydzc1.top/gthkwaccew.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.daria6918.cn/gtdrpwgcjh.html

[L02] 发送 POST JSON
来源：http://hz.kuanghao11.cn/gtrbtyxqrn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.wangdashe.top/gturiikqub.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhoulong.xyz/gthkugmahh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gaohongyu789.top/gtrbbauaoq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jlsjyb.cn/gtgdxxrnlx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yueranfly.top/gtehaebgav.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.chenzaomai.com/gtekeltzhc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jqgufenzy.top/gtnjobufow.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.daria6918.cn/gtlmnrhxoh.html

[L03] 设置自定义请求头
来源：http://hz.sweek.top/gtfjeukorh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yvedp.cn/gtecfkryfy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sysykeji.top/gtxpgokaji.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.c1oappe.top/gtlnvftduv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuanzx.com/gtydektyao.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ppjwa.cn/gtpbliiisg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yuxming.cn/gtjaurisde.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.kuanghao11.cn/gtoeswxnzt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuanzhike.top/gtihamhfbi.html

[L04] 设置超时
来源：http://hz.yvedp.cn/gtoajmfqat.html

Py:   requests.get(url, timeout=5)
来源：http://hz.dianchejie.cn/gteavxoiap.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hongshengwenyu.top/gtxbaywdeb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sweek.top/gtlylpubsa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj202588.top/gtrpbgaisr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xuetiantiany.cn/gtkehclnty.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xinyue.icu/gtrviggovq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yanxiufei.cn/gtadbtdltj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.tanke756.top/gtfnxiscew.html

[L05] 上传文件（multipart）
来源：http://hz.mhx1999.top/gttjwnexah.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hywenlv.cn/gteubxnqeb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xingfuxueyuan.xyz/gtbvpngsrf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenlongwang.top/gtkktneauj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.c1oappe.top/gtxqnsplwu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ehwqpu.com/gtmuthgrtw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sysykeji.top/gtavgyvdys.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jianghu66.top/gtfopemvww.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.aibaodan.cn/gtrvdlotmg.html

[L06] 解析响应为 JSON
来源：http://hz.kuanghao11.cn/gtvqyybyza.html

Py:   resp.json()
来源：http://hz.yangfankeji.com/gtpjizolvf.html

PHP:  json_decode($body, true);
来源：http://hz.fzhhl.top/gtqxuaicmw.html

JS:   await resp.json()
来源：http://hz.sufxvd.cn/gtdoruovhj.html

TS:   await resp.json()
来源：http://hz.gzhubu.top/gttclsapzh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhoulong.xyz/gthnkpkeun.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.fzhhl.top/gtbpstqivr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenjidiqi.icu/gtsmpjrnkn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hfpthk.cn/gtwaepshua.html

[L07] 处理 HTTP 状态码
来源：http://hz.yuxming.cn/gtiwxeconm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenlongwang.top/gtzsltqmzn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xylfe.cn/gtccyywrpe.html

JS:   resp.ok;  resp.status
来源：http://hz.zycfv.cn/gtqzyemfzd.html

TS:   resp.ok;  resp.status
来源：http://hz.0kj1m.cn/gtmehndevx.html

Java: resp.statusCode()
来源：http://hz.meibo888.top/gtttsddudp.html

Go:   resp.StatusCode
来源：http://hz.zhixingplan.top/gtsdqemmbe.html

Ruby: resp.code.to_i
来源：http://hz.fengsongda.top/gtthbdbemv.html

C#:   (int)resp.StatusCode
来源：http://hz.c1oappe.top/gtlihflhbj.html

[L08] 并发请求多个地址
来源：http://hz.hfpthk.cn/gtcmmbnhbe.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.andypj.xyz/gtzslkqxxg.html

PHP:  curl_multi_init() 系列
来源：http://hz.ybcxt.top/gtcrtoduej.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cdnleiting.top/gtjlweomxj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigfzy.top/gtyapotwhc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hysaishi.cn/gtmwkzjpxc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yonumen.top/gtmfxstpfp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yuanzhike.top/gtqjryyvog.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.smart0.xyz/gtbnoabkdb.html

================================================================================
来源：http://hz.fzhhl.top/gtgfhisrrb.html

M. 命令行 / 进程 / 环境
来源：http://hz.52xcode.cn/gtcxotzekg.html

================================================================================
来源：http://hz.shuidangran.top/gtltaovfpj.html

[M01] 读取命令行参数
来源：http://hz.ehwqpu.com/gtrvgofbnt.html

Py:   sys.argv[1:]
来源：http://hz.chenjidiqi.icu/gtrwzzhyrq.html

PHP:  $argv;  $argc;
来源：http://hz.0kj1m.cn/gtdnsibqry.html

JS:   process.argv.slice(2)
来源：http://hz.kuanghao11.cn/gthzvhvazu.html

TS:   process.argv.slice(2)
来源：http://hz.xziqi.cn/gtcgexrnit.html

Java: args 数组（main 方法参数）
来源：http://hz.feifeiyinyue.top/gtxnbvvtqc.html

Go:   os.Args[1:]
来源：http://hz.yongpay.top/gtapaayspk.html

Ruby: ARGV
来源：http://hz.zhijiandao.cn/gtbrkkjaug.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hywenlv.cn/gtymznmsnv.html

[M02] 读取环境变量
来源：http://hz.ivvv.top/gtlbrgikrg.html

Py:   os.environ.get("HOME")
来源：http://hz.dianchejie.cn/gtpdzggawx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cdnleiting.top/gtqrhlespj.html

JS:   process.env.HOME
来源：http://hz.dianchejie.cn/gtuoeokjsf.html

TS:   process.env.HOME
来源：http://hz.ppjwa.cn/gtjjeeitns.html

Java: System.getenv("HOME")
来源：http://hz.zhengqikj.top/gtipumepgk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yj20258.top/gtegllcest.html

Ruby: ENV["HOME"]
来源：http://hz.tian-w.cn/gtiufdoqmx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ybcxt.top/gtytdodmaq.html

[M03] 执行外部命令
来源：http://hz.jianghu66.top/gtbcffkqqo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cheryme.top/gtfprzynhr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gzhubu.top/gtmdthpfdy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yueranfly.top/gtazqajkyb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xylfe.cn/gtwmylkgzi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.nanxinkj.top/gtyuclbafo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xinyue.icu/gtdjgvvosh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shuidangran.top/gtxhzyriyn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.guannengcc.top/gtygvquuti.html

[M04] 获取当前工作目录
来源：http://hz.guannengcc.top/gtbqmxboas.html

Py:   os.getcwd()
来源：http://hz.yvedp.cn/gtwzkqoyvv.html

PHP:  getcwd();
来源：http://hz.zhijiandao.cn/gtnvzatguc.html

JS:   process.cwd()
来源：http://hz.xziqi.cn/gtrfdnlmbu.html

TS:   process.cwd()
来源：http://hz.ivvv.top/gtgndzxyjn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hysaishi.cn/gtcwssytui.html

Go:   os.Getwd()
来源：http://hz.guowangkeji.top/gtavjdqefl.html

Ruby: Dir.pwd
来源：http://hz.yanxiufei.cn/gtlrrolres.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.nanxuanxn.top/gtvyimhrfo.html

[M05] 设置退出码
来源：http://hz.gzhubu.top/gtbpklqhud.html

Py:   sys.exit(1)
来源：http://hz.hongshengwenyu.top/gtkrovwrmz.html

PHP:  exit(1);
来源：http://hz.zhengqikj.top/gtlofmffdh.html

JS:   process.exit(1)
来源：http://hz.aizwys.cn/gtzhevohcz.html

TS:   process.exit(1)
来源：http://hz.ybcxt.top/gthalednof.html

Java: System.exit(1)
来源：http://hz.meibo888.top/gtlbugnhmi.html

Go:   os.Exit(1)
来源：http://hz.jyoumei.cn/gtrpamjldb.html

Ruby: exit 1
来源：http://hz.hongshengwenyu.top/gtfhkskimo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ydzc1.top/gtuzjnatal.html

[M06] 向标准错误输出
来源：http://hz.jinqigfzy.top/gthyilqpbr.html

Py:   print("err", file=sys.stderr)
来源：http://hz.bjfxy.top/gtafbemdru.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenlongwang.top/gtifhxokue.html

JS:   console.error("err")
来源：http://hz.cashguo.top/gtzhtrdnws.html

TS:   console.error("err")
来源：http://hz.wangdashe.top/gtotpkhrak.html

Java: System.err.println("err")
来源：http://hz.zhongyouzk.top/gtrbmgbhpz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gogol.net.cn/gtijwwproh.html

Ruby: warn "err"
来源：http://hz.yuanzhike.top/gthewavcla.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cashguo.top/gtyiplgffv.html

[M07] 判断是否为主入口
来源：http://hz.xingfuxueyuan.xyz/gttenhadtr.html

Py:   if __name__ == "__main__":
来源：http://hz.shangyingyoupin.top/gticdhqbik.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yueranfly.top/gtgvuenfsf.html

JS:   require.main === module
来源：http://hz.fzhhl.top/gtwplerxyp.html

TS:   require.main === module
来源：http://hz.yangfankeji.com/gtdddywewm.html

Java: public static void main(String[] args)
来源：http://hz.yanxiufei.cn/gtzheazveu.html

Go:   func main()
来源：http://hz.0kj1m.cn/gttlfbvgbs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.0kj1m.cn/gtfnwqkmxz.html

C#:   static void Main(string[] args)
来源：http://hz.nanxuanxn.top/gtykxjjjqq.html

[M08] 获取系统与运行时信息
来源：http://hz.ywan-chungtsiang.top/gtnwqvdybi.html

Py:   platform.system();  platform.python_version()
来源：http://hz.tianlin.xyz/gtaknnfinm.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shanyushiyangtech.top/gtypyngsbz.html

JS:   process.platform;  process.version
来源：http://hz.nanxinkj.top/gtuwxtrdee.html

TS:   process.platform;  process.version
来源：http://hz.yongpay.top/gtzhttwmpm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ydjk.org.cn/gtsazlmipc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.guannengcc.top/gtfvaycpsn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hongshengwenyu.top/gtldulurxc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj20258888.top/gtgdlnzesj.html

================================================================================
来源：http://hz.havefunace.top/gttscxsvmu.html

N. 数据结构与算法
来源：http://hz.jianghu66.top/gtneqpqmrt.html

================================================================================
来源：http://hz.hnxiangtu.top/gtnzrbbxdp.html

[N01] 二分查找（有序数组）
来源：http://hz.ydzc1.top/gtcuunxyxq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hfpthk.cn/gtgybzijrt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jianghu66.top/gtzwvtfjnj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hammf.cn/gtuuumfqcl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.birdmap.top/gtqzlasgre.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jinqigfzy.top/gtoiydbktk.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.sysykeji.top/gturwzqhyc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hnqzz.top/gtkzsaabgj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hongshengwenyu.top/gtxrjckczr.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.dianchejie.cn/gtkohmzbdi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jlsjyb.cn/gtoglnxija.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhengqikj.top/gtntrzuapy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sufxvd.cn/gtylcjjism.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yangfankeji.com/gtxbjxuuue.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.vqdsnc.cn/gtuirrppab.html

Go:   slices.Sort(arr)
来源：http://hz.yj20258.top/gtiobfuqqb.html

Ruby: arr.sort
来源：http://hz.yonumen.top/gtblrgeygd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinghuilouyu.cn/gtwbqxnwql.html

[N03] 快速排序（分治示例）
来源：http://hz.bjfxy.top/gtvzvyaujv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ywan-chungtsiang.top/gtgjyrvvjk.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xziqi.cn/gtgylfptbp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gogol.net.cn/gttwvhoqga.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhoulong.xyz/gttdxavclt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.wangshuangyany.cn/gtsnhadsrz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.316326.xyz/gtasxpbgwt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hnqzz.top/gtgpwnmhqc.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.aizwys.cn/gtcshroxnm.html

[N04] 斐波那契数列
来源：http://hz.shzxlz.cn/gtrafcboyp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhaomingkeji.xyz/gttfisdnso.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xuanzx.com/gtyixlesxg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aizwys.cn/gtjmbqaiqv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhixingplan.top/gtlffnebjy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hywenlv.cn/gtkkqgpgdr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhaomingkeji.xyz/gtmbjgyamv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xziqi.cn/gtirsrpyzg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ydzc1.top/gtjtfsoeqn.html

[N05] 最大公约数
来源：http://hz.yvedp.cn/gttinvvqyz.html

Py:   math.gcd(a, b)
来源：http://hz.quarkkingdee.top/gtipfiphan.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xinyue.icu/gtpofmckie.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xylfe.cn/gtquvpbvao.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gtffxjrwzf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ywan-chungtsiang.top/gtcvnxponm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenzaomai.com/gtvkhfhlvb.html

Ruby: a.gcd(b)
来源：http://hz.tianlin.xyz/gtviddhpsy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gzhubu.top/gttwdidwwy.html

[N06] 判断回文字符串
来源：http://hz.tianlin.xyz/gtvhyrsqsk.html

Py:   s == s[::-1]
来源：http://hz.ivvv.top/gtbgnzgseh.html

PHP:  $s === strrev($s);
来源：http://hz.yueranfly.top/gthafmuwvg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtdcgqgoea.html

TS:   s === [...s].reverse().join("")
来源：http://hz.fengsongda.top/gtlwezohxb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.52xcode.cn/gtfixwptvd.html

Go:   // 双指针从两端比较
来源：http://hz.jyoumei.cn/gtmqlcrqvp.html

Ruby: s == s.reverse
来源：http://hz.yanxiufei.cn/gtmrukjoze.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ydjk.org.cn/gtfuylmydz.html

[N07] 两数之和（返回下标）
来源：http://hz.nwbrower.top/gtvtlzhefy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ybcxt.top/gtxqnhkqgp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.svipenyu.cn/gtdymytbnd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.pengpengdd.cyou/gtedvocluc.html

TS:   // 手写 Map<string, number>
来源：http://hz.dashuyun.cn/gtjcavyxur.html

Java: // 手写 HashMap
来源：http://hz.yonumen.top/gtnsbueysg.html

Go:   // 手写 map[int]int
来源：http://hz.sysykeji.top/gtqwoyxsll.html

Ruby: // 手写 Hash
来源：http://hz.jinqigufen.top/gtsaulslcw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.guowangkeji.top/gtxbpkrgkh.html

[N08] 生成全排列
来源：http://hz.52xcode.cn/gtusongbqq.html

Py:   itertools.permutations(arr)
来源：http://hz.0kj1m.cn/gtpqwurlrg.html

PHP:  // 手写递归交换
来源：http://hz.yj202588.top/gtqemnpgwa.html

JS:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtnklhyran.html

TS:   // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtltdugpwg.html

Java: // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtoxfreffd.html

Go:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtdvaycvnt.html

Ruby: arr.permutation.to_a
来源：http://hz.sysykeji.top/gteobpycru.html

C#:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtatledsdv.html

[N09] 栈与队列
来源：http://hz.pycfn.com/gtyltzayia.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shangyingyoupin.top/gtpgvywmai.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhiwuduotai.top/gtjygcsmix.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhijiandao.cn/gtvksxmtbq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.gzhubu.top/gtvxdldovq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.52xcode.cn/gtztwbndzn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhoulong.xyz/gttmakxoxw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.smart0.xyz/gtxrmaihec.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.andypj.xyz/gtshimguvu.html

[N10] 链表节点定义
来源：http://hz.feifeiyinyue.top/gtwuinsmxl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhiwuduotai.top/gtfmzphnae.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.wangdashe.top/gtkvnmazgt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.c1oappe.top/gtrcnxvper.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xuanzx.com/gtjxlazpbi.html

Java: class Node { int v; Node next; }
来源：http://hz.zhengqikj.top/gtaexlolso.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ppjwa.cn/gtvtuyisdm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.dashuyun.cn/gtxbsbixzk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.dashuyun.cn/gtjkiswrhj.html

[N11] 二叉树中序遍历
来源：http://hz.cashguo.top/gtrokfrvwx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.fzhhl.top/gtqguykzga.html

PHP:  // 手写递归函数
来源：http://hz.xinyue.icu/gtqyefsozs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fengsongda.top/gtylpkkjdc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gaohongyu789.top/gtditglqix.html

Java: // 手写递归
来源：http://hz.shanyushiyangkeji.top/gtastwxeto.html

Go:   // 手写递归
来源：http://hz.cucudq.cn/gtvdwtimuu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tianlin.xyz/gtgqxsyhgm.html

C#:   // 手写递归
来源：http://hz.smart0.xyz/gtgmluwmhr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yuanzhike.top/gtunsklset.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.pengpengdd.cyou/gtxdjvbogy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ydjk.org.cn/gtdlavivoa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jianghu66.top/gtwhhriipj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangdashe.top/gtealayizx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhixingplan.top/gtimwhxkjn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hfpthk.cn/gtwgsjdstg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.gzhubu.top/gtbrdhtiyb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hammf.cn/gtfslqfmrt.html

================================================================================
来源：http://hz.hfpthk.cn/gthfcaypon.html

O. 并发与异步
来源：http://hz.zhongyouzk.top/gtvhhnrkho.html

================================================================================
来源：http://hz.nanxinkj.top/gtgjnoavhs.html

[O01] 启动一个线程
来源：http://hz.vqdsnc.cn/gtxdygkkxd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.0kj1m.cn/gtxrvhhjcc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zycfv.cn/gtwvrvajfb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hywenlv.cn/gtrhxrvcql.html

TS:   // 同 JS
来源：http://hz.yj202588.top/gtfhvebbxk.html

Java: new Thread(() -> f()).start()
来源：http://hz.nanxuanxn.top/gtmbjpbfbl.html

Go:   go f()
来源：http://hz.guowangkeji.top/gtjqmzxxjs.html

Ruby: Thread.new { f }
来源：http://hz.shzxlz.cn/gtbsajpknw.html

C#:   Task.Run(() => F());
来源：http://hz.hammf.cn/gtihwydpkn.html

[O02] 使用线程池
来源：http://hz.aizwys.cn/gttbqtwlgz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.wangdashe.top/gtnqptsiqq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jqgfzy.top/gtwsjbklmz.html

JS:   // worker_threads 线程池
来源：http://hz.sufxvd.cn/gtzjrtcrng.html

TS:   // worker_threads 线程池
来源：http://hz.meibo888.top/gtgirfqfgp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jyoumei.cn/gtbggveron.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hywenlv.cn/gtjfnxftbi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ydjk.org.cn/gtoruqiagp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shuidangran.top/gticwwtcmv.html

[O03] 加锁保护共享数据
来源：http://hz.jinqigfzy.top/gtofcahcme.html

Py:   with lock: shared += 1
来源：http://hz.redwolf501.top/gtmpvbsvon.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xuetiantiany.cn/gtieeoefug.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.guowangkeji.top/gtdtkmfffm.html

TS:   // 同 JS
来源：http://hz.hysaishi.cn/gtrxghwato.html

Java: synchronized (this) { shared++; }
来源：http://hz.hammf.cn/gtssixdicw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.dianchejie.cn/gtyotdpoak.html


<!-- 参考信息 -->