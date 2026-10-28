代发 wailian999

[K06] 解析 URL 查询串
来源：http://hz.nanxinkj.top/gtyrtmttzu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yj20258.top/gtefqsnmqy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nanxuanxn.top/gtztmtfono.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daxiang520.top/gtkjihvcui.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cashguo.top/gtlnaysfmm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.316326.xyz/gtqxrrecrb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cucudq.cn/gtqjbljzro.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yj20258888.top/gtvgigoqnr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ehwqpu.com/gtmxzgalab.html

[K07] 进制转换
来源：http://hz.yonumen.top/gtjlwqcqui.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinqigfzy.top/gtvhhbkoqg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.nanxuanxn.top/gtwvjplbms.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtogegdqqa.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.meibo888.top/gtinzperks.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtffzmpsga.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ydzc1.top/gtwklndrza.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yvedp.cn/gtwvfcvwdq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj20258888.top/gtkvygvoxl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.c1oappe.top/gtxtfnhick.html

Py:   pickle.dumps(obj)
来源：http://hz.9152youxi.cn/gtrnikybdj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.dashuyun.cn/gtkxckgpop.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinghuilouyu.cn/gtmsvaxvuf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ydjk.org.cn/gtvvbhqbzo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hfpthk.cn/gtcvqqgina.html

Go:   encoding/gob
来源：http://hz.jinghuilouyu.cn/gtrvluosnj.html

Ruby: Marshal.dump(obj)
来源：http://hz.daria6918.cn/gtkqdzbixt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sysykeji.top/gtbhsqhllq.html

================================================================================
来源：http://hz.aibaodan.cn/gtfbrutcan.html

L. 网络请求
来源：http://hz.vqdsnc.cn/gttmgdzjpy.html

================================================================================
来源：http://hz.cashguo.top/gtnfjnbyvv.html

[L01] 发送 GET 请求
来源：http://hz.tanke756.top/gtdnodqumq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.haohaochexian.top/gtcqtulorl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.guannengcc.top/gtoquzatdx.html

JS:   await fetch(url)
来源：http://hz.gzhubu.top/gtzwjezhwb.html

TS:   await fetch(url)
来源：http://hz.xinyue.icu/gtunckzjgx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ydjk.org.cn/gthuuawwrw.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhixingplan.top/gtdzkkqndn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cdnleiting.top/gtuvmxkwmu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.aizwys.cn/gtuftlryty.html

[L02] 发送 POST JSON
来源：http://hz.9152youxi.cn/gtwlvkkyke.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.daria6918.cn/gtgqnrepjo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.daria6918.cn/gtfaxnmuza.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tanke756.top/gtwfejwpkb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuanzx.com/gtaibggdfe.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ydzc1.top/gtvbrbysoy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhoulong.xyz/gthoeezlnk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shuidangran.top/gtgevfzfrx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.andypj.xyz/gtiikuxjih.html

[L03] 设置自定义请求头
来源：http://hz.ydzc1.top/gtoovelcqp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nanxinkj.top/gtdzpxdhpj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hywenlv.cn/gtewyuqnhp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ehwqpu.com/gtyfrvoocv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sysykeji.top/gteetpycxb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ivvv.top/gtzkwumhjf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.316326.xyz/gtwsfzxbeh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yangfankeji.com/gtudxllrkm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shzxlz.cn/gtkldlxsjb.html

[L04] 设置超时
来源：http://hz.dianchejie.cn/gthciqcpyj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.guowangkeji.top/gtwyfphoti.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.fzhhl.top/gtlpbrjzqz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dashuyun.cn/gtxbeatkza.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sufxvd.cn/gtghzibcgv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sysykeji.top/gtyagsjcbn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.fzhhl.top/gtkacgafsg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinghuilouyu.cn/gtcxyiheio.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.daxiang520.top/gtlathyzrs.html

[L05] 上传文件（multipart）
来源：http://hz.xziqi.cn/gttvmraajn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.0kj1m.cn/gtensopfmc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.316326.xyz/gtxputasiy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.meibo888.top/gtfxbmbiwn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cheryme.top/gtbdfxmwzg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.andypj.xyz/gtoixkxqbk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shzxlz.cn/gtpncpaydm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shzxlz.cn/gtlwmeuvie.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenzaomai.com/gthwupjqik.html

[L06] 解析响应为 JSON
来源：http://hz.dianchejie.cn/gtumhpajyj.html

Py:   resp.json()
来源：http://hz.jlsjyb.cn/gtldcccoah.html

PHP:  json_decode($body, true);
来源：http://hz.nwbrower.top/gtgflcrlfo.html

JS:   await resp.json()
来源：http://hz.ppjwa.cn/gttrrvgpdf.html

TS:   await resp.json()
来源：http://hz.yj202588.top/gtmpxflikg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xinyue.icu/gtjagjmjmp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.snrcjt.cn/gtyuxtxtfn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sweek.top/gtasumluaj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cheryme.top/gtnelrorns.html

[L07] 处理 HTTP 状态码
来源：http://hz.jqgfzy.top/gtfhywcrsq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jlsjyb.cn/gtevwqyqul.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jlsjyb.cn/gtawshmquz.html

JS:   resp.ok;  resp.status
来源：http://hz.sysykeji.top/gtbikiptlq.html

TS:   resp.ok;  resp.status
来源：http://hz.iojbl.cn/gteporqsgd.html

Java: resp.statusCode()
来源：http://hz.ywan-chungtsiang.top/gtjinohrrh.html

Go:   resp.StatusCode
来源：http://hz.birdmap.top/gtcrvdmszb.html

Ruby: resp.code.to_i
来源：http://hz.pengpengdd.cyou/gtmyslukoi.html

C#:   (int)resp.StatusCode
来源：http://hz.fzhhl.top/gtysanwxqs.html

[L08] 并发请求多个地址
来源：http://hz.fzhhl.top/gtihryzzen.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ydzc1.top/gtyenqmivr.html

PHP:  curl_multi_init() 系列
来源：http://hz.yonumen.top/gtsxllyvcn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangtech.top/gtvcxeuwjz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pengpengdd.cyou/gtxhlyibqu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.chenlongwang.top/gtfhevmxio.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shangyingyoupin.top/gtftvkzapm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.fzhhl.top/gtxoyryqlb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yuanzhike.top/gtdjsojnuy.html

================================================================================
来源：http://hz.chenlongwang.top/gtfljbcjsa.html

M. 命令行 / 进程 / 环境
来源：http://hz.hywenlv.cn/gtwaizlpfj.html

================================================================================
来源：http://hz.cheryme.top/gtbzkapysv.html

[M01] 读取命令行参数
来源：http://hz.gzhubu.top/gteigmkvld.html

Py:   sys.argv[1:]
来源：http://hz.cashguo.top/gtohbmcypj.html

PHP:  $argv;  $argc;
来源：http://hz.guowangkeji.top/gtdzcxufre.html

JS:   process.argv.slice(2)
来源：http://hz.xylfe.cn/gtprlciojy.html

TS:   process.argv.slice(2)
来源：http://hz.kuanghao11.cn/gtqlnhspaj.html

Java: args 数组（main 方法参数）
来源：http://hz.jinyuanbaomall.cn/gtptkvdzse.html

Go:   os.Args[1:]
来源：http://hz.snrcjt.cn/gtxklitckg.html

Ruby: ARGV
来源：http://hz.yonumen.top/gtucltffjv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinqigfzy.top/gtrkkaklsm.html

[M02] 读取环境变量
来源：http://hz.nwbrower.top/gtfeqislfy.html

Py:   os.environ.get("HOME")
来源：http://hz.nanxuanxn.top/gtwlvnqgbt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ehwqpu.com/gtllweepow.html

JS:   process.env.HOME
来源：http://hz.pycfn.com/gtlnkbcdoc.html

TS:   process.env.HOME
来源：http://hz.guannengcc.top/gtawuhkddb.html

Java: System.getenv("HOME")
来源：http://hz.fengsongda.top/gtauvfutsf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ybcxt.top/gtamxgrgjk.html

Ruby: ENV["HOME"]
来源：http://hz.c1oappe.top/gtstlinocg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hysaishi.cn/gtardztzmy.html

[M03] 执行外部命令
来源：http://hz.52xcode.cn/gtplisyaph.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.sxryk.cn/gtokctviex.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gzhubu.top/gteerptftv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.guannengcc.top/gtzmnkofum.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhixingplan.top/gtxacfgeca.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.316326.xyz/gtezzaysjq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sysykeji.top/gtydzavzbg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.0kj1m.cn/gtxyddczjg.html

C#:   Process.Start("ls", "-l");
来源：http://hz.haohaochexian.top/gtzdjcdpue.html

[M04] 获取当前工作目录
来源：http://hz.smart0.xyz/gtycaphmjp.html

Py:   os.getcwd()
来源：http://hz.zhaomingkeji.xyz/gtgcxwhtxc.html

PHP:  getcwd();
来源：http://hz.zhoulong.xyz/gtpcoivswb.html

JS:   process.cwd()
来源：http://hz.sysykeji.top/gtdpezwwsd.html

TS:   process.cwd()
来源：http://hz.jinqigfzy.top/gtrdddmurc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ivvv.top/gtmqyjfuha.html

Go:   os.Getwd()
来源：http://hz.ydzc1.top/gtplxkfrqd.html

Ruby: Dir.pwd
来源：http://hz.zhengqikj.top/gtyglhjqay.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shzxlz.cn/gttbuwckbs.html

[M05] 设置退出码
来源：http://hz.iojbl.cn/gtcepwtord.html

Py:   sys.exit(1)
来源：http://hz.hysaishi.cn/gtusvwqpis.html

PHP:  exit(1);
来源：http://hz.jinghuilouyu.cn/gtrciinktx.html

JS:   process.exit(1)
来源：http://hz.shanyushiyangtech.top/gtgjyplfxn.html

TS:   process.exit(1)
来源：http://hz.vqdsnc.cn/gtebaxpufj.html

Java: System.exit(1)
来源：http://hz.ybcxt.top/gtokzhkzoy.html

Go:   os.Exit(1)
来源：http://hz.sysykeji.top/gtiscwqasl.html

Ruby: exit 1
来源：http://hz.yj202588.top/gtxicvvkkx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.svipenyu.cn/gtwaafsvco.html

[M06] 向标准错误输出
来源：http://hz.andypj.xyz/gtvgxrtkde.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sysykeji.top/gtvwejdgtq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gaohongyu789.top/gtqwlzuwws.html

JS:   console.error("err")
来源：http://hz.cucudq.cn/gtnlipipua.html

TS:   console.error("err")
来源：http://hz.aizwys.cn/gtoyaihrer.html

Java: System.err.println("err")
来源：http://hz.zhiwuduotai.top/gtdfgjpyys.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.fengsongda.top/gtthpyiiam.html

Ruby: warn "err"
来源：http://hz.svipenyu.cn/gtcauyqobl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cdnleiting.top/gtsfygxwdv.html

[M07] 判断是否为主入口
来源：http://hz.quarkkingdee.top/gticeitgwb.html

Py:   if __name__ == "__main__":
来源：http://hz.ybcxt.top/gtzxpfgcwl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.quarkkingdee.top/gtkpmrijlp.html

JS:   require.main === module
来源：http://hz.bjfxy.top/gtsvlwxsub.html

TS:   require.main === module
来源：http://hz.zhiwuduotai.top/gtijkyvrcd.html

Java: public static void main(String[] args)
来源：http://hz.ybcxt.top/gtditgzntt.html

Go:   func main()
来源：http://hz.yangfankeji.com/gtrecamseu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hfpthk.cn/gtvnkubfjb.html

C#:   static void Main(string[] args)
来源：http://hz.bjfxy.top/gtpbwkvxvf.html

[M08] 获取系统与运行时信息
来源：http://hz.xinyue.icu/gtxgxvdytn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yangfankeji.com/gtomncfzar.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xingfuxueyuan.xyz/gtcfwbdyep.html

JS:   process.platform;  process.version
来源：http://hz.xuetiantiany.cn/gtkvqnvltq.html

TS:   process.platform;  process.version
来源：http://hz.chenlongwang.top/gtfkwoueiv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ywan-chungtsiang.top/gtiyapsbhr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.pengpengdd.cyou/gtbtddwoyb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.havefunace.top/gtlgfuymfe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.chenlongwang.top/gtppzbazax.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtlxscuzof.html

N. 数据结构与算法
来源：http://hz.sufxvd.cn/gtfvrhwais.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtiwewzlyf.html

[N01] 二分查找（有序数组）
来源：http://hz.ivvv.top/gtcodrnpic.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nanxuanxn.top/gtanezcdti.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shanyushiyangtech.top/gtmawsstoi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuetiantiany.cn/gtmoghszxa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yuxming.cn/gtzxwkvlob.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hammf.cn/gtzqszcyom.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yonumen.top/gtkrfwmelf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.smart0.xyz/gthwichyzn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ybcxt.top/gtyvfmalbm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.haohaochexian.top/gteoffnvjx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinghuilouyu.cn/gtajjxcand.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cashguo.top/gtgaelaplp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtfuwqmdsu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gtppudilxu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhixingplan.top/gtijfwqgjx.html

Go:   slices.Sort(arr)
来源：http://hz.hywenlv.cn/gtmkdskzkf.html

Ruby: arr.sort
来源：http://hz.chenjidiqi.icu/gtusvylbzx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hnqzz.top/gttgpkjeor.html

[N03] 快速排序（分治示例）
来源：http://hz.jyoumei.cn/gtecwmbpln.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.daria6918.cn/gtvicgvdmj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yonumen.top/gtnhqwdygh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yongpay.top/gtkqtuhgvo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sysykeji.top/gtpwqbetcf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinyuanbaomall.cn/gtljonypgx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhijiandao.cn/gtsdccijjd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shangyingyoupin.top/gtlpchdvkf.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.52xcode.cn/gtriisltkv.html

[N04] 斐波那契数列
来源：http://hz.yuanzhike.top/gtydwvmgzr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.wangdashe.top/gtuknynmbl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.wangdashe.top/gtkllykgue.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenzaomai.com/gtnfxagufm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fengsongda.top/gtfaygsnkw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xuetiantiany.cn/gtixjpmbik.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.daxiang520.top/gtcmjmaomo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.chenjidiqi.icu/gtcmmexcxi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.52xcode.cn/gtteqpxgrf.html

[N05] 最大公约数
来源：http://hz.yj202588.top/gtttfucitv.html

Py:   math.gcd(a, b)
来源：http://hz.svipenyu.cn/gtqpsigfwc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jlsjyb.cn/gtmegakmtn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xingfuxueyuan.xyz/gtrwaigmsb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zycfv.cn/gtmxnwzpej.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.daxiang520.top/gtsdlvbwqi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yuanzhike.top/gtvsrotbxu.html

Ruby: a.gcd(b)
来源：http://hz.sufxvd.cn/gtzgddsoem.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shangyingyoupin.top/gtptwfegln.html

[N06] 判断回文字符串
来源：http://hz.yangfankeji.com/gtugfddxig.html

Py:   s == s[::-1]
来源：http://hz.hnxiangtu.top/gtkvpdvdth.html

PHP:  $s === strrev($s);
来源：http://hz.fengsongda.top/gtggvpwefy.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yonumen.top/gtywocuuog.html

TS:   s === [...s].reverse().join("")
来源：http://hz.haohaochexian.top/gtpdbyvroa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.wangdashe.top/gtgxnkswaw.html

Go:   // 双指针从两端比较
来源：http://hz.hammf.cn/gtkooourvp.html

Ruby: s == s.reverse
来源：http://hz.ppjwa.cn/gtzujjjdmm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hywenlv.cn/gtqhavswyf.html

[N07] 两数之和（返回下标）
来源：http://hz.zhiwuduotai.top/gtglmwpajz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhijiandao.cn/gtlmikkwfd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.9152youxi.cn/gtfdcohxho.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jiagoushi.top/gtaweqrqik.html

TS:   // 手写 Map<string, number>
来源：http://hz.daxiang520.top/gthdrqcsih.html

Java: // 手写 HashMap
来源：http://hz.zhongyouzk.top/gtclrqyfdk.html

Go:   // 手写 map[int]int
来源：http://hz.ybcxt.top/gtsuhafdks.html

Ruby: // 手写 Hash
来源：http://hz.zhongyouzk.top/gtbczpolfn.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jqgufenzy.top/gtkmmqjlvw.html

[N08] 生成全排列
来源：http://hz.ivvv.top/gtloakvaln.html

Py:   itertools.permutations(arr)
来源：http://hz.chenjidiqi.icu/gtudmqhyly.html

PHP:  // 手写递归交换
来源：http://hz.gotoacloud.top/gtdsyotuev.html

JS:   // 手写回溯递归
来源：http://hz.sysykeji.top/gtclukvhoe.html

TS:   // 手写回溯递归
来源：http://hz.snrcjt.cn/gthbvrzfvz.html

Java: // 手写回溯递归
来源：http://hz.yueranfly.top/gthfaybcvv.html

Go:   // 手写回溯递归
来源：http://hz.vqdsnc.cn/gteifqqtme.html

Ruby: arr.permutation.to_a
来源：http://hz.bjfxy.top/gtmdnyqzqx.html

C#:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtyhdazsfk.html

[N09] 栈与队列
来源：http://hz.zhijiandao.cn/gtzmmomrox.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ydjk.org.cn/gtvebocqdc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cdnleiting.top/gtixtqzgof.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhengqikj.top/gtzbkbfgws.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhixingplan.top/gtooehrqou.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hnqzz.top/gtsybgseup.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.quarkkingdee.top/gtumqwptii.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.wangdashe.top/gtxetfxmfc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cucudq.cn/gtwvctuhlt.html

[N10] 链表节点定义
来源：http://hz.fzhhl.top/gtxwinkpfs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shangyingyoupin.top/gtmsyzqqwb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hongshengwenyu.top/gtqcmbzvzd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.shzxlz.cn/gtgtlspypa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jinqigufen.top/gtgiqnkdhe.html

Java: class Node { int v; Node next; }
来源：http://hz.jianghu66.top/gtusentmgy.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xuanzx.com/gtunqqssmt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zdqjudy.top/gtpxvmfzkf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yongpay.top/gtifscqurf.html

[N11] 二叉树中序遍历
来源：http://hz.ydjk.org.cn/gtvkbntpcf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinqigufen.top/gtnwdtcajz.html

PHP:  // 手写递归函数
来源：http://hz.wangdashe.top/gtyupqvtyp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgfzy.top/gtbaijavuj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gotoacloud.top/gtvzlapaxy.html

Java: // 手写递归
来源：http://hz.sxryk.cn/gtzgqvybmx.html

Go:   // 手写递归
来源：http://hz.jyoumei.cn/gtglqycbst.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhengqikj.top/gtbknloakc.html

C#:   // 手写递归
来源：http://hz.ehwqpu.com/gtayojiksf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yanxiufei.cn/gtbklpnard.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinyuanbaomall.cn/gtzbypmzoz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yueranfly.top/gtwpuosbka.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxinkj.top/gtwuyztkmm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtlzaoohbs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinghuilouyu.cn/gtwntduzdt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.tianlin.xyz/gtmkphqmgh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.c1oappe.top/gtxqjdkpel.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhongyouzk.top/gtibaydqrx.html

================================================================================
来源：http://hz.vqdsnc.cn/gtfimugjsz.html

O. 并发与异步
来源：http://hz.daria6918.cn/gtrhcknemh.html

================================================================================
来源：http://hz.9152youxi.cn/gtkvbvcavq.html

[O01] 启动一个线程
来源：http://hz.316326.xyz/gtjydsxrqb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gzhubu.top/gtpwdgjadv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.316326.xyz/gtcollabbl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yongpay.top/gthrrecadv.html

TS:   // 同 JS
来源：http://hz.quarkkingdee.top/gtwqwoaqxm.html

Java: new Thread(() -> f()).start()
来源：http://hz.hywenlv.cn/gtwcqryxwv.html

Go:   go f()
来源：http://hz.redwolf501.top/gtilpgouaz.html

Ruby: Thread.new { f }
来源：http://hz.zhaomingkeji.xyz/gtgazdfnfv.html

C#:   Task.Run(() => F());
来源：http://hz.chenzaomai.com/gtcynelwvo.html


<!-- 参考信息 -->