代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.vqdsnc.cn/gtpjchvzbr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinqigfzy.top/gtzttmpeqe.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.smart0.xyz/gtdwnoyxlg.html

Py:   pickle.dumps(obj)
来源：http://hz.havefunace.top/gtkewsvajc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinghuilouyu.cn/gtsbbmeotf.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.haohaochexian.top/gtpwrbssho.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yanxiufei.cn/gtjukltsrc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.sweek.top/gtaskcefyx.html

Go:   encoding/gob
来源：http://hz.52xcode.cn/gtzbenewva.html

Ruby: Marshal.dump(obj)
来源：http://hz.dashuyun.cn/gtsdfbqfoq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.nanxinkj.top/gtiihnbfae.html

================================================================================
来源：http://hz.gogol.net.cn/gtdumjesfx.html

L. 网络请求
来源：http://hz.quarkkingdee.top/gtawziltyv.html

================================================================================
来源：http://hz.cucudq.cn/gtddsisvbu.html

[L01] 发送 GET 请求
来源：http://hz.zhixingplan.top/gtmtushvaa.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hnqzz.top/gtgefcxvho.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cashguo.top/gtvcxdeddf.html

JS:   await fetch(url)
来源：http://hz.shzxlz.cn/gtupzyqxyv.html

TS:   await fetch(url)
来源：http://hz.zhaomingkeji.xyz/gtpdzxusgs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zdqjudy.top/gtivbngeib.html

Go:   resp, err := http.Get(url)
来源：http://hz.birdmap.top/gtfgfodspf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.aizwys.cn/gtpcpimdtx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ywan-chungtsiang.top/gtkavpnhsw.html

[L02] 发送 POST JSON
来源：http://hz.redwolf501.top/gtlddoqfjn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jqgfzy.top/gtvpeswvcd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gogol.net.cn/gtajscsyoe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sufxvd.cn/gtvwxcyhii.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fengsongda.top/gtuoyuwquo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yuxming.cn/gtuliadzbz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.tianlin.xyz/gtsogzeyfy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xziqi.cn/gtojqlnqwa.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinghuilouyu.cn/gtndtvzjly.html

[L03] 设置自定义请求头
来源：http://hz.shanyushiyangkeji.top/gtsanamxfl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.shuidangran.top/gtqtkdzocq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.vqdsnc.cn/gtnzhsfail.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tianlin.xyz/gtkonnbbzm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangshuangyany.cn/gtksgrbusv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.redwolf501.top/gtxgfkxaco.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.daxiang520.top/gtxanvaesl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hysaishi.cn/gtfjnsfqon.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yangfankeji.com/gtfozzfcip.html

[L04] 设置超时
来源：http://hz.xziqi.cn/gtixufthaw.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shanyushiyangtech.top/gtvwvcpvwy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sxryk.cn/gtuocjxgvc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shzxlz.cn/gtctbsohjx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gzhubu.top/gtjqkmzgec.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hongshengwenyu.top/gtmrpsheyx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.andypj.xyz/gteltiooxw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.wangdashe.top/gtczqksyxn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hnqzz.top/gthrwsoipw.html

[L05] 上传文件（multipart）
来源：http://hz.gotoacloud.top/gtamctdngv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.snrcjt.cn/gtbsjmimws.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shzxlz.cn/gtzigiokjn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zycfv.cn/gtzlymfsdm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xuetiantiany.cn/gtgaupenbd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xuetiantiany.cn/gtfhkgqkfa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hysaishi.cn/gtqzqmahwq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.wangdashe.top/gthsshkcaw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.aibaodan.cn/gtxxmubjbc.html

[L06] 解析响应为 JSON
来源：http://hz.jianghu66.top/gtzmjwycqr.html

Py:   resp.json()
来源：http://hz.gogol.net.cn/gtcqkifnyv.html

PHP:  json_decode($body, true);
来源：http://hz.gogol.net.cn/gtwpozvymb.html

JS:   await resp.json()
来源：http://hz.haohaochexian.top/gtsjtmfthw.html

TS:   await resp.json()
来源：http://hz.jlsjyb.cn/gtdawjhgaa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hnqzz.top/gtkhggiddj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yuxming.cn/gtwodtxoaf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zycfv.cn/gtxskztufa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hfpthk.cn/gtsemdxzuh.html

[L07] 处理 HTTP 状态码
来源：http://hz.ppjwa.cn/gtlritcfdb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.tian-w.cn/gtsdaxqnzy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.iojbl.cn/gtnwklrybw.html

JS:   resp.ok;  resp.status
来源：http://hz.aizwys.cn/gtpjgiohkp.html

TS:   resp.ok;  resp.status
来源：http://hz.zhaomingkeji.xyz/gtaplsfqxr.html

Java: resp.statusCode()
来源：http://hz.shzxlz.cn/gtdawcnwzz.html

Go:   resp.StatusCode
来源：http://hz.nwbrower.top/gtrrriacvs.html

Ruby: resp.code.to_i
来源：http://hz.haohaochexian.top/gtmplnzrzk.html

C#:   (int)resp.StatusCode
来源：http://hz.jiagoushi.top/gtrakzzwta.html

[L08] 并发请求多个地址
来源：http://hz.shangyingyoupin.top/gtfalicvwt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinyuanbaomall.cn/gtlkipccmz.html

PHP:  curl_multi_init() 系列
来源：http://hz.yongpay.top/gtvfpfsjwn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yanxiufei.cn/gtiumobwht.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.kuanghao11.cn/gttpuhpsqg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hongshengwenyu.top/gtfgnurzpu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yuanzhike.top/gtxfcstkya.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zdqjudy.top/gtxzdzphrt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.nwbrower.top/gtmsphhsnc.html

================================================================================
来源：http://hz.shzxlz.cn/gtptxmcgra.html

M. 命令行 / 进程 / 环境
来源：http://hz.jinyuanbaomall.cn/gtbabwzkyg.html

================================================================================
来源：http://hz.shzxlz.cn/gtpfktxglb.html

[M01] 读取命令行参数
来源：http://hz.pycfn.com/gtgwgacprx.html

Py:   sys.argv[1:]
来源：http://hz.zhijiandao.cn/gteughlcnz.html

PHP:  $argv;  $argc;
来源：http://hz.yueranfly.top/gtgwmmajta.html

JS:   process.argv.slice(2)
来源：http://hz.sufxvd.cn/gtfnghmvxc.html

TS:   process.argv.slice(2)
来源：http://hz.sysykeji.top/gtvgzkywun.html

Java: args 数组（main 方法参数）
来源：http://hz.ydzc1.top/gtcsxoinky.html

Go:   os.Args[1:]
来源：http://hz.sysykeji.top/gtgyrglkxj.html

Ruby: ARGV
来源：http://hz.ivvv.top/gtketjddtl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ybcxt.top/gtkbclcvcx.html

[M02] 读取环境变量
来源：http://hz.havefunace.top/gtylnzwder.html

Py:   os.environ.get("HOME")
来源：http://hz.yj20258888.top/gtlhrsranz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yueranfly.top/gtxnyfvzis.html

JS:   process.env.HOME
来源：http://hz.sxryk.cn/gtxmrhbbfs.html

TS:   process.env.HOME
来源：http://hz.yuxming.cn/gtsxtxhpfa.html

Java: System.getenv("HOME")
来源：http://hz.jyoumei.cn/gtdujcwomw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cheryme.top/gtephbpqag.html

Ruby: ENV["HOME"]
来源：http://hz.snrcjt.cn/gtegjozlkd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinyuanbaomall.cn/gtfcycxpxg.html

[M03] 执行外部命令
来源：http://hz.feifeiyinyue.top/gtndyxzqkg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuanzhike.top/gtdymacpkh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.meibo888.top/gtszqtdtlq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xylfe.cn/gtwokorakk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.bjfxy.top/gtmeqeftby.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ybcxt.top/gtyptoyiqp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sufxvd.cn/gttqawedkc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ybcxt.top/gtvfioxlcj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.kuanghao11.cn/gtwbtkbhot.html

[M04] 获取当前工作目录
来源：http://hz.zycfv.cn/gtrmtcutoz.html

Py:   os.getcwd()
来源：http://hz.wangshuangyany.cn/gtyklkpirf.html

PHP:  getcwd();
来源：http://hz.gotoacloud.top/gtvsyspxfo.html

JS:   process.cwd()
来源：http://hz.hammf.cn/gtdqdsstsl.html

TS:   process.cwd()
来源：http://hz.xingfuxueyuan.xyz/gtbnmkimmo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.haohaochexian.top/gtiwvkrfgx.html

Go:   os.Getwd()
来源：http://hz.zhengqikj.top/gthtbcamkn.html

Ruby: Dir.pwd
来源：http://hz.havefunace.top/gtdcksjdwd.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ehwqpu.com/gtdihdytfx.html

[M05] 设置退出码
来源：http://hz.hfpthk.cn/gtdcohzhxg.html

Py:   sys.exit(1)
来源：http://hz.yanxiufei.cn/gtluuomibl.html

PHP:  exit(1);
来源：http://hz.ppjwa.cn/gthjxdfhaf.html

JS:   process.exit(1)
来源：http://hz.havefunace.top/gtfcujitlb.html

TS:   process.exit(1)
来源：http://hz.yongpay.top/gtsudxllur.html

Java: System.exit(1)
来源：http://hz.ydjk.org.cn/gtzjcokyrh.html

Go:   os.Exit(1)
来源：http://hz.smart0.xyz/gtpvivtrdj.html

Ruby: exit 1
来源：http://hz.zdqjudy.top/gtkhwamtvu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.tianlin.xyz/gtixbrasbu.html

[M06] 向标准错误输出
来源：http://hz.ybcxt.top/gtykvjbtko.html

Py:   print("err", file=sys.stderr)
来源：http://hz.redwolf501.top/gtltecdmhu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.daria6918.cn/gtlckzgyaj.html

JS:   console.error("err")
来源：http://hz.jinyuanbaomall.cn/gtcbptkkxt.html

TS:   console.error("err")
来源：http://hz.snrcjt.cn/gtxozkfswi.html

Java: System.err.println("err")
来源：http://hz.9152youxi.cn/gtsxzihyql.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.snrcjt.cn/gtuparucwh.html

Ruby: warn "err"
来源：http://hz.fengsongda.top/gtkakxzhbz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jinqigufen.top/gtrygrdzab.html

[M07] 判断是否为主入口
来源：http://hz.ydzc1.top/gtbyuvyskp.html

Py:   if __name__ == "__main__":
来源：http://hz.xziqi.cn/gtyhdypsjr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shuidangran.top/gttqbmaswu.html

JS:   require.main === module
来源：http://hz.0kj1m.cn/gtakvyjqsb.html

TS:   require.main === module
来源：http://hz.pycfn.com/gtswioecxb.html

Java: public static void main(String[] args)
来源：http://hz.zhongyouzk.top/gtzqyfvllp.html

Go:   func main()
来源：http://hz.gzhubu.top/gttvbhxjds.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.quarkkingdee.top/gtcbwcgtar.html

C#:   static void Main(string[] args)
来源：http://hz.bjfxy.top/gtxdweqauc.html

[M08] 获取系统与运行时信息
来源：http://hz.jinqigfzy.top/gtbqhytldt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shuidangran.top/gtsmnexyaa.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.guannengcc.top/gttpudqhac.html

JS:   process.platform;  process.version
来源：http://hz.cashguo.top/gtlhqepquw.html

TS:   process.platform;  process.version
来源：http://hz.xinyue.icu/gtugnzggou.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xziqi.cn/gtcmcdrgof.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ybcxt.top/gthibxxzvu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.bjfxy.top/gthauvyjrp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.nanxinkj.top/gtaramoary.html

================================================================================
来源：http://hz.hnqzz.top/gtkmpqpozb.html

N. 数据结构与算法
来源：http://hz.daria6918.cn/gtgvzbfmrh.html

================================================================================
来源：http://hz.sxryk.cn/gtnaebffki.html

[N01] 二分查找（有序数组）
来源：http://hz.birdmap.top/gtjzqlpkkz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jyoumei.cn/gtlqkafwyl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yanxiufei.cn/gtxgzvijqd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dashuyun.cn/gtrvqetnnq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aizwys.cn/gtplnfzbal.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.mhx1999.top/gtvwjxkqex.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinghuilouyu.cn/gtldtlbxte.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.cashguo.top/gtcvtcjhtb.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sxryk.cn/gtsdyoqikc.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yanxiufei.cn/gtnrvcopkr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hfpthk.cn/gtjrgtfpev.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yongpay.top/gtujwqbany.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.redwolf501.top/gtjfxgpglp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.dashuyun.cn/gtqqmlgxvs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xuetiantiany.cn/gtqfzwkxyw.html

Go:   slices.Sort(arr)
来源：http://hz.fzhhl.top/gthrgcexap.html

Ruby: arr.sort
来源：http://hz.yj20258.top/gtqwjjinqx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cucudq.cn/gtxblwsxsp.html

[N03] 快速排序（分治示例）
来源：http://hz.hfpthk.cn/gtozoxmccu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ybcxt.top/gtldbbbxlr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.haohaochexian.top/gtelfrvauu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xylfe.cn/gtfbzrlegi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.iojbl.cn/gteuafrxqu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xingfuxueyuan.xyz/gteirwzrvk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shanyushiyangtech.top/gtsqrltmxm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yj20258888.top/gtzpudfngt.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.chenlongwang.top/gtcqgpfzsu.html

[N04] 斐波那契数列
来源：http://hz.iojbl.cn/gtezbbnjeq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangkeji.top/gtgudbjaru.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jiagoushi.top/gtfixdbiox.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xingfuxueyuan.xyz/gtotonpczl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xinyue.icu/gtroldzfwj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yuxming.cn/gtralszuju.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hammf.cn/gtchkbhuvl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhiwuduotai.top/gtydudkifi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhengqikj.top/gtbjbuwhyh.html

[N05] 最大公约数
来源：http://hz.haohaochexian.top/gthogyrxsb.html

Py:   math.gcd(a, b)
来源：http://hz.nanxuanxn.top/gtnkeyneam.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.52xcode.cn/gtouzhbowo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nanxinkj.top/gtiexqibbz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pengpengdd.cyou/gtdajrajsf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jinqigufen.top/gtqahaiudr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinyuanbaomall.cn/gtcehenxmk.html

Ruby: a.gcd(b)
来源：http://hz.9152youxi.cn/gtymlobgmg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.aizwys.cn/gtrrigvkem.html

[N06] 判断回文字符串
来源：http://hz.birdmap.top/gtioaqjohm.html

Py:   s == s[::-1]
来源：http://hz.zhengqikj.top/gtygpglidr.html

PHP:  $s === strrev($s);
来源：http://hz.xinyue.icu/gtoghphszg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.feifeiyinyue.top/gthjhrzwfx.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtlgvasjmn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhongyouzk.top/gtliybupml.html

Go:   // 双指针从两端比较
来源：http://hz.cashguo.top/gtsewafhhz.html

Ruby: s == s.reverse
来源：http://hz.chenjidiqi.icu/gtmkanxmin.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.chenlongwang.top/gtnosrxdxh.html

[N07] 两数之和（返回下标）
来源：http://hz.9152youxi.cn/gtuolcbcos.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.mhx1999.top/gtdetevcap.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shuidangran.top/gtrsyytrfm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.pengpengdd.cyou/gtxwgzinyp.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinqigfzy.top/gtzzosvvzp.html

Java: // 手写 HashMap
来源：http://hz.hnxiangtu.top/gtmjhqefat.html

Go:   // 手写 map[int]int
来源：http://hz.tian-w.cn/gtxxzfnfig.html

Ruby: // 手写 Hash
来源：http://hz.c1oappe.top/gtwnnnzuaf.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ydzc1.top/gtglgtzkss.html

[N08] 生成全排列
来源：http://hz.havefunace.top/gtjwuguhay.html

Py:   itertools.permutations(arr)
来源：http://hz.zhaomingkeji.xyz/gtfkbvskib.html

PHP:  // 手写递归交换
来源：http://hz.jiagoushi.top/gtxaptsfhl.html

JS:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtredvhrep.html

TS:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtjujodzgs.html

Java: // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gteusrvmkl.html

Go:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtfrmblxep.html

Ruby: arr.permutation.to_a
来源：http://hz.gotoacloud.top/gtkayyaeeg.html

C#:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtbxadpgfw.html

[N09] 栈与队列
来源：http://hz.xylfe.cn/gtphazagqc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.aizwys.cn/gtosibeojl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.wangshuangyany.cn/gtwbeoifha.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.bjfxy.top/gtppafkixb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.daria6918.cn/gtqonqsxoe.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ydjk.org.cn/gtzhkxlujl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.9152youxi.cn/gtkprlhxmh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yj20258.top/gtchszouzx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yanxiufei.cn/gtszyzjhnn.html

[N10] 链表节点定义
来源：http://hz.cheryme.top/gtezmvasfz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.9152youxi.cn/gtquilihmw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xuetiantiany.cn/gtchrbtkdj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.tianlin.xyz/gtgdfotcno.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.pycfn.com/gtczauebmo.html

Java: class Node { int v; Node next; }
来源：http://hz.snrcjt.cn/gtcfhumafp.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yj20258.top/gtvarzhglc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhijiandao.cn/gthbtqcurp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hongshengwenyu.top/gtrdlzcmre.html

[N11] 二叉树中序遍历
来源：http://hz.ppjwa.cn/gtqlaersrk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.pycfn.com/gtcnnshgqv.html

PHP:  // 手写递归函数
来源：http://hz.zhoulong.xyz/gthmryrsjr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.daria6918.cn/gtuszbdwnb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sxryk.cn/gtzydnvfxf.html

Java: // 手写递归
来源：http://hz.0kj1m.cn/gttszyogzn.html

Go:   // 手写递归
来源：http://hz.dianchejie.cn/gtazpwiawa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.meibo888.top/gtntmobrnp.html

C#:   // 手写递归
来源：http://hz.haohaochexian.top/gtjjtnknxk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.dianchejie.cn/gtpzhqsigb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.mhx1999.top/gthdiysptm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.dianchejie.cn/gtlfekmzdr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhengqikj.top/gtiqnwnnxq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sweek.top/gtsspvalvf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhaomingkeji.xyz/gtkjrhtyba.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.gotoacloud.top/gthihcdfeh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.fzhhl.top/gtitgojnwj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gogol.net.cn/gtkqitkvdc.html

================================================================================
来源：http://hz.zhoulong.xyz/gtjliomsoi.html

O. 并发与异步
来源：http://hz.yvedp.cn/gtphdjpwxu.html

================================================================================
来源：http://hz.jianghu66.top/gtszqeufol.html

[O01] 启动一个线程
来源：http://hz.0kj1m.cn/gtfrwkgfoa.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yuanzhike.top/gtitdyvymi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ybcxt.top/gtxgchkgdc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jinqigfzy.top/gtdgjoddam.html

TS:   // 同 JS
来源：http://hz.sufxvd.cn/gtarxubasw.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhijiandao.cn/gtghugzvcq.html

Go:   go f()
来源：http://hz.gotoacloud.top/gtobrpqklz.html

Ruby: Thread.new { f }
来源：http://hz.yj20258.top/gtwllzxvdy.html

C#:   Task.Run(() => F());
来源：http://hz.gotoacloud.top/gtzkbuuozb.html

[O02] 使用线程池
来源：http://hz.9152youxi.cn/gtmgzjzlla.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yj20258888.top/gtlubowtzw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhongyouzk.top/gtkvbmxszl.html

JS:   // worker_threads 线程池
来源：http://hz.quarkkingdee.top/gtvmlubcsq.html

TS:   // worker_threads 线程池
来源：http://hz.gotoacloud.top/gtwjlqifhy.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.9152youxi.cn/gtzgwqfsdi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cashguo.top/gtquboqnwl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.guannengcc.top/gtyqlxldmo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.c1oappe.top/gtxisexpqk.html

[O03] 加锁保护共享数据
来源：http://hz.iojbl.cn/gthxlgblph.html

Py:   with lock: shared += 1
来源：http://hz.jianghu66.top/gtdikbfmpr.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.redwolf501.top/gtuakeorhq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hywenlv.cn/gtvsyuzpij.html

TS:   // 同 JS
来源：http://hz.haohaochexian.top/gtcggdhmzn.html

Java: synchronized (this) { shared++; }
来源：http://hz.9152youxi.cn/gtjoopzgjp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yj20258.top/gtzltqwqxx.html


<!-- 参考信息 -->