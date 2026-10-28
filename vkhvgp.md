代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinqigufen.top/gtpjjztrus.html

[K07] 进制转换
来源：http://hz.sufxvd.cn/gtyivydsgu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhijiandao.cn/gtgscivoly.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.fengsongda.top/gtjbrzyxjg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhoulong.xyz/gtjoqldrox.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtyvhncaov.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tian-w.cn/gtvoyqsfhq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.dashuyun.cn/gtufmjdkrl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zdqjudy.top/gtdpzaucgp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xuetiantiany.cn/gtwsslaiuh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.redwolf501.top/gtxqyogafs.html

Py:   pickle.dumps(obj)
来源：http://hz.ywan-chungtsiang.top/gtbmyfybwu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tanke756.top/gttunyurzz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.c1oappe.top/gtpgaatsfz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hongshengwenyu.top/gtmfunxvtj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.pengpengdd.cyou/gtczahetxj.html

Go:   encoding/gob
来源：http://hz.xziqi.cn/gtflpbjnpw.html

Ruby: Marshal.dump(obj)
来源：http://hz.chenlongwang.top/gtpcqmlxfd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.mhx1999.top/gtesvihjmm.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtvdbsluzp.html

L. 网络请求
来源：http://hz.havefunace.top/gtxvcswjmq.html

================================================================================
来源：http://hz.yangfankeji.com/gtxsxbfbpp.html

[L01] 发送 GET 请求
来源：http://hz.kuanghao11.cn/gtbdrjoyjm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.fzhhl.top/gtgbcgvwts.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.dashuyun.cn/gtjcttyyxg.html

JS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gtaxjmhxkg.html

TS:   await fetch(url)
来源：http://hz.shanyushiyangkeji.top/gtjfodrhli.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhongyouzk.top/gthtxbfjdx.html

Go:   resp, err := http.Get(url)
来源：http://hz.snrcjt.cn/gtouxccafe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sysykeji.top/gtbaiintyi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhengqikj.top/gtbcpkdpct.html

[L02] 发送 POST JSON
来源：http://hz.hfpthk.cn/gtpwicynkj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.bjfxy.top/gteyktwwhc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.wangshuangyany.cn/gtqshsobdn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guannengcc.top/gtqyqmiykp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.quarkkingdee.top/gtzmsflvcf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hnxiangtu.top/gtpbkoldmz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ivvv.top/gtrjdygvaq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nwbrower.top/gtponxvfvw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.gaohongyu789.top/gtipxbfnjx.html

[L03] 设置自定义请求头
来源：http://hz.redwolf501.top/gtfyouqcda.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.tianlin.xyz/gtbtwckenm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yuanzhike.top/gtyjzkztfj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hongshengwenyu.top/gtpiifwrat.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ywan-chungtsiang.top/gtzxedvpye.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhongyouzk.top/gtfhjkbbeb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cqqwz.cn/gtrihcinnl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ywan-chungtsiang.top/gtmzstiuks.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jyoumei.cn/gtqqchhtuj.html

[L04] 设置超时
来源：http://hz.jinqigfzy.top/gtfkhlvswe.html

Py:   requests.get(url, timeout=5)
来源：http://hz.sufxvd.cn/gtfsgcijei.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinghuilouyu.cn/gtgefctzof.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnqzz.top/gtllhqsaez.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhengqikj.top/gtykmmuzgx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sufxvd.cn/gtnfxwjngn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.vqdsnc.cn/gtscoyanxi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.birdmap.top/gtlppbfgfg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.c1oappe.top/gttokjgtff.html

[L05] 上传文件（multipart）
来源：http://hz.yueranfly.top/gtzmzwjjji.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hammf.cn/gtyjpputcp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhongyouzk.top/gtklpftruw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xuetiantiany.cn/gtkunvtitk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.pengpengdd.cyou/gtxxtepnxo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ywan-chungtsiang.top/gtkdwftmwe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.gzhubu.top/gtemahgofm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ivvv.top/gtyjgylsee.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.iojbl.cn/gtnfdayoke.html

[L06] 解析响应为 JSON
来源：http://hz.sysykeji.top/gttqvggesh.html

Py:   resp.json()
来源：http://hz.hywenlv.cn/gtuvnoxear.html

PHP:  json_decode($body, true);
来源：http://hz.vqdsnc.cn/gtbpfdyidv.html

JS:   await resp.json()
来源：http://hz.xuanzx.com/gtsmskawyx.html

TS:   await resp.json()
来源：http://hz.jlsjyb.cn/gthloxesda.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinqigfzy.top/gtiydtgvqa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jianghu66.top/gtihtdrgik.html

Ruby: JSON.parse(resp.body)
来源：http://hz.smart0.xyz/gtuhvkexus.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.guowangkeji.top/gtvywcvmto.html

[L07] 处理 HTTP 状态码
来源：http://hz.haohaochexian.top/gtkrmtftmm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ppjwa.cn/gttknevuvr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.aibaodan.cn/gtntomjmkq.html

JS:   resp.ok;  resp.status
来源：http://hz.feifeiyinyue.top/gtpsjafzvt.html

TS:   resp.ok;  resp.status
来源：http://hz.cqqwz.cn/gthawlkchm.html

Java: resp.statusCode()
来源：http://hz.pengpengdd.cyou/gtqvlnibbm.html

Go:   resp.StatusCode
来源：http://hz.zhijiandao.cn/gtxzreembi.html

Ruby: resp.code.to_i
来源：http://hz.hongshengwenyu.top/gtsjtccisz.html

C#:   (int)resp.StatusCode
来源：http://hz.gogol.net.cn/gtonzarafr.html

[L08] 并发请求多个地址
来源：http://hz.chenjidiqi.icu/gtkyyvzhgk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yuxming.cn/gtpzmkslyy.html

PHP:  curl_multi_init() 系列
来源：http://hz.yongpay.top/gtvfrsular.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.meibo888.top/gtxlkqekwz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gtjjmkhols.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.aizwys.cn/gtachmhlbv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.smart0.xyz/gtbydzrqge.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhijiandao.cn/gtelksysap.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.c1oappe.top/gtrqpkktxk.html

================================================================================
来源：http://hz.shuidangran.top/gtbipzworg.html

M. 命令行 / 进程 / 环境
来源：http://hz.yueranfly.top/gtrhxjmjle.html

================================================================================
来源：http://hz.yuanzhike.top/gtuygqfpfz.html

[M01] 读取命令行参数
来源：http://hz.hnxiangtu.top/gtzpbuhvyt.html

Py:   sys.argv[1:]
来源：http://hz.sweek.top/gtnaaloewu.html

PHP:  $argv;  $argc;
来源：http://hz.sweek.top/gttcdrquhl.html

JS:   process.argv.slice(2)
来源：http://hz.dashuyun.cn/gtvmdywtuq.html

TS:   process.argv.slice(2)
来源：http://hz.ydjk.org.cn/gtolituabj.html

Java: args 数组（main 方法参数）
来源：http://hz.yuxming.cn/gthjoqergp.html

Go:   os.Args[1:]
来源：http://hz.9152youxi.cn/gtbbkascnd.html

Ruby: ARGV
来源：http://hz.aizwys.cn/gtdfnctadl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shuidangran.top/gtiuwmfock.html

[M02] 读取环境变量
来源：http://hz.xuanzx.com/gtijnhzebk.html

Py:   os.environ.get("HOME")
来源：http://hz.cucudq.cn/gtthqztuwq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.havefunace.top/gtayeujuls.html

JS:   process.env.HOME
来源：http://hz.iojbl.cn/gthymtclks.html

TS:   process.env.HOME
来源：http://hz.yvedp.cn/gtkvzbzcbh.html

Java: System.getenv("HOME")
来源：http://hz.hongshengwenyu.top/gtdgtzljio.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.nwbrower.top/gtepuxxnof.html

Ruby: ENV["HOME"]
来源：http://hz.zhongyouzk.top/gtfdnsaukc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hammf.cn/gtgcftcaas.html

[M03] 执行外部命令
来源：http://hz.yvedp.cn/gthkkacrqm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ydzc1.top/gtvjqnlmax.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.fzhhl.top/gtvahgotqe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.gaohongyu789.top/gtniuitgqm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangtech.top/gtokclyktm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.smart0.xyz/gtdsfoathe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.pengpengdd.cyou/gtqnjrgrfa.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shanyushiyangtech.top/gtncrauula.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jlsjyb.cn/gtjlpoksaw.html

[M04] 获取当前工作目录
来源：http://hz.jqgfzy.top/gtafklcrof.html

Py:   os.getcwd()
来源：http://hz.xziqi.cn/gtkqkkotpe.html

PHP:  getcwd();
来源：http://hz.meibo888.top/gtzqudfidl.html

JS:   process.cwd()
来源：http://hz.nanxinkj.top/gtxylkagqm.html

TS:   process.cwd()
来源：http://hz.daria6918.cn/gtjebxgfhu.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yuanzhike.top/gtfncjmlgm.html

Go:   os.Getwd()
来源：http://hz.gogol.net.cn/gtmvmfzwxw.html

Ruby: Dir.pwd
来源：http://hz.jqgufenzy.top/gtjhjmaonl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.c1oappe.top/gtehffkcsx.html

[M05] 设置退出码
来源：http://hz.wangshuangyany.cn/gtupemmivq.html

Py:   sys.exit(1)
来源：http://hz.haohaochexian.top/gtddsxnvgc.html

PHP:  exit(1);
来源：http://hz.zhengqikj.top/gtbfoholuh.html

JS:   process.exit(1)
来源：http://hz.sweek.top/gtzhqwqsnw.html

TS:   process.exit(1)
来源：http://hz.cheryme.top/gtkqaqajwm.html

Java: System.exit(1)
来源：http://hz.gotoacloud.top/gtipkbnhaw.html

Go:   os.Exit(1)
来源：http://hz.hnqzz.top/gtvpnjlxpd.html

Ruby: exit 1
来源：http://hz.hnqzz.top/gttplbtomg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yangfankeji.com/gtdgxfqinz.html

[M06] 向标准错误输出
来源：http://hz.hywenlv.cn/gtoodzhrnq.html

Py:   print("err", file=sys.stderr)
来源：http://hz.aibaodan.cn/gtoqplksyx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhijiandao.cn/gtoeowclkc.html

JS:   console.error("err")
来源：http://hz.c1oappe.top/gtabltwttm.html

TS:   console.error("err")
来源：http://hz.zhiwuduotai.top/gthqikvake.html

Java: System.err.println("err")
来源：http://hz.sufxvd.cn/gtqfoqwaoj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yuxming.cn/gteswusojf.html

Ruby: warn "err"
来源：http://hz.yvedp.cn/gtyouuhced.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhongyouzk.top/gtukivruyo.html

[M07] 判断是否为主入口
来源：http://hz.ppjwa.cn/gteyeasydl.html

Py:   if __name__ == "__main__":
来源：http://hz.shangyingyoupin.top/gtxhmodtpp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.andypj.xyz/gtsbghhski.html

JS:   require.main === module
来源：http://hz.nanxuanxn.top/gttjimdpmo.html

TS:   require.main === module
来源：http://hz.52xcode.cn/gtwapfhvvb.html

Java: public static void main(String[] args)
来源：http://hz.bjfxy.top/gtgorocuaj.html

Go:   func main()
来源：http://hz.tian-w.cn/gtipwvjewk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.tian-w.cn/gtbovkkgxl.html

C#:   static void Main(string[] args)
来源：http://hz.yanxiufei.cn/gtxqeomvzk.html

[M08] 获取系统与运行时信息
来源：http://hz.kuanghao11.cn/gtphxdpobt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhijiandao.cn/gtjtziqsuk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xuanzx.com/gtxhrwohbd.html

JS:   process.platform;  process.version
来源：http://hz.shzxlz.cn/gtwblwamne.html

TS:   process.platform;  process.version
来源：http://hz.hywenlv.cn/gtjmhmcvoi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hammf.cn/gtmltgiekz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yangfankeji.com/gtixkvdfyz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yuanzhike.top/gticftqpsh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinqigufen.top/gtrkvxdqhx.html

================================================================================
来源：http://hz.jinqigufen.top/gtwudidugg.html

N. 数据结构与算法
来源：http://hz.aizwys.cn/gtnmwzjrgv.html

================================================================================
来源：http://hz.jinqigufen.top/gtplujyvtv.html

[N01] 二分查找（有序数组）
来源：http://hz.ydjk.org.cn/gtasgxthuw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jyoumei.cn/gtqrckyaey.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.daria6918.cn/gtqxmwneoz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jianghu66.top/gtkhhxansv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hammf.cn/gtgeylvktp.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jiagoushi.top/gtgaedcewn.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gogol.net.cn/gtmzwsjbsd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hongshengwenyu.top/gtzozfdcom.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.fzhhl.top/gtgozvafpg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.aibaodan.cn/gtydkfktsa.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.bjfxy.top/gtzvnqwcxz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jlsjyb.cn/gtochjsvol.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.haohaochexian.top/gtfwcrnmqj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jiagoushi.top/gtifyspjjh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhixingplan.top/gtpkpueidk.html

Go:   slices.Sort(arr)
来源：http://hz.ydjk.org.cn/gtqjscntrs.html

Ruby: arr.sort
来源：http://hz.yj20258.top/gtiqilxkif.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.gogol.net.cn/gtzkgbnusf.html

[N03] 快速排序（分治示例）
来源：http://hz.xuanzx.com/gtswixlmfc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.vqdsnc.cn/gtmrqihlqn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hnqzz.top/gtowzvtjgw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgfzy.top/gtomioqdqr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuanzhike.top/gtwssucola.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.nwbrower.top/gtmghwjhxf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.wangshuangyany.cn/gttxuefsqx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hnqzz.top/gtjscajcbm.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jinqigfzy.top/gtmnoaywub.html

[N04] 斐波那契数列
来源：http://hz.zhijiandao.cn/gtvstcbsca.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xuetiantiany.cn/gtdjatqntb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sysykeji.top/gtvrotvxsg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.vqdsnc.cn/gtjzqpkyci.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daxiang520.top/gtneovvbny.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hnxiangtu.top/gtjqioszhw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.nanxuanxn.top/gtbxdrttdk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sufxvd.cn/gtfknaytte.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.daxiang520.top/gtncdxeozh.html

[N05] 最大公约数
来源：http://hz.zhengqikj.top/gtsunooujt.html

Py:   math.gcd(a, b)
来源：http://hz.yonumen.top/gtqbgkdtyl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.aibaodan.cn/gttqufpsyx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xuetiantiany.cn/gtelnkexnl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj202588.top/gtsjvtumwx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenlongwang.top/gtkklmreyf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.haohaochexian.top/gtmomcwicz.html

Ruby: a.gcd(b)
来源：http://hz.cashguo.top/gtpzlmnsnx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.chenzaomai.com/gtujimcrzy.html

[N06] 判断回文字符串
来源：http://hz.jqgfzy.top/gtsegthigs.html

Py:   s == s[::-1]
来源：http://hz.tian-w.cn/gtnwrzstea.html

PHP:  $s === strrev($s);
来源：http://hz.zhongyouzk.top/gtalucpuhv.html

JS:   s === [...s].reverse().join("")
来源：http://hz.havefunace.top/gtgcyioqgz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtnebqaqfq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.gotoacloud.top/gtljdgxtmk.html

Go:   // 双指针从两端比较
来源：http://hz.hongshengwenyu.top/gtqojnveks.html

Ruby: s == s.reverse
来源：http://hz.zhaomingkeji.xyz/gtyythzgmy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xuetiantiany.cn/gtxxxzwxfz.html

[N07] 两数之和（返回下标）
来源：http://hz.nanxuanxn.top/gtdlxezovh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gaohongyu789.top/gtudjtvayc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.pengpengdd.cyou/gtcytvmwdw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ydzc1.top/gtnmsskgnn.html

TS:   // 手写 Map<string, number>
来源：http://hz.jqgfzy.top/gtzusqswdy.html

Java: // 手写 HashMap
来源：http://hz.zycfv.cn/gtmyonbwte.html

Go:   // 手写 map[int]int
来源：http://hz.guannengcc.top/gtxquuokyl.html

Ruby: // 手写 Hash
来源：http://hz.yj20258888.top/gtjfmsuyiv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hysaishi.cn/gtmowvjqwf.html

[N08] 生成全排列
来源：http://hz.mhx1999.top/gtqtcartdm.html

Py:   itertools.permutations(arr)
来源：http://hz.hnqzz.top/gtmvzeqvjw.html

PHP:  // 手写递归交换
来源：http://hz.zhiwuduotai.top/gttbiijryk.html

JS:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtpegtgsny.html

TS:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtlqdexkor.html

Java: // 手写回溯递归
来源：http://hz.mhx1999.top/gtsiszdbpm.html

Go:   // 手写回溯递归
来源：http://hz.sysykeji.top/gtmkyxvkyj.html

Ruby: arr.permutation.to_a
来源：http://hz.52xcode.cn/gtspqhhtfg.html

C#:   // 手写回溯递归
来源：http://hz.zycfv.cn/gtxzqsrrem.html

[N09] 栈与队列
来源：http://hz.jiagoushi.top/gtwdmduiiz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yuxming.cn/gtiipkubuy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hnqzz.top/gtcnquplxb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yanxiufei.cn/gtdmpjnlqq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yongpay.top/gtntfswagl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ehwqpu.com/gtsawxuwfk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.andypj.xyz/gtstbybbwg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jinghuilouyu.cn/gtnrdfazgl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.wangdashe.top/gtqvnwasng.html

[N10] 链表节点定义
来源：http://hz.ydzc1.top/gtatfxeonz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.meibo888.top/gtrxxdvuyr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jianghu66.top/gtrdllwchs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.birdmap.top/gthcdegnib.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yj202588.top/gtldeqgyim.html

Java: class Node { int v; Node next; }
来源：http://hz.hnqzz.top/gtijmdrdsp.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.sweek.top/gtgkcamssu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.kuanghao11.cn/gtxmqkkeap.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yvedp.cn/gtpirsgxde.html

[N11] 二叉树中序遍历
来源：http://hz.shanyushiyangkeji.top/gtmopcnqty.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xinyue.icu/gtqjxjzrkl.html

PHP:  // 手写递归函数
来源：http://hz.jinqigfzy.top/gtsaokrdjc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zdqjudy.top/gtthwdqpjj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tian-w.cn/gtuhsbinwp.html

Java: // 手写递归
来源：http://hz.guowangkeji.top/gtrzqmqvcu.html

Go:   // 手写递归
来源：http://hz.jinyuanbaomall.cn/gtqidxmvob.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.daria6918.cn/gtonsfyrtl.html

C#:   // 手写递归
来源：http://hz.jinyuanbaomall.cn/gtwwbdonlp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yj20258.top/gtymkqszps.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhijiandao.cn/gtynpwluei.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhengqikj.top/gtxkxdjxnu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgfzy.top/gtduwjltny.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgufenzy.top/gtgeknbbdv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shzxlz.cn/gtotnkaeaw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jinyuanbaomall.cn/gtplmgsljm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.havefunace.top/gtaubwncon.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.c1oappe.top/gtxzuwjwwl.html

================================================================================
来源：http://hz.zhoulong.xyz/gtbichobsf.html

O. 并发与异步
来源：http://hz.yueranfly.top/gtwaespqvm.html

================================================================================
来源：http://hz.aibaodan.cn/gtizmdnxts.html

[O01] 启动一个线程
来源：http://hz.birdmap.top/gtbralvlmz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.quarkkingdee.top/gtbxzslrvb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhongyouzk.top/gtwbfupmuf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.sysykeji.top/gtevjxmczd.html

TS:   // 同 JS
来源：http://hz.andypj.xyz/gtqoedrczr.html

Java: new Thread(() -> f()).start()
来源：http://hz.jiagoushi.top/gtlxdguxza.html

Go:   go f()
来源：http://hz.sxryk.cn/gtufvflsii.html

Ruby: Thread.new { f }
来源：http://hz.redwolf501.top/gttnzgxscu.html

C#:   Task.Run(() => F());
来源：http://hz.ivvv.top/gtpatbyyni.html

[O02] 使用线程池
来源：http://hz.mhx1999.top/gtowvtopai.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jianghu66.top/gtjswgpufo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hnxiangtu.top/gtaxmvsrml.html

JS:   // worker_threads 线程池
来源：http://hz.smart0.xyz/gtfrkgyduf.html

TS:   // worker_threads 线程池
来源：http://hz.yangfankeji.com/gtzwaauihr.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jianghu66.top/gtooidltso.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.fzhhl.top/gtwsmnewrk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.dashuyun.cn/gtowrhhqxs.html


<!-- 参考信息 -->