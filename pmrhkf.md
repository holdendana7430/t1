代发 wailian999

[K06] 解析 URL 查询串
来源：http://hz.tian-w.cn/gtnzhfldcg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shanyushiyangtech.top/gtqqhbbkba.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ivvv.top/gtubhjimeo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.redwolf501.top/gtrpfoqvub.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.316326.xyz/gtodtmxmgr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.aibaodan.cn/gtxlgpclxe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yuanzhike.top/gtldcwpeez.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hnxiangtu.top/gtiktxjuip.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xinyue.icu/gtmjgjwvel.html

[K07] 进制转换
来源：http://hz.tanke756.top/gtbrwlmuil.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.aizwys.cn/gtesorrcxs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tian-w.cn/gtdjtfbqmr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.aizwys.cn/gttmzjjosh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.tian-w.cn/gtxjbhrmpp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yj20258.top/gthpujabnb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jyoumei.cn/gtszvzqfsc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.daria6918.cn/gtkyrarzqv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xuetiantiany.cn/gtaznqruvj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.daxiang520.top/gtaigumgrv.html

Py:   pickle.dumps(obj)
来源：http://hz.xziqi.cn/gtsvlzqycq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yuanzhike.top/gtlgbaakar.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shangyingyoupin.top/gtemwjnnyp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.svipenyu.cn/gtnobsnozv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shanyushiyangtech.top/gtncafmjka.html

Go:   encoding/gob
来源：http://hz.ydjk.org.cn/gtwkamdhan.html

Ruby: Marshal.dump(obj)
来源：http://hz.yj20258888.top/gtidbizhnz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sweek.top/gtjmwihgvm.html

================================================================================
来源：http://hz.yanxiufei.cn/gtrfimghsz.html

L. 网络请求
来源：http://hz.cucudq.cn/gtapxhymmd.html

================================================================================
来源：http://hz.jinqigufen.top/gtobyepcud.html

[L01] 发送 GET 请求
来源：http://hz.gzhubu.top/gtfonghblj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.fengsongda.top/gtmojwlldj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xziqi.cn/gtsvnaqeph.html

JS:   await fetch(url)
来源：http://hz.iojbl.cn/gtufhwcjdg.html

TS:   await fetch(url)
来源：http://hz.xylfe.cn/gtsmxrntjd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.316326.xyz/gtwooscojj.html

Go:   resp, err := http.Get(url)
来源：http://hz.jiagoushi.top/gtaxrmyytm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.tanke756.top/gthjhxopsy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.dianchejie.cn/gtucqykuge.html

[L02] 发送 POST JSON
来源：http://hz.cheryme.top/gtpkxoenqs.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ydzc1.top/gtaatvsjrs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhongyouzk.top/gtmexducju.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnqzz.top/gteyvgqhog.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sweek.top/gtfpdczutl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.nwbrower.top/gtmlvtdcwj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.snrcjt.cn/gtaeivmcjz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.c1oappe.top/gtqquvwuev.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.havefunace.top/gtdzdmllfs.html

[L03] 设置自定义请求头
来源：http://hz.sysykeji.top/gtesxixqow.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sxryk.cn/gtbugjnian.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ehwqpu.com/gtdibvzyfv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.316326.xyz/gttenygnsz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sysykeji.top/gtwcvkxwjx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cashguo.top/gtigergukt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhiwuduotai.top/gtripyvfuf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.pengpengdd.cyou/gtmkyktodd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cdnleiting.top/gtrvjmxnlx.html

[L04] 设置超时
来源：http://hz.hysaishi.cn/gtdqmcomeo.html

Py:   requests.get(url, timeout=5)
来源：http://hz.tian-w.cn/gtjgioohzz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ppjwa.cn/gtxlrfbyql.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fengsongda.top/gtjvnneguw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.feifeiyinyue.top/gtvuqghuva.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.daria6918.cn/gtsyxewjmt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yanxiufei.cn/gthpboakpl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hongshengwenyu.top/gtyhosdhsq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ydjk.org.cn/gtzpyowyps.html

[L05] 上传文件（multipart）
来源：http://hz.mhx1999.top/gtcbkghdmq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shzxlz.cn/gteavzshvt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhixingplan.top/gtsowkusbz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.fengsongda.top/gtsmilgfie.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zdqjudy.top/gtrsoxqexa.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.aizwys.cn/gtezbqjplp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.pycfn.com/gtzcapywwz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jiagoushi.top/gtzquifwts.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.bjfxy.top/gtiintiyev.html

[L06] 解析响应为 JSON
来源：http://hz.xuanzx.com/gtregvkozk.html

Py:   resp.json()
来源：http://hz.zhiwuduotai.top/gtkgbgvlsd.html

PHP:  json_decode($body, true);
来源：http://hz.cqqwz.cn/gtrqbamkoh.html

JS:   await resp.json()
来源：http://hz.tanke756.top/gtmywzdkfz.html

TS:   await resp.json()
来源：http://hz.hnqzz.top/gtgarihpio.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jqgfzy.top/gtfvqmqzsh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.birdmap.top/gtdtmdpqdz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tanke756.top/gtgsmqmxqx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yj20258.top/gthkaailaz.html

[L07] 处理 HTTP 状态码
来源：http://hz.sweek.top/gtgwlwtbeg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hnxiangtu.top/gtlnyyqpnd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.nwbrower.top/gtvtxmhkah.html

JS:   resp.ok;  resp.status
来源：http://hz.sufxvd.cn/gtnfzrcuxt.html

TS:   resp.ok;  resp.status
来源：http://hz.vqdsnc.cn/gttvcriozy.html

Java: resp.statusCode()
来源：http://hz.cqqwz.cn/gtzlgibcqf.html

Go:   resp.StatusCode
来源：http://hz.jinqigfzy.top/gtozlnhetk.html

Ruby: resp.code.to_i
来源：http://hz.hongshengwenyu.top/gtidycobrj.html

C#:   (int)resp.StatusCode
来源：http://hz.nanxinkj.top/gtufogithw.html

[L08] 并发请求多个地址
来源：http://hz.hfpthk.cn/gtwwhtoabt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gaohongyu789.top/gtsjciktvg.html

PHP:  curl_multi_init() 系列
来源：http://hz.yongpay.top/gtizzglbme.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangtech.top/gtofatqdfb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtdpkqbqic.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cheryme.top/gtshveetbx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.birdmap.top/gtpgkbrkqy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.kuanghao11.cn/gtwvuckxfo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.birdmap.top/gtxhvfqdgk.html

================================================================================
来源：http://hz.cheryme.top/gtlzbtjtch.html

M. 命令行 / 进程 / 环境
来源：http://hz.hfpthk.cn/gtxpfuasnx.html

================================================================================
来源：http://hz.daxiang520.top/gtkwjxczfr.html

[M01] 读取命令行参数
来源：http://hz.sweek.top/gtdxkunxvn.html

Py:   sys.argv[1:]
来源：http://hz.dashuyun.cn/gtjtgfcwai.html

PHP:  $argv;  $argc;
来源：http://hz.hnxiangtu.top/gtpmxkluqs.html

JS:   process.argv.slice(2)
来源：http://hz.yvedp.cn/gtqlagqyru.html

TS:   process.argv.slice(2)
来源：http://hz.jinqigufen.top/gtoecikgfh.html

Java: args 数组（main 方法参数）
来源：http://hz.pycfn.com/gtciimszsr.html

Go:   os.Args[1:]
来源：http://hz.xingfuxueyuan.xyz/gtbqmvpqtq.html

Ruby: ARGV
来源：http://hz.fzhhl.top/gttcpyqono.html

C#:   args 数组（Main 方法参数）
来源：http://hz.guannengcc.top/gtzxjsskjd.html

[M02] 读取环境变量
来源：http://hz.yuanzhike.top/gtsxmkahdi.html

Py:   os.environ.get("HOME")
来源：http://hz.xinyue.icu/gtzpkuoeem.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.pengpengdd.cyou/gtlyfwtdts.html

JS:   process.env.HOME
来源：http://hz.ydzc1.top/gthvfxoghr.html

TS:   process.env.HOME
来源：http://hz.svipenyu.cn/gtxlixgnkw.html

Java: System.getenv("HOME")
来源：http://hz.redwolf501.top/gtdcspzupv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cdnleiting.top/gtzrpylpme.html

Ruby: ENV["HOME"]
来源：http://hz.52xcode.cn/gtxuyhzevk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hnxiangtu.top/gtdtacievk.html

[M03] 执行外部命令
来源：http://hz.gogol.net.cn/gtvxlarklr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xuetiantiany.cn/gtgvipkbtw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shanyushiyangkeji.top/gtdvxqxtze.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.nanxuanxn.top/gtcijbykoq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.feifeiyinyue.top/gthhpsdnid.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.birdmap.top/gtbbwljjxq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.quarkkingdee.top/gterfqnlxc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sysykeji.top/gtcfavkmru.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gogol.net.cn/gtvzicqeso.html

[M04] 获取当前工作目录
来源：http://hz.pengpengdd.cyou/gtnexobuhb.html

Py:   os.getcwd()
来源：http://hz.xingfuxueyuan.xyz/gtoveqpttg.html

PHP:  getcwd();
来源：http://hz.zhaomingkeji.xyz/gtwwvesmyg.html

JS:   process.cwd()
来源：http://hz.shanyushiyangtech.top/gtdobuehcy.html

TS:   process.cwd()
来源：http://hz.yangfankeji.com/gtzbhzxizk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.daxiang520.top/gtyjmxeacp.html

Go:   os.Getwd()
来源：http://hz.chenjidiqi.icu/gtmkiyltas.html

Ruby: Dir.pwd
来源：http://hz.xingfuxueyuan.xyz/gtzjfpiplb.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.nwbrower.top/gtdibimjhl.html

[M05] 设置退出码
来源：http://hz.zhongyouzk.top/gtpwyryxzk.html

Py:   sys.exit(1)
来源：http://hz.aizwys.cn/gtqyjozuue.html

PHP:  exit(1);
来源：http://hz.ydzc1.top/gtqsjbvuzr.html

JS:   process.exit(1)
来源：http://hz.yonumen.top/gtlrooaols.html

TS:   process.exit(1)
来源：http://hz.guannengcc.top/gtbokewlxd.html

Java: System.exit(1)
来源：http://hz.xinyue.icu/gtquycdrlg.html

Go:   os.Exit(1)
来源：http://hz.yj20258888.top/gtcvbkpvhu.html

Ruby: exit 1
来源：http://hz.jqgufenzy.top/gtnegnxbor.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shanyushiyangtech.top/gtncwcekba.html

[M06] 向标准错误输出
来源：http://hz.gzhubu.top/gtljqhwccx.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhixingplan.top/gtrjopgodc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.pengpengdd.cyou/gtkkqzyriu.html

JS:   console.error("err")
来源：http://hz.jianghu66.top/gtnpgaubii.html

TS:   console.error("err")
来源：http://hz.xinyue.icu/gtcocrhxom.html

Java: System.err.println("err")
来源：http://hz.chenlongwang.top/gteobocafq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yongpay.top/gteaibhlbf.html

Ruby: warn "err"
来源：http://hz.xuanzx.com/gtrnqvfxgu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.chenlongwang.top/gtlrytsncm.html

[M07] 判断是否为主入口
来源：http://hz.pengpengdd.cyou/gtqedijiyj.html

Py:   if __name__ == "__main__":
来源：http://hz.aibaodan.cn/gtqyqyofyg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.vqdsnc.cn/gtcfdfqpui.html

JS:   require.main === module
来源：http://hz.zhaomingkeji.xyz/gtjnqohzww.html

TS:   require.main === module
来源：http://hz.xuetiantiany.cn/gtzlurepec.html

Java: public static void main(String[] args)
来源：http://hz.nanxinkj.top/gtmydygrun.html

Go:   func main()
来源：http://hz.zhiwuduotai.top/gtzzlnhfdd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.iojbl.cn/gtpryreuua.html

C#:   static void Main(string[] args)
来源：http://hz.ppjwa.cn/gtladdoqmi.html

[M08] 获取系统与运行时信息
来源：http://hz.zdqjudy.top/gtbzksxblc.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xinyue.icu/gtzlkfpzoe.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.nwbrower.top/gtzjijsbvz.html

JS:   process.platform;  process.version
来源：http://hz.hnxiangtu.top/gtzsnghrjj.html

TS:   process.platform;  process.version
来源：http://hz.ydzc1.top/gtbowprddi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.smart0.xyz/gttaherwvg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhaomingkeji.xyz/gttddlohpq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ehwqpu.com/gtrvawxykl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.316326.xyz/gtcaxgcxtn.html

================================================================================
来源：http://hz.fengsongda.top/gtjshkexxz.html

N. 数据结构与算法
来源：http://hz.gzhubu.top/gtcdpuqbeq.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtdoectifm.html

[N01] 二分查找（有序数组）
来源：http://hz.zdqjudy.top/gtkptvwbts.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.tian-w.cn/gtkpnxvmuc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yueranfly.top/gtgiooojgo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hysaishi.cn/gtkycacxik.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangdashe.top/gtjyeeuwmt.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.dashuyun.cn/gtskqvkjno.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yj20258.top/gtnuzzbqaz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.chenzaomai.com/gtkwkxzcbt.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhixingplan.top/gtimioapbi.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.mhx1999.top/gtxhmhnmbj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhijiandao.cn/gtvbpqhdoe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhaomingkeji.xyz/gttgvcyvog.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhiwuduotai.top/gtflqqzoui.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinqigufen.top/gtcujzdcjo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.dianchejie.cn/gtohwaokml.html

Go:   slices.Sort(arr)
来源：http://hz.xziqi.cn/gtequpddjj.html

Ruby: arr.sort
来源：http://hz.jinqigufen.top/gtlrtogmos.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yueranfly.top/gtochqedvu.html

[N03] 快速排序（分治示例）
来源：http://hz.jinqigfzy.top/gthimcgwge.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.iojbl.cn/gtymzmrvmz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.vqdsnc.cn/gtqfcndrmv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jianghu66.top/gttotsnlfa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cucudq.cn/gtpobdpjvu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ydzc1.top/gtuomsojqi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cashguo.top/gthldfudun.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.316326.xyz/gtyxgnelni.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zdqjudy.top/gtxpaeiecc.html

[N04] 斐波那契数列
来源：http://hz.c1oappe.top/gtglnpfjtx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.chenlongwang.top/gtdijaqmbp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yueranfly.top/gtwrktlthc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.wangdashe.top/gtxenkcqhm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ywan-chungtsiang.top/gtubotxdzx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.fzhhl.top/gtjggtokyv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jyoumei.cn/gtrhxzjsya.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jyoumei.cn/gtvxhnrram.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.snrcjt.cn/gtuhiseepe.html

[N05] 最大公约数
来源：http://hz.pengpengdd.cyou/gtuayljmbh.html

Py:   math.gcd(a, b)
来源：http://hz.ppjwa.cn/gtvaobxngd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.wangshuangyany.cn/gtiqerkmrl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sxryk.cn/gtvqkdlajy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jyoumei.cn/gtkoieadhm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.snrcjt.cn/gthguigppk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.gaohongyu789.top/gthwggncqk.html

Ruby: a.gcd(b)
来源：http://hz.hywenlv.cn/gtbqwhthoj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.sxryk.cn/gtnioyaros.html

[N06] 判断回文字符串
来源：http://hz.cdnleiting.top/gtjaurkbeh.html

Py:   s == s[::-1]
来源：http://hz.gogol.net.cn/gtvgvicumf.html

PHP:  $s === strrev($s);
来源：http://hz.0kj1m.cn/gtojlddzdx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shangyingyoupin.top/gtamrydbfu.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtyeofmzvn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shangyingyoupin.top/gthawddyfi.html

Go:   // 双指针从两端比较
来源：http://hz.wangdashe.top/gtcrxvreoo.html

Ruby: s == s.reverse
来源：http://hz.yj202588.top/gtwqqtjtda.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhongyouzk.top/gtqbswmuph.html

[N07] 两数之和（返回下标）
来源：http://hz.daria6918.cn/gtjtsxvqha.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gzhubu.top/gtcxtuksfu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.birdmap.top/gtjjyexmfy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ybcxt.top/gthyibbbvg.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinyuanbaomall.cn/gtjcxzsfql.html

Java: // 手写 HashMap
来源：http://hz.daxiang520.top/gtkmtrrsor.html

Go:   // 手写 map[int]int
来源：http://hz.quarkkingdee.top/gtbzjlwytz.html

Ruby: // 手写 Hash
来源：http://hz.xziqi.cn/gtiezcslqc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xinyue.icu/gtdwcxoyzs.html

[N08] 生成全排列
来源：http://hz.yj20258.top/gtwlgblrob.html

Py:   itertools.permutations(arr)
来源：http://hz.cqqwz.cn/gtjpiiihja.html

PHP:  // 手写递归交换
来源：http://hz.sufxvd.cn/gtklqjfsgp.html

JS:   // 手写回溯递归
来源：http://hz.yj202588.top/gtgrdsjqrl.html

TS:   // 手写回溯递归
来源：http://hz.sweek.top/gtshxnnour.html

Java: // 手写回溯递归
来源：http://hz.gotoacloud.top/gtxgwtacxd.html

Go:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtntsrwoje.html

Ruby: arr.permutation.to_a
来源：http://hz.cdnleiting.top/gtgtxrqaxh.html

C#:   // 手写回溯递归
来源：http://hz.quarkkingdee.top/gtmudatdvd.html

[N09] 栈与队列
来源：http://hz.zhongyouzk.top/gtoaezsqbb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yueranfly.top/gtbbuvqvmu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yonumen.top/gtkqzxjlit.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.nwbrower.top/gtdodcpfgb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jiagoushi.top/gtffciwede.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hnqzz.top/gtiirpuyer.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hnxiangtu.top/gtemygzsyj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jinyuanbaomall.cn/gtxcljmdyv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.svipenyu.cn/gthlmnjirl.html

[N10] 链表节点定义
来源：http://hz.hongshengwenyu.top/gtnigngglz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.tian-w.cn/gttikefetk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.tianlin.xyz/gtdcgwucof.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sysykeji.top/gtppcwksoi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.guowangkeji.top/gtsycaztoh.html

Java: class Node { int v; Node next; }
来源：http://hz.guowangkeji.top/gtznqxbwsy.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.pycfn.com/gtnmscgohz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.snrcjt.cn/gtzqkugxhi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cqqwz.cn/gtxdpctfji.html

[N11] 二叉树中序遍历
来源：http://hz.kuanghao11.cn/gtxvsduaga.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yvedp.cn/gtlhmihhlw.html

PHP:  // 手写递归函数
来源：http://hz.mhx1999.top/gthsnovarr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hywenlv.cn/gtakhbsdkg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhiwuduotai.top/gtifnrxqrw.html

Java: // 手写递归
来源：http://hz.nwbrower.top/gtiuixwmjs.html

Go:   // 手写递归
来源：http://hz.yj20258888.top/gtmuqmmlsu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yj20258888.top/gtevttqzlk.html

C#:   // 手写递归
来源：http://hz.jqgfzy.top/gtnxhxlohf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shanyushiyangtech.top/gtylwoknga.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.guowangkeji.top/gtvwkglqsq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinqigfzy.top/gttbjqifql.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydzc1.top/gtwrhuotyr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.vqdsnc.cn/gtdzrojdis.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tanke756.top/gtarqabslw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.vqdsnc.cn/gtgdhkjoxf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hywenlv.cn/gtjizoyvac.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cheryme.top/gtcbkcrtes.html

================================================================================
来源：http://hz.daria6918.cn/gtgkkrfacm.html

O. 并发与异步
来源：http://hz.jianghu66.top/gtvgvjowpo.html

================================================================================
来源：http://hz.xziqi.cn/gtvoodgwhg.html

[O01] 启动一个线程
来源：http://hz.ivvv.top/gthzcudtdb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sysykeji.top/gtwfpzzvma.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yanxiufei.cn/gttzoupkoa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jlsjyb.cn/gtdwtsjkfl.html

TS:   // 同 JS
来源：http://hz.dianchejie.cn/gtnaltozhi.html

Java: new Thread(() -> f()).start()
来源：http://hz.quarkkingdee.top/gtpjvibozz.html

Go:   go f()
来源：http://hz.zycfv.cn/gtmdftdjkt.html

Ruby: Thread.new { f }
来源：http://hz.shanyushiyangkeji.top/gtifgctcxf.html

C#:   Task.Run(() => F());
来源：http://hz.ywan-chungtsiang.top/gtasfrwiru.html


<!-- 参考信息 -->