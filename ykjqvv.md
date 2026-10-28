代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.birdmap.top/gtxflhlsav.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cucudq.cn/gtkwpwfwug.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shangyingyoupin.top/gtgbsxvhrh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xingfuxueyuan.xyz/gtebwlefkv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.wangshuangyany.cn/gtkoztphsv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.feifeiyinyue.top/gtothfmuci.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinqigufen.top/gtuqhwrqmx.html

Py:   pickle.dumps(obj)
来源：http://hz.xylfe.cn/gtezgfmuua.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zycfv.cn/gtatjovsdh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenjidiqi.icu/gtshxtrigl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hfpthk.cn/gtvzgtllyr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jianghu66.top/gtcejphgzh.html

Go:   encoding/gob
来源：http://hz.zdqjudy.top/gtzbrbttsf.html

Ruby: Marshal.dump(obj)
来源：http://hz.xziqi.cn/gtsazubabw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xziqi.cn/gtjczsntdi.html

================================================================================
来源：http://hz.bjfxy.top/gtkdgakvmx.html

L. 网络请求
来源：http://hz.yj20258.top/gtaisrrcth.html

================================================================================
来源：http://hz.quarkkingdee.top/gtsmpyknfe.html

[L01] 发送 GET 请求
来源：http://hz.hywenlv.cn/gtgyxypors.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jyoumei.cn/gtviylftyz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jyoumei.cn/gtvkqwayvv.html

JS:   await fetch(url)
来源：http://hz.guannengcc.top/gtlnlwgoxi.html

TS:   await fetch(url)
来源：http://hz.nanxuanxn.top/gtoupmmeah.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhongyouzk.top/gthdxxzqro.html

Go:   resp, err := http.Get(url)
来源：http://hz.pycfn.com/gtooukriok.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cashguo.top/gtvivqcpqz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinqigfzy.top/gtoepqtqqj.html

[L02] 发送 POST JSON
来源：http://hz.shangyingyoupin.top/gtixnbskfg.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yj202588.top/gtgdptxrhi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhongyouzk.top/gtbkshumlz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.snrcjt.cn/gtaoygvkuo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258888.top/gtszrpllea.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.quarkkingdee.top/gtibhztefv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhiwuduotai.top/gtzdjzlcgl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhengqikj.top/gthdempmgo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ydjk.org.cn/gttoanohkj.html

[L03] 设置自定义请求头
来源：http://hz.shanyushiyangtech.top/gtinxqznlb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhiwuduotai.top/gttuvrnkag.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sysykeji.top/gtkfnvpeba.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jiagoushi.top/gtvuidimor.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cqqwz.cn/gtasijklmu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.pycfn.com/gtjgbcvfbi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.guannengcc.top/gtujxvwcpq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hysaishi.cn/gtihuardyi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.haohaochexian.top/gtbiyufjrq.html

[L04] 设置超时
来源：http://hz.tian-w.cn/gtdhpcwowi.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shuidangran.top/gtoqpvsqul.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ivvv.top/gtdvathcui.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhixingplan.top/gtkdeotabv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fengsongda.top/gtyztziwti.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yangfankeji.com/gtganvmaay.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.feifeiyinyue.top/gtkesyexqv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zycfv.cn/gtroxngawv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhixingplan.top/gtdjufclvk.html

[L05] 上传文件（multipart）
来源：http://hz.shzxlz.cn/gtdctytzpa.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hongshengwenyu.top/gtbzefimvq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.aibaodan.cn/gtnuczmrvz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258.top/gtmnfybady.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.0kj1m.cn/gtgnjpsbdz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ybcxt.top/gtnrjtlaml.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shangyingyoupin.top/gtlabnnkcq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xziqi.cn/gttvbmxntf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.haohaochexian.top/gtjyrydapx.html

[L06] 解析响应为 JSON
来源：http://hz.xuanzx.com/gtnxfswmqq.html

Py:   resp.json()
来源：http://hz.ydjk.org.cn/gtspkjawbe.html

PHP:  json_decode($body, true);
来源：http://hz.hfpthk.cn/gtpmttqcjh.html

JS:   await resp.json()
来源：http://hz.vqdsnc.cn/gteyxkjgmv.html

TS:   await resp.json()
来源：http://hz.ydjk.org.cn/gtblqgyskw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hnqzz.top/gthbjfkqss.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhixingplan.top/gtticjadda.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gogol.net.cn/gtyppuethc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.haohaochexian.top/gtjvchvqei.html

[L07] 处理 HTTP 状态码
来源：http://hz.chenlongwang.top/gtczzfcjfx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.meibo888.top/gtmvhqantg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cheryme.top/gttycgvdjd.html

JS:   resp.ok;  resp.status
来源：http://hz.vqdsnc.cn/gtvwnhgqdw.html

TS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangtech.top/gtjssjmvuj.html

Java: resp.statusCode()
来源：http://hz.haohaochexian.top/gtchganffb.html

Go:   resp.StatusCode
来源：http://hz.shangyingyoupin.top/gtyixfacxl.html

Ruby: resp.code.to_i
来源：http://hz.vqdsnc.cn/gtltgxbklw.html

C#:   (int)resp.StatusCode
来源：http://hz.zhongyouzk.top/gtbjmdvbqq.html

[L08] 并发请求多个地址
来源：http://hz.cashguo.top/gtyqyzubvt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hammf.cn/gtwadkgwut.html

PHP:  curl_multi_init() 系列
来源：http://hz.ppjwa.cn/gtqpsshhhf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgufenzy.top/gttgsbksdh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gotoacloud.top/gtikoylvuu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.c1oappe.top/gtyrzdjzxe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinqigufen.top/gtqogpfggq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.0kj1m.cn/gtloicatcy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gotoacloud.top/gttcwfzemr.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtbzspltvc.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhoulong.xyz/gtmuvhqpbx.html

================================================================================
来源：http://hz.pycfn.com/gtinmjgbdj.html

[M01] 读取命令行参数
来源：http://hz.gotoacloud.top/gtfbdnbmbn.html

Py:   sys.argv[1:]
来源：http://hz.yuanzhike.top/gtxjvstsgs.html

PHP:  $argv;  $argc;
来源：http://hz.aibaodan.cn/gtnvrjfctp.html

JS:   process.argv.slice(2)
来源：http://hz.xuanzx.com/gtwotqdfam.html

TS:   process.argv.slice(2)
来源：http://hz.cdnleiting.top/gtokrhvpuj.html

Java: args 数组（main 方法参数）
来源：http://hz.hfpthk.cn/gtuwmtfwaw.html

Go:   os.Args[1:]
来源：http://hz.andypj.xyz/gtnnqovqzv.html

Ruby: ARGV
来源：http://hz.zhengqikj.top/gtsfxrcxle.html

C#:   args 数组（Main 方法参数）
来源：http://hz.tian-w.cn/gtrkxjqrpc.html

[M02] 读取环境变量
来源：http://hz.hysaishi.cn/gtjerhdjqd.html

Py:   os.environ.get("HOME")
来源：http://hz.bjfxy.top/gtirlgxktl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hywenlv.cn/gtlwbhdisg.html

JS:   process.env.HOME
来源：http://hz.jinghuilouyu.cn/gtvsanubca.html

TS:   process.env.HOME
来源：http://hz.yj202588.top/gtkewhueas.html

Java: System.getenv("HOME")
来源：http://hz.iojbl.cn/gtwvxbgzly.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.kuanghao11.cn/gtlwqumukm.html

Ruby: ENV["HOME"]
来源：http://hz.cheryme.top/gtlajiylmc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.snrcjt.cn/gtyjpjfhjc.html

[M03] 执行外部命令
来源：http://hz.svipenyu.cn/gtydjvgbxn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hnqzz.top/gtbkheenms.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhiwuduotai.top/gtqyqnubds.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yonumen.top/gtzpuzmjje.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.daxiang520.top/gtpqwyykfj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.bjfxy.top/gtpsjkzcet.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.dianchejie.cn/gtvulrovre.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zycfv.cn/gtjwjydsyl.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shangyingyoupin.top/gtdczkgybj.html

[M04] 获取当前工作目录
来源：http://hz.yj20258888.top/gtmptpbcml.html

Py:   os.getcwd()
来源：http://hz.ppjwa.cn/gtbmcplfig.html

PHP:  getcwd();
来源：http://hz.jqgfzy.top/gtsnoyvdkz.html

JS:   process.cwd()
来源：http://hz.pycfn.com/gtwwwqjvuh.html

TS:   process.cwd()
来源：http://hz.iojbl.cn/gtpdhgnvoc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.mhx1999.top/gtgwvyakuq.html

Go:   os.Getwd()
来源：http://hz.jqgufenzy.top/gtokssnqez.html

Ruby: Dir.pwd
来源：http://hz.9152youxi.cn/gtfcfloiss.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.kuanghao11.cn/gtmliqrthx.html

[M05] 设置退出码
来源：http://hz.yj202588.top/gtvalkywra.html

Py:   sys.exit(1)
来源：http://hz.yj20258888.top/gtrnxsslqv.html

PHP:  exit(1);
来源：http://hz.hnqzz.top/gthyxqyslk.html

JS:   process.exit(1)
来源：http://hz.haohaochexian.top/gtcbftnelv.html

TS:   process.exit(1)
来源：http://hz.havefunace.top/gtqcsjqilg.html

Java: System.exit(1)
来源：http://hz.ydzc1.top/gtsdvxshhj.html

Go:   os.Exit(1)
来源：http://hz.jinyuanbaomall.cn/gtcvrgoomu.html

Ruby: exit 1
来源：http://hz.wangdashe.top/gtiolmadqb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xuanzx.com/gtnlbtyxjv.html

[M06] 向标准错误输出
来源：http://hz.feifeiyinyue.top/gtgawtiyja.html

Py:   print("err", file=sys.stderr)
来源：http://hz.smart0.xyz/gtfzufsiii.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yuanzhike.top/gtjkqzgbjw.html

JS:   console.error("err")
来源：http://hz.ehwqpu.com/gtgpordlxs.html

TS:   console.error("err")
来源：http://hz.hywenlv.cn/gtkltmydba.html

Java: System.err.println("err")
来源：http://hz.yongpay.top/gtquumekkb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gogol.net.cn/gtvahleyfi.html

Ruby: warn "err"
来源：http://hz.wangdashe.top/gthgstrokx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhijiandao.cn/gtjowywqnx.html

[M07] 判断是否为主入口
来源：http://hz.tianlin.xyz/gtzhyzgokf.html

Py:   if __name__ == "__main__":
来源：http://hz.yj20258888.top/gtwnpnbdmn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.mhx1999.top/gtrwrziuzp.html

JS:   require.main === module
来源：http://hz.cucudq.cn/gtffrdxfii.html

TS:   require.main === module
来源：http://hz.tian-w.cn/gtiaxjowlp.html

Java: public static void main(String[] args)
来源：http://hz.ydjk.org.cn/gtwrrmrcrj.html

Go:   func main()
来源：http://hz.zhoulong.xyz/gtwwxahkfe.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.andypj.xyz/gtkuohqdok.html

C#:   static void Main(string[] args)
来源：http://hz.tian-w.cn/gtqnzawceb.html

[M08] 获取系统与运行时信息
来源：http://hz.tian-w.cn/gtuvccbgcm.html

Py:   platform.system();  platform.python_version()
来源：http://hz.dashuyun.cn/gtczbobsip.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cqqwz.cn/gtmgwkqvea.html

JS:   process.platform;  process.version
来源：http://hz.jianghu66.top/gtvfsukftd.html

TS:   process.platform;  process.version
来源：http://hz.fengsongda.top/gtozoxvuvo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hysaishi.cn/gttlfrjqfb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sufxvd.cn/gtztiiazeg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hywenlv.cn/gtyutlhrqz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.chenjidiqi.icu/gtglyyzpns.html

================================================================================
来源：http://hz.tian-w.cn/gtxpvqktep.html

N. 数据结构与算法
来源：http://hz.tianlin.xyz/gtuzkjqxbj.html

================================================================================
来源：http://hz.52xcode.cn/gtleyuncaj.html

[N01] 二分查找（有序数组）
来源：http://hz.ydzc1.top/gtbkaunuth.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xylfe.cn/gthsnkknkq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ydjk.org.cn/gtvqvaxnvu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhongyouzk.top/gteyzckosw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinyuanbaomall.cn/gtyaxnqaum.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yanxiufei.cn/gtxnzffrnz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhijiandao.cn/gteqvzpedh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jlsjyb.cn/gteuoedonc.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jiagoushi.top/gthvkekwvl.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.52xcode.cn/gtuffzwngo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigufen.top/gtzjnqpbkz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.fengsongda.top/gtentoqjbm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxinkj.top/gtnxyjwvbo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinyuanbaomall.cn/gtvrozheti.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jqgufenzy.top/gtfnbnzvig.html

Go:   slices.Sort(arr)
来源：http://hz.wangshuangyany.cn/gtpeajwvie.html

Ruby: arr.sort
来源：http://hz.redwolf501.top/gtjyhrfbko.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ydzc1.top/gtibqjljib.html

[N03] 快速排序（分治示例）
来源：http://hz.316326.xyz/gtzzreutpk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yj202588.top/gtziktazxv.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ywan-chungtsiang.top/gtkytlwybn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dianchejie.cn/gtgxoczewv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yonumen.top/gtdredxabu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jiagoushi.top/gticudykvo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yangfankeji.com/gtpuxggyow.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenzaomai.com/gtefxnexgc.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hysaishi.cn/gtgyvevezk.html

[N04] 斐波那契数列
来源：http://hz.jinqigfzy.top/gtlrfvljna.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yangfankeji.com/gtbfuesfdo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.gogol.net.cn/gtockaxaor.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jqgufenzy.top/gtstriupvs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.birdmap.top/gtrdxbegxk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sweek.top/gthydrmsho.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhoulong.xyz/gtqoyhlsfg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hysaishi.cn/gtwuozctzb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.dianchejie.cn/gtivsinswu.html

[N05] 最大公约数
来源：http://hz.chenzaomai.com/gtubjpmrvr.html

Py:   math.gcd(a, b)
来源：http://hz.wangshuangyany.cn/gtacysixzu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zdqjudy.top/gtnplgtyka.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydzc1.top/gtqdbwygsy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.meibo888.top/gtwdvbtqtn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yuanzhike.top/gtkasqctwj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.bjfxy.top/gtzuxsnklt.html

Ruby: a.gcd(b)
来源：http://hz.chenlongwang.top/gtuapzufcn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shzxlz.cn/gtdyqrdgtc.html

[N06] 判断回文字符串
来源：http://hz.yj20258.top/gtfkuxsotg.html

Py:   s == s[::-1]
来源：http://hz.sufxvd.cn/gtgmsjhala.html

PHP:  $s === strrev($s);
来源：http://hz.jinqigufen.top/gtdripzgze.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtiacqcxfr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ybcxt.top/gtuhzricjf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.mhx1999.top/gtwgjzrnus.html

Go:   // 双指针从两端比较
来源：http://hz.nwbrower.top/gttepeenmb.html

Ruby: s == s.reverse
来源：http://hz.andypj.xyz/gtwsktarwo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cqqwz.cn/gtdxgrtafp.html

[N07] 两数之和（返回下标）
来源：http://hz.havefunace.top/gtznwssyyq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.aibaodan.cn/gtjyszqxdb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ywan-chungtsiang.top/gtpiixapat.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ywan-chungtsiang.top/gtsiukvpgp.html

TS:   // 手写 Map<string, number>
来源：http://hz.andypj.xyz/gtnexdlqcl.html

Java: // 手写 HashMap
来源：http://hz.jyoumei.cn/gtthnjeedn.html

Go:   // 手写 map[int]int
来源：http://hz.yonumen.top/gtjvcxyatq.html

Ruby: // 手写 Hash
来源：http://hz.hnxiangtu.top/gtmazbmnnh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shanyushiyangtech.top/gtjmxppzgy.html

[N08] 生成全排列
来源：http://hz.shuidangran.top/gtxddicnwu.html

Py:   itertools.permutations(arr)
来源：http://hz.0kj1m.cn/gtvpatbpvk.html

PHP:  // 手写递归交换
来源：http://hz.hnqzz.top/gtzwkomwaz.html

JS:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtjcoeokjw.html

TS:   // 手写回溯递归
来源：http://hz.wangdashe.top/gtmvowbrgq.html

Java: // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtmkmoupmd.html

Go:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtknwolrsw.html

Ruby: arr.permutation.to_a
来源：http://hz.jiagoushi.top/gtqblgdxto.html

C#:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtkxhsybrc.html

[N09] 栈与队列
来源：http://hz.redwolf501.top/gtkmsuzapw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shuidangran.top/gtbclhegkc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.aibaodan.cn/gtxpvgydcp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yvedp.cn/gtjpjiogqv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jianghu66.top/gtvsymldqk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhixingplan.top/gtcfgymrot.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cqqwz.cn/gtmlfsrtdn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.c1oappe.top/gtczmlhkiq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.chenjidiqi.icu/gtmivbycew.html

[N10] 链表节点定义
来源：http://hz.aibaodan.cn/gtmwcbnory.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.52xcode.cn/gtqlvubmsx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shangyingyoupin.top/gttwixsoyq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.bjfxy.top/gtnpzlykfj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tian-w.cn/gtghsfngpx.html

Java: class Node { int v; Node next; }
来源：http://hz.hysaishi.cn/gtrxtxcdnq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xinyue.icu/gtwwesxayi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yvedp.cn/gtckllbhlg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.andypj.xyz/gtxeaynbcf.html

[N11] 二叉树中序遍历
来源：http://hz.jqgufenzy.top/gtaomndnnn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hysaishi.cn/gtkznrvyyj.html

PHP:  // 手写递归函数
来源：http://hz.yonumen.top/gtfpmntbuf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenlongwang.top/gtxjzbzshn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cqqwz.cn/gtawhkatfc.html

Java: // 手写递归
来源：http://hz.tanke756.top/gteticfbbc.html

Go:   // 手写递归
来源：http://hz.nwbrower.top/gtbqssuhcd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xinyue.icu/gtosmnylpf.html

C#:   // 手写递归
来源：http://hz.iojbl.cn/gtxfjaoqot.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xinyue.icu/gtnmxdgwph.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ybcxt.top/gtbwerfhzw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yanxiufei.cn/gtbhknweit.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhiwuduotai.top/gtavizdgyr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gotoacloud.top/gthusyogmx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinghuilouyu.cn/gttlipysnv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.daria6918.cn/gtexntkgzf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hammf.cn/gtpdaixkqf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shzxlz.cn/gtfcktgisn.html

================================================================================
来源：http://hz.meibo888.top/gtmqolkdyk.html

O. 并发与异步
来源：http://hz.ehwqpu.com/gtnaosacuh.html

================================================================================
来源：http://hz.vqdsnc.cn/gtmmpcyqif.html

[O01] 启动一个线程
来源：http://hz.iojbl.cn/gtzcbevjjh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shzxlz.cn/gtugcrmsuu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xuetiantiany.cn/gtnfmjnbnz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.shanyushiyangkeji.top/gtkuwonxsp.html

TS:   // 同 JS
来源：http://hz.daria6918.cn/gthoquuytz.html

Java: new Thread(() -> f()).start()
来源：http://hz.haohaochexian.top/gtkspqtnxn.html

Go:   go f()
来源：http://hz.sxryk.cn/gtomxdhxlg.html

Ruby: Thread.new { f }
来源：http://hz.daria6918.cn/gtalyxpodl.html

C#:   Task.Run(() => F());
来源：http://hz.xuetiantiany.cn/gtoabocaaf.html

[O02] 使用线程池
来源：http://hz.ydjk.org.cn/gtykquwqge.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xylfe.cn/gtignnnvbz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.quarkkingdee.top/gtzbvsubas.html

JS:   // worker_threads 线程池
来源：http://hz.xuanzx.com/gtrozpyufv.html

TS:   // worker_threads 线程池
来源：http://hz.chenlongwang.top/gthlryfklg.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cdnleiting.top/gtgebqkccj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hywenlv.cn/gtzdqmejit.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ppjwa.cn/gtrlyoxstw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yj202588.top/gtabivbrry.html

[O03] 加锁保护共享数据
来源：http://hz.jlsjyb.cn/gtzisvrphy.html

Py:   with lock: shared += 1
来源：http://hz.dianchejie.cn/gtnoenfivc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.gaohongyu789.top/gtddrmcejr.html


<!-- 参考信息 -->