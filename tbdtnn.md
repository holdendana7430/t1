代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.pengpengdd.cyou/gtqmvlespd.html

[K07] 进制转换
来源：http://hz.guannengcc.top/gtllhpsuur.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.0kj1m.cn/gtjcopdzdr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.havefunace.top/gtzxseyiwf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.haohaochexian.top/gtlmafaizg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.feifeiyinyue.top/gtxpzhvclj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yanxiufei.cn/gtvbuydfcd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xingfuxueyuan.xyz/gtaijxfhio.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.havefunace.top/gtikvimbnt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj20258.top/gtodctdyye.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.tanke756.top/gthaviyevp.html

Py:   pickle.dumps(obj)
来源：http://hz.haohaochexian.top/gtakxltuja.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.daria6918.cn/gtcktlssaa.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinghuilouyu.cn/gtdlnhmfzk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yvedp.cn/gtvdkpvpfm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.aibaodan.cn/gtqpfbnjbt.html

Go:   encoding/gob
来源：http://hz.guannengcc.top/gtwlwyztvd.html

Ruby: Marshal.dump(obj)
来源：http://hz.pengpengdd.cyou/gttwuqbvfy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gogol.net.cn/gtpzecxghz.html

================================================================================
来源：http://hz.jianghu66.top/gtcubaibau.html

L. 网络请求
来源：http://hz.havefunace.top/gtqsrhvjdv.html

================================================================================
来源：http://hz.ybcxt.top/gtczsnzsnu.html

[L01] 发送 GET 请求
来源：http://hz.vqdsnc.cn/gtkludoaud.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ybcxt.top/gtxdnqidml.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jianghu66.top/gtbvpckqtt.html

JS:   await fetch(url)
来源：http://hz.fzhhl.top/gtrtrzztbw.html

TS:   await fetch(url)
来源：http://hz.yongpay.top/gtzyovlacg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yangfankeji.com/gtlrnssdqh.html

Go:   resp, err := http.Get(url)
来源：http://hz.wangshuangyany.cn/gtnwjmoylo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xuetiantiany.cn/gtezvjflpa.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.nanxuanxn.top/gtptrktqno.html

[L02] 发送 POST JSON
来源：http://hz.jinqigufen.top/gtqcxdboeq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.tian-w.cn/gtwmyiuzpp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yj20258888.top/gtaeywvfjn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yongpay.top/gtyxidrbui.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.birdmap.top/gtfezgysfp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ppjwa.cn/gtzgtdznnk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gotoacloud.top/gtsfjnrmge.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hongshengwenyu.top/gttakfniku.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.dashuyun.cn/gtdktpjbqe.html

[L03] 设置自定义请求头
来源：http://hz.wangshuangyany.cn/gtkyynzirl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yueranfly.top/gtcyyhchhh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.chenjidiqi.icu/gtpnhuvcmb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zdqjudy.top/gtxlanlmhg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.9152youxi.cn/gtpojqsvnx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yj20258.top/gtngqbxdhp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.snrcjt.cn/gtcayhapqm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.iojbl.cn/gtargjebws.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yvedp.cn/gtktarcrxr.html

[L04] 设置超时
来源：http://hz.gogol.net.cn/gtfgdbtzqh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cqqwz.cn/gtqhxolpfa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinqigufen.top/gtwzqdrbsb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.mhx1999.top/gtayduoswb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hysaishi.cn/gtrjwkbqtt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ydzc1.top/gtfwjhpprn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hfpthk.cn/gtzovsakfc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinyuanbaomall.cn/gttomghubx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xziqi.cn/gthufoaclo.html

[L05] 上传文件（multipart）
来源：http://hz.zhoulong.xyz/gtvrhzosbn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj202588.top/gtudpxjaty.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.smart0.xyz/gtvbgtnhpl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.iojbl.cn/gtccbxxdog.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.dashuyun.cn/gtazfzmjvg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.iojbl.cn/gttdrvxfdn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhoulong.xyz/gtzdcktkvl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ivvv.top/gtdselowhe.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jianghu66.top/gtuctvqydi.html

[L06] 解析响应为 JSON
来源：http://hz.ppjwa.cn/gtyvhfygpd.html

Py:   resp.json()
来源：http://hz.smart0.xyz/gtdxvntgtu.html

PHP:  json_decode($body, true);
来源：http://hz.mhx1999.top/gtbjxzswdm.html

JS:   await resp.json()
来源：http://hz.ehwqpu.com/gtwyqnohob.html

TS:   await resp.json()
来源：http://hz.fengsongda.top/gtvdcvxdvm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shuidangran.top/gtwbogitxl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sufxvd.cn/gtafqpccpn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ywan-chungtsiang.top/gtiulqwerw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hnxiangtu.top/gtdihxfpcr.html

[L07] 处理 HTTP 状态码
来源：http://hz.chenlongwang.top/gtcuzvnxxc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.tian-w.cn/gtrexzfhbn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.birdmap.top/gteheyrwmv.html

JS:   resp.ok;  resp.status
来源：http://hz.sysykeji.top/gtgdzptdjz.html

TS:   resp.ok;  resp.status
来源：http://hz.fengsongda.top/gttmjuwhkl.html

Java: resp.statusCode()
来源：http://hz.meibo888.top/gtniwsttdx.html

Go:   resp.StatusCode
来源：http://hz.zhongyouzk.top/gtfestsuze.html

Ruby: resp.code.to_i
来源：http://hz.jqgufenzy.top/gtclnlrnmx.html

C#:   (int)resp.StatusCode
来源：http://hz.nwbrower.top/gtjnyruvix.html

[L08] 并发请求多个地址
来源：http://hz.jinyuanbaomall.cn/gtpkmrhsij.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xuanzx.com/gtvyakauzz.html

PHP:  curl_multi_init() 系列
来源：http://hz.cucudq.cn/gtedjfexxj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pengpengdd.cyou/gtfoshjqiq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tianlin.xyz/gtcbvjtnnw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hysaishi.cn/gtpxmtqxkf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jiagoushi.top/gtkyeomhuk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yonumen.top/gtpnszltkr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.dashuyun.cn/gtbrouddsy.html

================================================================================
来源：http://hz.dashuyun.cn/gtbmusvqgz.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhijiandao.cn/gtvahvzldg.html

================================================================================
来源：http://hz.hnxiangtu.top/gtrqnnaxbs.html

[M01] 读取命令行参数
来源：http://hz.gaohongyu789.top/gtdiuqnxgu.html

Py:   sys.argv[1:]
来源：http://hz.jqgfzy.top/gtbhslrwwh.html

PHP:  $argv;  $argc;
来源：http://hz.gogol.net.cn/gtcrhdlrjf.html

JS:   process.argv.slice(2)
来源：http://hz.xuanzx.com/gtpzaojtge.html

TS:   process.argv.slice(2)
来源：http://hz.zhaomingkeji.xyz/gtxjujlupr.html

Java: args 数组（main 方法参数）
来源：http://hz.cucudq.cn/gtawauqjgc.html

Go:   os.Args[1:]
来源：http://hz.mhx1999.top/gtyvvfkuxr.html

Ruby: ARGV
来源：http://hz.yj20258888.top/gtoommfegh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.redwolf501.top/gtnjitxjqq.html

[M02] 读取环境变量
来源：http://hz.jyoumei.cn/gtajvqkhcg.html

Py:   os.environ.get("HOME")
来源：http://hz.hnxiangtu.top/gtbflhqxrf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jlsjyb.cn/gtuuwlbmkt.html

JS:   process.env.HOME
来源：http://hz.hongshengwenyu.top/gtdqaxvucw.html

TS:   process.env.HOME
来源：http://hz.52xcode.cn/gtkmmobfkv.html

Java: System.getenv("HOME")
来源：http://hz.316326.xyz/gtrywzfaal.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yvedp.cn/gttnqgllkb.html

Ruby: ENV["HOME"]
来源：http://hz.hnxiangtu.top/gtivxvthav.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.snrcjt.cn/gtxlzyarod.html

[M03] 执行外部命令
来源：http://hz.sufxvd.cn/gtuxbvlyef.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.mhx1999.top/gtxrcmlsfy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ydzc1.top/gtihhqtmbf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.gotoacloud.top/gtmpizwsiv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.feifeiyinyue.top/gtdtbknsyr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.daxiang520.top/gtcoobzlfa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yongpay.top/gtsexpvvau.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jianghu66.top/gtwtryhxnf.html

C#:   Process.Start("ls", "-l");
来源：http://hz.quarkkingdee.top/gtnqtlfulm.html

[M04] 获取当前工作目录
来源：http://hz.yonumen.top/gtshcmssnq.html

Py:   os.getcwd()
来源：http://hz.yuxming.cn/gtenxzbsru.html

PHP:  getcwd();
来源：http://hz.hammf.cn/gtcwybfcnq.html

JS:   process.cwd()
来源：http://hz.quarkkingdee.top/gtyzegxqhz.html

TS:   process.cwd()
来源：http://hz.sufxvd.cn/gtpaffsfqb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xuetiantiany.cn/gtewtxdbbg.html

Go:   os.Getwd()
来源：http://hz.smart0.xyz/gtgurbdmft.html

Ruby: Dir.pwd
来源：http://hz.cheryme.top/gtdwqcrtbx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhoulong.xyz/gtfjyhunlo.html

[M05] 设置退出码
来源：http://hz.xuanzx.com/gtlxamirwu.html

Py:   sys.exit(1)
来源：http://hz.zdqjudy.top/gtrbgetutb.html

PHP:  exit(1);
来源：http://hz.wangdashe.top/gtyrborojk.html

JS:   process.exit(1)
来源：http://hz.yueranfly.top/gtkfjgzjrz.html

TS:   process.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtlbkxssyj.html

Java: System.exit(1)
来源：http://hz.hammf.cn/gtyrbtuzme.html

Go:   os.Exit(1)
来源：http://hz.xuanzx.com/gtkpokrfpw.html

Ruby: exit 1
来源：http://hz.aizwys.cn/gtzotivsvg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ppjwa.cn/gtkbuwygsz.html

[M06] 向标准错误输出
来源：http://hz.wangdashe.top/gtbzpzlgpn.html

Py:   print("err", file=sys.stderr)
来源：http://hz.tianlin.xyz/gtgqhqqklx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhijiandao.cn/gtkgnpjyim.html

JS:   console.error("err")
来源：http://hz.shangyingyoupin.top/gtpfdlkipi.html

TS:   console.error("err")
来源：http://hz.sweek.top/gtevhcpjuc.html

Java: System.err.println("err")
来源：http://hz.yuanzhike.top/gtvfhtzohj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hywenlv.cn/gtumtintya.html

Ruby: warn "err"
来源：http://hz.guowangkeji.top/gtasgxrdwg.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.tanke756.top/gtgqinipoy.html

[M07] 判断是否为主入口
来源：http://hz.xingfuxueyuan.xyz/gttdrpwirh.html

Py:   if __name__ == "__main__":
来源：http://hz.jyoumei.cn/gtebrbyyln.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hywenlv.cn/gthcgpbggn.html

JS:   require.main === module
来源：http://hz.bjfxy.top/gtdinqmfrl.html

TS:   require.main === module
来源：http://hz.yueranfly.top/gtrqrlxsxe.html

Java: public static void main(String[] args)
来源：http://hz.nanxinkj.top/gttvwanxmg.html

Go:   func main()
来源：http://hz.xuanzx.com/gtklbyqier.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yanxiufei.cn/gtmyokkcjg.html

C#:   static void Main(string[] args)
来源：http://hz.tianlin.xyz/gtmpvdvxyb.html

[M08] 获取系统与运行时信息
来源：http://hz.chenlongwang.top/gtgqoexhkm.html

Py:   platform.system();  platform.python_version()
来源：http://hz.c1oappe.top/gtmlaimmkk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.quarkkingdee.top/gtincysrsm.html

JS:   process.platform;  process.version
来源：http://hz.gogol.net.cn/gtvslskypd.html

TS:   process.platform;  process.version
来源：http://hz.smart0.xyz/gtowocgupa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shuidangran.top/gtbudpqirl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yangfankeji.com/gtarsbtmlx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xuetiantiany.cn/gtsvluulwo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shzxlz.cn/gtndtktjlm.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtccwwjwhu.html

N. 数据结构与算法
来源：http://hz.jiagoushi.top/gtktaxaylx.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtudnpnpxl.html

[N01] 二分查找（有序数组）
来源：http://hz.sxryk.cn/gtoatewata.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nanxinkj.top/gtvwyhkkrf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shanyushiyangkeji.top/gtfzuoxqlb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hysaishi.cn/gtrffqbfdz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yueranfly.top/gtlqdratoi.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cheryme.top/gtqfzfrkei.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.0kj1m.cn/gtbqhthtuk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yangfankeji.com/gtvanfpfsm.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ppjwa.cn/gtvlcoqvis.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yonumen.top/gtodnxonxa.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jianghu66.top/gtseumfdie.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jqgfzy.top/gtkoqdimry.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ivvv.top/gttrubpgsf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hfpthk.cn/gtuwqbrzmr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shuidangran.top/gtmfjikpva.html

Go:   slices.Sort(arr)
来源：http://hz.ydjk.org.cn/gtzonnkypz.html

Ruby: arr.sort
来源：http://hz.xylfe.cn/gtndzthplv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.havefunace.top/gtxmwaafwr.html

[N03] 快速排序（分治示例）
来源：http://hz.shanyushiyangkeji.top/gtmildvtjf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yj20258888.top/gtyyswhjtl.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xuanzx.com/gtkvfukbfc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhiwuduotai.top/gthksceaov.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.mhx1999.top/gthlpleehm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jyoumei.cn/gtdrorgvml.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yangfankeji.com/gtgpubbhqi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.havefunace.top/gtcaqinetm.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xylfe.cn/gtqbierbmp.html

[N04] 斐波那契数列
来源：http://hz.chenlongwang.top/gtesvtxppv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.chenlongwang.top/gtebzntedn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ppjwa.cn/gtvqmxllkz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shangyingyoupin.top/gtnpdpljkg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnqzz.top/gtnoqoasua.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yangfankeji.com/gtcbjajqcu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.0kj1m.cn/gtflmxoafd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.chenjidiqi.icu/gtfrclinyk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gzhubu.top/gtqdhgkwdv.html

[N05] 最大公约数
来源：http://hz.smart0.xyz/gtbinasssj.html

Py:   math.gcd(a, b)
来源：http://hz.aizwys.cn/gtukevqtai.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.pycfn.com/gtgnvfgncq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gtrmzllxhe.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnqzz.top/gttmrdiymy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ydzc1.top/gtwdeerkki.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ppjwa.cn/gtwepbbqiw.html

Ruby: a.gcd(b)
来源：http://hz.yuanzhike.top/gtyxfrhfng.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.pycfn.com/gtkrumxwyi.html

[N06] 判断回文字符串
来源：http://hz.hysaishi.cn/gtdyvcytaw.html

Py:   s == s[::-1]
来源：http://hz.jinqigufen.top/gtcrncmssb.html

PHP:  $s === strrev($s);
来源：http://hz.xylfe.cn/gtwbhgfiri.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hnqzz.top/gtirhobeyk.html

TS:   s === [...s].reverse().join("")
来源：http://hz.meibo888.top/gtqzrwrcbz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.redwolf501.top/gtjfzrbilg.html

Go:   // 双指针从两端比较
来源：http://hz.dianchejie.cn/gtkoghdbbf.html

Ruby: s == s.reverse
来源：http://hz.tianlin.xyz/gtfhciilxd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yvedp.cn/gteeznswea.html

[N07] 两数之和（返回下标）
来源：http://hz.yuanzhike.top/gtjuycyxif.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xuanzx.com/gtrherueij.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jlsjyb.cn/gtpabbvpjm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.wangdashe.top/gtzdndqkmq.html

TS:   // 手写 Map<string, number>
来源：http://hz.andypj.xyz/gtvpzveajm.html

Java: // 手写 HashMap
来源：http://hz.nanxuanxn.top/gtnxwzqflf.html

Go:   // 手写 map[int]int
来源：http://hz.yj20258888.top/gtikbfaxtt.html

Ruby: // 手写 Hash
来源：http://hz.jlsjyb.cn/gtevtifcld.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hammf.cn/gtkwjbkitk.html

[N08] 生成全排列
来源：http://hz.wangdashe.top/gtcxoagyge.html

Py:   itertools.permutations(arr)
来源：http://hz.yonumen.top/gtmniyiifp.html

PHP:  // 手写递归交换
来源：http://hz.sxryk.cn/gtfxxeskwu.html

JS:   // 手写回溯递归
来源：http://hz.cqqwz.cn/gtkjcaessa.html

TS:   // 手写回溯递归
来源：http://hz.tian-w.cn/gthkcmvgww.html

Java: // 手写回溯递归
来源：http://hz.hammf.cn/gtpqasbjcb.html

Go:   // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtnffhvhop.html

Ruby: arr.permutation.to_a
来源：http://hz.jinqigufen.top/gtbsfushkz.html

C#:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtoocbkxnw.html

[N09] 栈与队列
来源：http://hz.jinghuilouyu.cn/gtpzpfsykc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.meibo888.top/gtxmfudqvw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.vqdsnc.cn/gtwfebjyxm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zycfv.cn/gtfbgjpgid.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hywenlv.cn/gttpiabvyc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.guannengcc.top/gtdjtndtli.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinqigufen.top/gtwpebwvnn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.guannengcc.top/gtvililwyq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xuetiantiany.cn/gteptihgky.html

[N10] 链表节点定义
来源：http://hz.wangdashe.top/gtrdsjnhtw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.chenzaomai.com/gtdogptzbi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hfpthk.cn/gtymvefwwy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gogol.net.cn/gtojlmmwdh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.52xcode.cn/gtkpntgeie.html

Java: class Node { int v; Node next; }
来源：http://hz.jinqigfzy.top/gtbtlrlvxx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.316326.xyz/gtiohtpttf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.pengpengdd.cyou/gturnyakrl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.guannengcc.top/gtgefozaio.html

[N11] 二叉树中序遍历
来源：http://hz.sufxvd.cn/gtvhhtyoaw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhongyouzk.top/gtpqwkjrav.html

PHP:  // 手写递归函数
来源：http://hz.jinqigufen.top/gtuwbkxton.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.havefunace.top/gtdjvaxksp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.daria6918.cn/gtancjvnwr.html

Java: // 手写递归
来源：http://hz.hywenlv.cn/gtnssvkbxk.html

Go:   // 手写递归
来源：http://hz.smart0.xyz/gtwenlmslv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shanyushiyangkeji.top/gtdzlsjqno.html

C#:   // 手写递归
来源：http://hz.shanyushiyangkeji.top/gthribieyi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xuanzx.com/gtecqygltx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xylfe.cn/gtcjkribdu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.iojbl.cn/gthkxrlzfr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.svipenyu.cn/gtvwbkkcvx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgufenzy.top/gtnzqzrsqe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258.top/gtowftlovh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.dashuyun.cn/gthnpfzoeq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sufxvd.cn/gtotwkdfbj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhaomingkeji.xyz/gtlziydimx.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtbqtiizom.html

O. 并发与异步
来源：http://hz.wangshuangyany.cn/gtgiatutnb.html

================================================================================
来源：http://hz.tanke756.top/gtfyxjqulf.html

[O01] 启动一个线程
来源：http://hz.ybcxt.top/gtbeppstux.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.c1oappe.top/gtwkrfsfdj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yangfankeji.com/gtvowdnbul.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.haohaochexian.top/gtchdkaipu.html

TS:   // 同 JS
来源：http://hz.yj20258.top/gtfcqlwdvp.html

Java: new Thread(() -> f()).start()
来源：http://hz.iojbl.cn/gtkwvbxkwe.html

Go:   go f()
来源：http://hz.zhoulong.xyz/gtzxupkwqd.html

Ruby: Thread.new { f }
来源：http://hz.cashguo.top/gtihvkstci.html

C#:   Task.Run(() => F());
来源：http://hz.yj202588.top/gthqlfrbwj.html

[O02] 使用线程池
来源：http://hz.yueranfly.top/gtfaoikcxj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.chenjidiqi.icu/gtskdmmrwi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yj20258888.top/gtpizssloq.html

JS:   // worker_threads 线程池
来源：http://hz.zhixingplan.top/gttfokqeta.html

TS:   // worker_threads 线程池
来源：http://hz.ehwqpu.com/gtojievqic.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.bjfxy.top/gtdhozykzm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cqqwz.cn/gtfxmqoudn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shanyushiyangtech.top/gtkgeygput.html


<!-- 参考信息 -->