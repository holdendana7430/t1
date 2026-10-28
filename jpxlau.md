代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tanke756.top/gtayspxhcp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yuxming.cn/gteregfftk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gtxbusjtqy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yvedp.cn/gtrhxafocy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.c1oappe.top/gtdpksakee.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hnxiangtu.top/gtdszbyjee.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cashguo.top/gtlvheywwj.html

Py:   pickle.dumps(obj)
来源：http://hz.ydjk.org.cn/gtepnsbtep.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.pycfn.com/gtyajaywju.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinqigufen.top/gtnvrbaqhz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhijiandao.cn/gtzcnmbndc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yangfankeji.com/gtrkztqcjd.html

Go:   encoding/gob
来源：http://hz.aibaodan.cn/gtjmysajby.html

Ruby: Marshal.dump(obj)
来源：http://hz.nanxuanxn.top/gtsahrcfqm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.316326.xyz/gtgafhonou.html

================================================================================
来源：http://hz.c1oappe.top/gtuwmiedck.html

L. 网络请求
来源：http://hz.ywan-chungtsiang.top/gtxuhmfywu.html

================================================================================
来源：http://hz.fengsongda.top/gtfmvsnnit.html

[L01] 发送 GET 请求
来源：http://hz.hongshengwenyu.top/gtkyupgmie.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.daxiang520.top/gtexokkcyv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shangyingyoupin.top/gtsiabtbir.html

JS:   await fetch(url)
来源：http://hz.sysykeji.top/gtywezgbrx.html

TS:   await fetch(url)
来源：http://hz.jinyuanbaomall.cn/gtegpazgzj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hysaishi.cn/gtvgtjuwbu.html

Go:   resp, err := http.Get(url)
来源：http://hz.birdmap.top/gtldotvaal.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhixingplan.top/gtsklmhfyn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.snrcjt.cn/gtsrqhrbtq.html

[L02] 发送 POST JSON
来源：http://hz.xingfuxueyuan.xyz/gtoqtftnyh.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.birdmap.top/gtyhmmiafv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cheryme.top/gtrbujbyfn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guowangkeji.top/gtnukjzjci.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jlsjyb.cn/gtxgewvkxu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gogol.net.cn/gtpiyjvnqq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.pengpengdd.cyou/gtsvcgstfi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhengqikj.top/gtfpkmxtrn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.gaohongyu789.top/gtkjyvhznv.html

[L03] 设置自定义请求头
来源：http://hz.sxryk.cn/gtwixkqeyp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yuanzhike.top/gtbqmwmkpm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cashguo.top/gtrsjrunid.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenjidiqi.icu/gtahgvkesq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnqzz.top/gtujcbmhwa.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sxryk.cn/gtrzfylbcv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.quarkkingdee.top/gtsnvsdvhs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.pengpengdd.cyou/gtffjbcfdx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ehwqpu.com/gtokcysdyk.html

[L04] 设置超时
来源：http://hz.zhongyouzk.top/gtpljogutx.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cheryme.top/gtmhbraiso.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hnxiangtu.top/gtetptryra.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenzaomai.com/gtytoerriu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yvedp.cn/gtjkpxffvb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ywan-chungtsiang.top/gtdtuebxhq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj20258888.top/gtgqwvfagh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhijiandao.cn/gtpfkjjceh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.fengsongda.top/gtrvelgwhz.html

[L05] 上传文件（multipart）
来源：http://hz.aizwys.cn/gtcfqlzicg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yanxiufei.cn/gtimofmoel.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xuetiantiany.cn/gtmqzqbxnd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenjidiqi.icu/gtvizksblo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.birdmap.top/gtcafrzlqd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xinyue.icu/gtqfifgwhc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.daria6918.cn/gtjxezymzb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.wangshuangyany.cn/gtsfilxsoy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xuetiantiany.cn/gtgradknsp.html

[L06] 解析响应为 JSON
来源：http://hz.xingfuxueyuan.xyz/gttozunmuh.html

Py:   resp.json()
来源：http://hz.ybcxt.top/gtxyzfussu.html

PHP:  json_decode($body, true);
来源：http://hz.shanyushiyangkeji.top/gtdnhcppur.html

JS:   await resp.json()
来源：http://hz.jianghu66.top/gthubjnenp.html

TS:   await resp.json()
来源：http://hz.jyoumei.cn/gtnumrbkio.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gaohongyu789.top/gtmydpezhp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.quarkkingdee.top/gtralatwgs.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cheryme.top/gtthhfnqax.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jinqigfzy.top/gtjdgwtlqw.html

[L07] 处理 HTTP 状态码
来源：http://hz.cqqwz.cn/gtfxuqxizk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.dianchejie.cn/gtxrdawtaj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hnqzz.top/gtuxbrxbde.html

JS:   resp.ok;  resp.status
来源：http://hz.xinyue.icu/gtvvcpecoj.html

TS:   resp.ok;  resp.status
来源：http://hz.yuxming.cn/gtbmaarvkv.html

Java: resp.statusCode()
来源：http://hz.hongshengwenyu.top/gtvfnrjbew.html

Go:   resp.StatusCode
来源：http://hz.zdqjudy.top/gtvidpazfb.html

Ruby: resp.code.to_i
来源：http://hz.feifeiyinyue.top/gtyfoamxiq.html

C#:   (int)resp.StatusCode
来源：http://hz.hfpthk.cn/gtoajoafhj.html

[L08] 并发请求多个地址
来源：http://hz.ybcxt.top/gtctmpwycb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.chenlongwang.top/gtdwlsxjjb.html

PHP:  curl_multi_init() 系列
来源：http://hz.sxryk.cn/gtdkyqallq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.316326.xyz/gtprvnwvbq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.smart0.xyz/gtbimmnnqh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yuxming.cn/gtoqsjomkp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.9152youxi.cn/gtbhqsgycn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinghuilouyu.cn/gtjsxyqaln.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhiwuduotai.top/gtxheckasz.html

================================================================================
来源：http://hz.zhoulong.xyz/gtzpihfcya.html

M. 命令行 / 进程 / 环境
来源：http://hz.yj20258888.top/gtvxzoavxq.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtkiplccnt.html

[M01] 读取命令行参数
来源：http://hz.0kj1m.cn/gtluufoscm.html

Py:   sys.argv[1:]
来源：http://hz.jyoumei.cn/gtexgruksm.html

PHP:  $argv;  $argc;
来源：http://hz.tianlin.xyz/gtzigecfkx.html

JS:   process.argv.slice(2)
来源：http://hz.jinghuilouyu.cn/gtsseezkqh.html

TS:   process.argv.slice(2)
来源：http://hz.yangfankeji.com/gtkcvrpopk.html

Java: args 数组（main 方法参数）
来源：http://hz.hfpthk.cn/gtyycrsxpt.html

Go:   os.Args[1:]
来源：http://hz.svipenyu.cn/gthoijehim.html

Ruby: ARGV
来源：http://hz.hnqzz.top/gtswugxsyd.html

C#:   args 数组（Main 方法参数）
来源：http://hz.316326.xyz/gtnpumspat.html

[M02] 读取环境变量
来源：http://hz.jinyuanbaomall.cn/gtyxiaoswz.html

Py:   os.environ.get("HOME")
来源：http://hz.redwolf501.top/gtxpiyzwdn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.gaohongyu789.top/gtzgtxndbr.html

JS:   process.env.HOME
来源：http://hz.meibo888.top/gtfiutqtqx.html

TS:   process.env.HOME
来源：http://hz.nanxuanxn.top/gtrfkgwlwu.html

Java: System.getenv("HOME")
来源：http://hz.yonumen.top/gtxhscnmcp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yuxming.cn/gtikkwixph.html

Ruby: ENV["HOME"]
来源：http://hz.svipenyu.cn/gtbhtyureo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jqgfzy.top/gtyzxcsurp.html

[M03] 执行外部命令
来源：http://hz.bjfxy.top/gtkjdrcafh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ivvv.top/gtuhvytnju.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.dianchejie.cn/gtdkqvgxtn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jiagoushi.top/gtpsrvrgmh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.meibo888.top/gtpwdhwklk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.haohaochexian.top/gtyirycryy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ehwqpu.com/gteurkbyoq.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jqgufenzy.top/gttcjrycdz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yuanzhike.top/gtdpsyassm.html

[M04] 获取当前工作目录
来源：http://hz.chenjidiqi.icu/gtrezrzmjs.html

Py:   os.getcwd()
来源：http://hz.ehwqpu.com/gtaegvxkhv.html

PHP:  getcwd();
来源：http://hz.snrcjt.cn/gtcawntgcm.html

JS:   process.cwd()
来源：http://hz.andypj.xyz/gtrtiuosya.html

TS:   process.cwd()
来源：http://hz.aizwys.cn/gtzytbcbes.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cqqwz.cn/gtbbektzlf.html

Go:   os.Getwd()
来源：http://hz.316326.xyz/gtlwpvqudg.html

Ruby: Dir.pwd
来源：http://hz.ywan-chungtsiang.top/gtisfnmuiz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhixingplan.top/gtdqedfxed.html

[M05] 设置退出码
来源：http://hz.gzhubu.top/gtlkyydups.html

Py:   sys.exit(1)
来源：http://hz.yuanzhike.top/gtazyzxgjy.html

PHP:  exit(1);
来源：http://hz.xuetiantiany.cn/gtgwgbfotk.html

JS:   process.exit(1)
来源：http://hz.gzhubu.top/gtcpmatbio.html

TS:   process.exit(1)
来源：http://hz.aibaodan.cn/gtvoogiyrm.html

Java: System.exit(1)
来源：http://hz.yueranfly.top/gtelbtiwvs.html

Go:   os.Exit(1)
来源：http://hz.hfpthk.cn/gtlaovivnx.html

Ruby: exit 1
来源：http://hz.gogol.net.cn/gtecaipobu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhoulong.xyz/gtsxwziuxs.html

[M06] 向标准错误输出
来源：http://hz.zhixingplan.top/gtnbwlxruj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinyuanbaomall.cn/gtywrpivhy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.pengpengdd.cyou/gtvfmajzvg.html

JS:   console.error("err")
来源：http://hz.yongpay.top/gtcfynsian.html

TS:   console.error("err")
来源：http://hz.guannengcc.top/gtmtucwkim.html

Java: System.err.println("err")
来源：http://hz.birdmap.top/gtiepjcceb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sufxvd.cn/gtbyzdrawa.html

Ruby: warn "err"
来源：http://hz.xylfe.cn/gtgdmwpiqf.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.nanxuanxn.top/gtujidjlcl.html

[M07] 判断是否为主入口
来源：http://hz.316326.xyz/gtzjzwhlbs.html

Py:   if __name__ == "__main__":
来源：http://hz.fzhhl.top/gtlavwawqo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.pycfn.com/gtnmxbsehp.html

JS:   require.main === module
来源：http://hz.shuidangran.top/gtfzcsiruf.html

TS:   require.main === module
来源：http://hz.zhongyouzk.top/gtljhycwdu.html

Java: public static void main(String[] args)
来源：http://hz.xziqi.cn/gtqoedttsx.html

Go:   func main()
来源：http://hz.hnxiangtu.top/gtzrxqnqzf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ydzc1.top/gtzxaqmixh.html

C#:   static void Main(string[] args)
来源：http://hz.yuxming.cn/gtiolyiauz.html

[M08] 获取系统与运行时信息
来源：http://hz.9152youxi.cn/gtumfkyayk.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cashguo.top/gtttiwnpac.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ydzc1.top/gtntslmzsb.html

JS:   process.platform;  process.version
来源：http://hz.ppjwa.cn/gtnrcnfrst.html

TS:   process.platform;  process.version
来源：http://hz.haohaochexian.top/gtcdpkiovu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.wangdashe.top/gtfxvjnued.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hfpthk.cn/gtmblthlep.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.tanke756.top/gttfdtghbb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ppjwa.cn/gtsgsdeylf.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtjrlflabd.html

N. 数据结构与算法
来源：http://hz.jianghu66.top/gtozabctsp.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtnyahviwk.html

[N01] 二分查找（有序数组）
来源：http://hz.hnxiangtu.top/gtgplhnijm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.quarkkingdee.top/gthriswftq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.haohaochexian.top/gtcfxjpsmy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.feifeiyinyue.top/gtejgwahmw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhoulong.xyz/gtqrikgtib.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yj20258888.top/gtbxpqzvht.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jyoumei.cn/gtnsprhlja.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhoulong.xyz/gtvjajljar.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jiagoushi.top/gtzfmncxaw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhaomingkeji.xyz/gtfcdszepu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yanxiufei.cn/gtfnvpciqt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.guowangkeji.top/gtiqibtiuc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jiagoushi.top/gtlhgdeizw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.pengpengdd.cyou/gtekqhmdiw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.fzhhl.top/gtykrmgevz.html

Go:   slices.Sort(arr)
来源：http://hz.kuanghao11.cn/gtgwenehen.html

Ruby: arr.sort
来源：http://hz.yuanzhike.top/gtxeyxkbun.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.dashuyun.cn/gtfacybeti.html

[N03] 快速排序（分治示例）
来源：http://hz.gzhubu.top/gtrupuyzti.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yueranfly.top/gtavkvgqte.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jiagoushi.top/gttslriwnc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.feifeiyinyue.top/gtcxvmtrky.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aibaodan.cn/gtgolixsah.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.birdmap.top/gtxxalymep.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.pengpengdd.cyou/gtgyepucgy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yvedp.cn/gtqgkmuzfi.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gotoacloud.top/gtrwzmkzng.html

[N04] 斐波那契数列
来源：http://hz.xylfe.cn/gtzzvfgpdj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cheryme.top/gtzshsxavo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.gaohongyu789.top/gtsjcpctid.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.feifeiyinyue.top/gtvwybvcwy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shangyingyoupin.top/gtjdxthkbl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.daxiang520.top/gtlzzomtzd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.kuanghao11.cn/gtmyhqfubw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zdqjudy.top/gtevcaxolk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hnqzz.top/gtizsffvbm.html

[N05] 最大公约数
来源：http://hz.zhiwuduotai.top/gtlhtdsrkp.html

Py:   math.gcd(a, b)
来源：http://hz.jinqigufen.top/gtrkoujzwi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yueranfly.top/gtwltxpdxc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenlongwang.top/gtuvezsngs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pycfn.com/gtpxtxxokn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.quarkkingdee.top/gtconlxwdz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.0kj1m.cn/gtrhsdebpn.html

Ruby: a.gcd(b)
来源：http://hz.snrcjt.cn/gtxijxdtcf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.smart0.xyz/gtuvelwuki.html

[N06] 判断回文字符串
来源：http://hz.sxryk.cn/gtdzbskdkv.html

Py:   s == s[::-1]
来源：http://hz.ywan-chungtsiang.top/gthhzqmqef.html

PHP:  $s === strrev($s);
来源：http://hz.zhaomingkeji.xyz/gtxdqbfjmw.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtrjwimehj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.meibo888.top/gtaqafbebd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.316326.xyz/gtetemilhg.html

Go:   // 双指针从两端比较
来源：http://hz.hywenlv.cn/gtiwbpndaw.html

Ruby: s == s.reverse
来源：http://hz.snrcjt.cn/gtxaqxtvob.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.snrcjt.cn/gtklzglsyq.html

[N07] 两数之和（返回下标）
来源：http://hz.tianlin.xyz/gtlocpdjfp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zdqjudy.top/gttgiynimf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.andypj.xyz/gtrwlbnxcd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gaohongyu789.top/gtiipajfcl.html

TS:   // 手写 Map<string, number>
来源：http://hz.wangdashe.top/gtwvydyvqt.html

Java: // 手写 HashMap
来源：http://hz.yuanzhike.top/gtrvufggxy.html

Go:   // 手写 map[int]int
来源：http://hz.smart0.xyz/gtsuwwdkxf.html

Ruby: // 手写 Hash
来源：http://hz.jqgufenzy.top/gthdqiyjfh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.quarkkingdee.top/gtklubweko.html

[N08] 生成全排列
来源：http://hz.wangdashe.top/gtkmdclmzo.html

Py:   itertools.permutations(arr)
来源：http://hz.yj202588.top/gtjhylexea.html

PHP:  // 手写递归交换
来源：http://hz.cdnleiting.top/gtcamafzwa.html

JS:   // 手写回溯递归
来源：http://hz.ivvv.top/gtwrsjxmvc.html

TS:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtgqhmxutk.html

Java: // 手写回溯递归
来源：http://hz.aizwys.cn/gthkaptbqq.html

Go:   // 手写回溯递归
来源：http://hz.hammf.cn/gtcqrmmgsk.html

Ruby: arr.permutation.to_a
来源：http://hz.jinyuanbaomall.cn/gtzbtebdth.html

C#:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gtkwumzzjy.html

[N09] 栈与队列
来源：http://hz.wangshuangyany.cn/gtvsnvitjk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.daria6918.cn/gtdrufrjtn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xinyue.icu/gtpzxoljfu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.pycfn.com/gthovslpga.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ydjk.org.cn/gtcmqskcar.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jqgfzy.top/gteggrjlta.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.pengpengdd.cyou/gtadgavqik.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cucudq.cn/gtdsjeoggl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinqigfzy.top/gtbfdazhgk.html

[N10] 链表节点定义
来源：http://hz.pengpengdd.cyou/gtgdzpzmoj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.dashuyun.cn/gtpmlrsgvx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.guannengcc.top/gtxqngkfoo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sxryk.cn/gtmslmwvox.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yonumen.top/gtppgivuic.html

Java: class Node { int v; Node next; }
来源：http://hz.snrcjt.cn/gtwdsqyrex.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yj20258888.top/gtwlbutijh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yuanzhike.top/gtxjhgldjj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jqgufenzy.top/gtfswzmfjw.html

[N11] 二叉树中序遍历
来源：http://hz.hongshengwenyu.top/gtkygfbatv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sxryk.cn/gtjevavtcr.html

PHP:  // 手写递归函数
来源：http://hz.dianchejie.cn/gtsfqznhoy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.iojbl.cn/gtoexgnwhn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnxiangtu.top/gtlvhcejip.html

Java: // 手写递归
来源：http://hz.pengpengdd.cyou/gtqbroaxqs.html

Go:   // 手写递归
来源：http://hz.dianchejie.cn/gtjbgrghss.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.bjfxy.top/gtwkrtumef.html

C#:   // 手写递归
来源：http://hz.havefunace.top/gtdnzalcnr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.feifeiyinyue.top/gtqzsrscex.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.316326.xyz/gtlypcmenv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yanxiufei.cn/gtbrlvtczk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhengqikj.top/gthgmoagky.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.smart0.xyz/gtgdgwjinv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgufenzy.top/gtdregwcug.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shanyushiyangtech.top/gtvdtmibhm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhaomingkeji.xyz/gtfoxjpxha.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gtenaxnumr.html

================================================================================
来源：http://hz.snrcjt.cn/gttxdmazuh.html

O. 并发与异步
来源：http://hz.jinqigfzy.top/gtxwtvqdps.html

================================================================================
来源：http://hz.daxiang520.top/gteaoqihtg.html

[O01] 启动一个线程
来源：http://hz.9152youxi.cn/gtaqhqwpoz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jqgufenzy.top/gthtqpxyff.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cqqwz.cn/gtvprnycza.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenjidiqi.icu/gtufsygmia.html

TS:   // 同 JS
来源：http://hz.zhaomingkeji.xyz/gtcyavzype.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinqigfzy.top/gtzvkbeepc.html

Go:   go f()
来源：http://hz.sysykeji.top/gtdmblyvuy.html

Ruby: Thread.new { f }
来源：http://hz.nwbrower.top/gtiaxyfvgq.html

C#:   Task.Run(() => F());
来源：http://hz.yuanzhike.top/gtyfcdsbkd.html

[O02] 使用线程池
来源：http://hz.9152youxi.cn/gtluiryiik.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.meibo888.top/gtmliejiyd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.meibo888.top/gtgxlaqipk.html

JS:   // worker_threads 线程池
来源：http://hz.aibaodan.cn/gtibargckf.html

TS:   // worker_threads 线程池
来源：http://hz.guannengcc.top/gtersrlwio.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.316326.xyz/gtuarblaqc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ydjk.org.cn/gtngjasakp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.9152youxi.cn/gtvnxwyqfn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cucudq.cn/gtufjbngsv.html

[O03] 加锁保护共享数据
来源：http://hz.smart0.xyz/gtknjpflmm.html

Py:   with lock: shared += 1
来源：http://hz.gaohongyu789.top/gtobwoxdsm.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.gotoacloud.top/gtcfxuqjml.html


<!-- 参考信息 -->