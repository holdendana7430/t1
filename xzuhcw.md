代发 wailian999

[K06] 解析 URL 查询串
来源：http://hz.yangfankeji.com/gtakqyagoy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sysykeji.top/gtowdfsnad.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.chenlongwang.top/gtsgajmxbc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.feifeiyinyue.top/gtakonqjvv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.haohaochexian.top/gtupdheant.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.fengsongda.top/gtqgmrnlal.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hnqzz.top/gtjuyainxm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.bjfxy.top/gtwjgndeeu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhijiandao.cn/gtaeptjxio.html

[K07] 进制转换
来源：http://hz.yongpay.top/gthekvzzua.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhengqikj.top/gtewmzxcos.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xuetiantiany.cn/gtmsodkebl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yueranfly.top/gtyanvsfdl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yvedp.cn/gtekchlgpp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cashguo.top/gtvwfzoyoc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jianghu66.top/gtxscfiktu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.daria6918.cn/gtgtnepaqj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hongshengwenyu.top/gtmmzchzmz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.dianchejie.cn/gtefwjvxeq.html

Py:   pickle.dumps(obj)
来源：http://hz.cheryme.top/gtdvwynvty.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinqigfzy.top/gtkrgbwezu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenjidiqi.icu/gtgfgjrhaj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.sufxvd.cn/gtpfunlxuu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yongpay.top/gtuycfprrb.html

Go:   encoding/gob
来源：http://hz.zhijiandao.cn/gtpjretfwd.html

Ruby: Marshal.dump(obj)
来源：http://hz.redwolf501.top/gtgfaohprm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.dashuyun.cn/gtghmidmng.html

================================================================================
来源：http://hz.c1oappe.top/gttjnknrsz.html

L. 网络请求
来源：http://hz.jinqigfzy.top/gtnzlxlwvo.html

================================================================================
来源：http://hz.ybcxt.top/gtlrjayviu.html

[L01] 发送 GET 请求
来源：http://hz.hammf.cn/gtxdsdfiur.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.quarkkingdee.top/gtyklvgynf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.bjfxy.top/gticpouupr.html

JS:   await fetch(url)
来源：http://hz.yj20258888.top/gtfjrkvqwi.html

TS:   await fetch(url)
来源：http://hz.hnxiangtu.top/gtskaehkkc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sweek.top/gtldovezag.html

Go:   resp, err := http.Get(url)
来源：http://hz.hnqzz.top/gtvhavurub.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.fzhhl.top/gtjulrlrug.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.mhx1999.top/gttudgnowf.html

[L02] 发送 POST JSON
来源：http://hz.jinghuilouyu.cn/gtfefakiaw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jinyuanbaomall.cn/gtraobzasp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jianghu66.top/gtvzgarckm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.iojbl.cn/gtmnbfnrut.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ppjwa.cn/gtpzwjstrx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yangfankeji.com/gtbqmqwhdm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xuanzx.com/gtrqyzlkyv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sxryk.cn/gtifrhzxrx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.havefunace.top/gtyroixuos.html

[L03] 设置自定义请求头
来源：http://hz.ybcxt.top/gtsvrddhqb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nanxinkj.top/gtvjmudqzn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gaohongyu789.top/gtynxlfprm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.andypj.xyz/gttpdfxsxq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fzhhl.top/gtbnfbhemk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xziqi.cn/gtlolxqmbg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.nanxinkj.top/gtoynbqgua.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.aizwys.cn/gtygbywvku.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.quarkkingdee.top/gtwisormhg.html

[L04] 设置超时
来源：http://hz.c1oappe.top/gtnexpzhgw.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hfpthk.cn/gtbldjnykj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.fengsongda.top/gtqwbekpjw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.birdmap.top/gtvurtkoqs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhengqikj.top/gttysbjqce.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.nwbrower.top/gtmxibgwss.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yanxiufei.cn/gtagsvuqbo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.kuanghao11.cn/gtmemgaier.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yongpay.top/gthqzkqrbq.html

[L05] 上传文件（multipart）
来源：http://hz.9152youxi.cn/gtsecnbvsq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.kuanghao11.cn/gtceryvyhk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yj202588.top/gtkybisizb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgufenzy.top/gtyctqexqj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xziqi.cn/gtaltcklwc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.mhx1999.top/gtcriljzbl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sweek.top/gtklphnjtf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinyuanbaomall.cn/gtpoppemfs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yonumen.top/gtjpvoeupj.html

[L06] 解析响应为 JSON
来源：http://hz.cheryme.top/gtjyvayfjr.html

Py:   resp.json()
来源：http://hz.zhijiandao.cn/gtnincprve.html

PHP:  json_decode($body, true);
来源：http://hz.0kj1m.cn/gtuwqnxcox.html

JS:   await resp.json()
来源：http://hz.daria6918.cn/gtiyhynibq.html

TS:   await resp.json()
来源：http://hz.jinghuilouyu.cn/gttxllevkd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gogol.net.cn/gtgozkgxsm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.smart0.xyz/gtnbwfzxty.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hammf.cn/gtulkjiagc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hnxiangtu.top/gtvbbirgtd.html

[L07] 处理 HTTP 状态码
来源：http://hz.hysaishi.cn/gtjpgnueph.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hnqzz.top/gtrvvxrhzg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cashguo.top/gtjjqocqrz.html

JS:   resp.ok;  resp.status
来源：http://hz.sweek.top/gtehaldiej.html

TS:   resp.ok;  resp.status
来源：http://hz.meibo888.top/gtpytfgfxv.html

Java: resp.statusCode()
来源：http://hz.hysaishi.cn/gtltupuxnr.html

Go:   resp.StatusCode
来源：http://hz.yj202588.top/gtswjgaxnr.html

Ruby: resp.code.to_i
来源：http://hz.mhx1999.top/gtainvzviu.html

C#:   (int)resp.StatusCode
来源：http://hz.shzxlz.cn/gtsznewrkj.html

[L08] 并发请求多个地址
来源：http://hz.hysaishi.cn/gtvfdahmqi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhiwuduotai.top/gtxwsepbvk.html

PHP:  curl_multi_init() 系列
来源：http://hz.sxryk.cn/gthpiojkbd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gtsnniuxka.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gzhubu.top/gtidtaciyh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinghuilouyu.cn/gtdqmmdkrq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.smart0.xyz/gtgkbnkjlo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.haohaochexian.top/gtjqbhtlzw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hongshengwenyu.top/gtgshprkxl.html

================================================================================
来源：http://hz.shuidangran.top/gtwcmvtqeq.html

M. 命令行 / 进程 / 环境
来源：http://hz.hywenlv.cn/gtowzzmtsv.html

================================================================================
来源：http://hz.cdnleiting.top/gtpdpjhedb.html

[M01] 读取命令行参数
来源：http://hz.zhixingplan.top/gthjkcnush.html

Py:   sys.argv[1:]
来源：http://hz.sweek.top/gtuyaikswu.html

PHP:  $argv;  $argc;
来源：http://hz.zhongyouzk.top/gtecvaqqyt.html

JS:   process.argv.slice(2)
来源：http://hz.haohaochexian.top/gtmqhsnmtm.html

TS:   process.argv.slice(2)
来源：http://hz.daxiang520.top/gtkzdcjoqg.html

Java: args 数组（main 方法参数）
来源：http://hz.wangshuangyany.cn/gtuajzgxdy.html

Go:   os.Args[1:]
来源：http://hz.ydjk.org.cn/gtispiubkb.html

Ruby: ARGV
来源：http://hz.wangdashe.top/gtjnbpjdfc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.guowangkeji.top/gtcxxkqoxr.html

[M02] 读取环境变量
来源：http://hz.vqdsnc.cn/gtjsvghvjd.html

Py:   os.environ.get("HOME")
来源：http://hz.0kj1m.cn/gtqmdpsica.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sweek.top/gtojjvxelm.html

JS:   process.env.HOME
来源：http://hz.dashuyun.cn/gteuxlzwef.html

TS:   process.env.HOME
来源：http://hz.hongshengwenyu.top/gtmzxbiywk.html

Java: System.getenv("HOME")
来源：http://hz.yj202588.top/gtgwurztos.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xuanzx.com/gtbluivyhw.html

Ruby: ENV["HOME"]
来源：http://hz.cqqwz.cn/gtueafuicf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yangfankeji.com/gtjcyenyfj.html

[M03] 执行外部命令
来源：http://hz.aizwys.cn/gtlksactnk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yueranfly.top/gterjlcyfp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sufxvd.cn/gtcyiblcqy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.nanxinkj.top/gtmlvmelte.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.snrcjt.cn/gtrvltrliy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.wangdashe.top/gtnzoxdjeb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.quarkkingdee.top/gtvtaouhek.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yj202588.top/gtqoxgcinu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cdnleiting.top/gtvhpcdsgm.html

[M04] 获取当前工作目录
来源：http://hz.zdqjudy.top/gtvjbckoyh.html

Py:   os.getcwd()
来源：http://hz.cqqwz.cn/gtrqavjpgd.html

PHP:  getcwd();
来源：http://hz.9152youxi.cn/gtnpoyibzq.html

JS:   process.cwd()
来源：http://hz.ybcxt.top/gtmtpchfoe.html

TS:   process.cwd()
来源：http://hz.yj20258.top/gtdvhadurr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gzhubu.top/gtrvvsmjav.html

Go:   os.Getwd()
来源：http://hz.sufxvd.cn/gtglsqkdpo.html

Ruby: Dir.pwd
来源：http://hz.nwbrower.top/gtdmcjusfy.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yonumen.top/gtupavbjyg.html

[M05] 设置退出码
来源：http://hz.sxryk.cn/gtaqtzfywc.html

Py:   sys.exit(1)
来源：http://hz.guowangkeji.top/gtfwgbkyhb.html

PHP:  exit(1);
来源：http://hz.hfpthk.cn/gthfdzxvqc.html

JS:   process.exit(1)
来源：http://hz.hammf.cn/gtxubrhvxt.html

TS:   process.exit(1)
来源：http://hz.hammf.cn/gtgviwjcdi.html

Java: System.exit(1)
来源：http://hz.mhx1999.top/gtkxayqebu.html

Go:   os.Exit(1)
来源：http://hz.cheryme.top/gtetibkqbm.html

Ruby: exit 1
来源：http://hz.chenzaomai.com/gtdkvzntfl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nwbrower.top/gtfayecebd.html

[M06] 向标准错误输出
来源：http://hz.ydzc1.top/gtgtcqojfj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.daxiang520.top/gtxupqfbig.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sweek.top/gtoxfdukjz.html

JS:   console.error("err")
来源：http://hz.jqgufenzy.top/gtgjaodcfg.html

TS:   console.error("err")
来源：http://hz.xingfuxueyuan.xyz/gticnzbtmv.html

Java: System.err.println("err")
来源：http://hz.shanyushiyangtech.top/gtpswuxenu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cqqwz.cn/gtqiwjiurb.html

Ruby: warn "err"
来源：http://hz.shanyushiyangtech.top/gthdlypvka.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.pycfn.com/gtachlekro.html

[M07] 判断是否为主入口
来源：http://hz.kuanghao11.cn/gtrnoukjoc.html

Py:   if __name__ == "__main__":
来源：http://hz.cucudq.cn/gtwmrjuhho.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cheryme.top/gtxjykyjkd.html

JS:   require.main === module
来源：http://hz.jlsjyb.cn/gtnmbbciym.html

TS:   require.main === module
来源：http://hz.jinqigfzy.top/gtvxvjddpu.html

Java: public static void main(String[] args)
来源：http://hz.guannengcc.top/gtkcmnbagf.html

Go:   func main()
来源：http://hz.xziqi.cn/gtltcusqbe.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hongshengwenyu.top/gtszhzorbm.html

C#:   static void Main(string[] args)
来源：http://hz.9152youxi.cn/gtuwipcqxm.html

[M08] 获取系统与运行时信息
来源：http://hz.ybcxt.top/gtyfshildh.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jlsjyb.cn/gtnehboill.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hnqzz.top/gtondumhef.html

JS:   process.platform;  process.version
来源：http://hz.daxiang520.top/gtiocrwgow.html

TS:   process.platform;  process.version
来源：http://hz.yj202588.top/gteuovkgpt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sysykeji.top/gtolmizvve.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xuanzx.com/gteqhsawcy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinqigufen.top/gtzykdyfiv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hysaishi.cn/gtjgibkvqw.html

================================================================================
来源：http://hz.sxryk.cn/gtjdprspro.html

N. 数据结构与算法
来源：http://hz.meibo888.top/gtlsqmwwau.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtunsgdxlv.html

[N01] 二分查找（有序数组）
来源：http://hz.c1oappe.top/gtxqwvtlum.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhijiandao.cn/gthcyjgmjy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cucudq.cn/gtldvaosuc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydzc1.top/gtmfxfkken.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gzhubu.top/gtfsqrfvix.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.snrcjt.cn/gtqplgorcv.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenzaomai.com/gtjajaqhxe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yonumen.top/gtxhcupdvm.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nanxuanxn.top/gtssfmyjyk.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yuanzhike.top/gtwaejoftl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.andypj.xyz/gtbrbayske.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinqigufen.top/gtymmpsyvj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jqgufenzy.top/gtpbbpomff.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj202588.top/gtymjqgmxu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cdnleiting.top/gtrglyoulh.html

Go:   slices.Sort(arr)
来源：http://hz.shangyingyoupin.top/gtmoqkabws.html

Ruby: arr.sort
来源：http://hz.chenlongwang.top/gtyyrhvjdu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xuanzx.com/gtrjkkxefz.html

[N03] 快速排序（分治示例）
来源：http://hz.guannengcc.top/gtgbqswfif.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.nwbrower.top/gtuhdsoctp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhoulong.xyz/gtpfmjqeqy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gaohongyu789.top/gtfeoggbak.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydzc1.top/gtmtnabanv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jyoumei.cn/gtaovgsxfm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhoulong.xyz/gtrhpzjhty.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.daria6918.cn/gtolbhcujl.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jqgfzy.top/gtplpzjhyl.html

[N04] 斐波那契数列
来源：http://hz.yangfankeji.com/gtzvgdsxau.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.snrcjt.cn/gtngtwuqif.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinqigufen.top/gthrvodhck.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.feifeiyinyue.top/gtcxbdtbmd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhoulong.xyz/gtblatlufg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hnxiangtu.top/gtvfogscwb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gaohongyu789.top/gthbcezuho.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinyuanbaomall.cn/gtlhdfekza.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ivvv.top/gtyanpecar.html

[N05] 最大公约数
来源：http://hz.zhongyouzk.top/gtnwrlesbr.html

Py:   math.gcd(a, b)
来源：http://hz.mhx1999.top/gtuwexkvir.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.gotoacloud.top/gtmvrgfczd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jiagoushi.top/gtlhmzaqhx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dashuyun.cn/gtxnncmibo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jinqigfzy.top/gtirffpxif.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinghuilouyu.cn/gtirxqfrek.html

Ruby: a.gcd(b)
来源：http://hz.meibo888.top/gtvteuqfvq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.bjfxy.top/gtgwhdsvty.html

[N06] 判断回文字符串
来源：http://hz.dashuyun.cn/gtfckcdjsp.html

Py:   s == s[::-1]
来源：http://hz.shuidangran.top/gtrzzqmiqa.html

PHP:  $s === strrev($s);
来源：http://hz.shanyushiyangkeji.top/gtufjubkci.html

JS:   s === [...s].reverse().join("")
来源：http://hz.wangdashe.top/gteajjnguy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.daria6918.cn/gtymzsezud.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.bjfxy.top/gtyarcbecy.html

Go:   // 双指针从两端比较
来源：http://hz.andypj.xyz/gtkuvwhojm.html

Ruby: s == s.reverse
来源：http://hz.guannengcc.top/gteyfpniqp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.dianchejie.cn/gtfjlshgze.html

[N07] 两数之和（返回下标）
来源：http://hz.iojbl.cn/gtcvndlgtj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.sufxvd.cn/gtjqbseqzt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gaohongyu789.top/gtianszedr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nwbrower.top/gthwojkcqs.html

TS:   // 手写 Map<string, number>
来源：http://hz.yueranfly.top/gtixrtdhur.html

Java: // 手写 HashMap
来源：http://hz.jiagoushi.top/gtafcohwon.html

Go:   // 手写 map[int]int
来源：http://hz.jiagoushi.top/gtmvkwncga.html

Ruby: // 手写 Hash
来源：http://hz.daxiang520.top/gtphxygkfs.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.chenlongwang.top/gtxmrsuckb.html

[N08] 生成全排列
来源：http://hz.hammf.cn/gtdbwcbphg.html

Py:   itertools.permutations(arr)
来源：http://hz.jinqigufen.top/gtuymmoipw.html

PHP:  // 手写递归交换
来源：http://hz.hnxiangtu.top/gtctybxymw.html

JS:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtejmtxsbj.html

TS:   // 手写回溯递归
来源：http://hz.sweek.top/gtnkymnnvo.html

Java: // 手写回溯递归
来源：http://hz.hfpthk.cn/gtdsmvycwo.html

Go:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gthyrteyrf.html

Ruby: arr.permutation.to_a
来源：http://hz.zhongyouzk.top/gtqotewxgv.html

C#:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtjgzmqrmg.html

[N09] 栈与队列
来源：http://hz.chenlongwang.top/gtjpmqudlq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sysykeji.top/gtwhomhgyl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hfpthk.cn/gtcdwzhdas.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.wangshuangyany.cn/gtxsrrljxz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.kuanghao11.cn/gtumvjxkud.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinqigufen.top/gtwibdjwrz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.wangdashe.top/gtrcpeftdq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jqgufenzy.top/gtzgdgdjwb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.birdmap.top/gtnypxknsj.html

[N10] 链表节点定义
来源：http://hz.pengpengdd.cyou/gtyslppruw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhengqikj.top/gtyswshvxx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yuanzhike.top/gtwrrrahct.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hnqzz.top/gthiirwwzm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sxryk.cn/gthyrdoysl.html

Java: class Node { int v; Node next; }
来源：http://hz.52xcode.cn/gtxjiefpdn.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.nwbrower.top/gtrvwnshtp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.svipenyu.cn/gtxuweusuh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jlsjyb.cn/gtvweeliml.html

[N11] 二叉树中序遍历
来源：http://hz.redwolf501.top/gtcurbbeai.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhoulong.xyz/gtpgvhkqwt.html

PHP:  // 手写递归函数
来源：http://hz.hongshengwenyu.top/gthgtgzupc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgfzy.top/gtveqaxnsy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenzaomai.com/gtkibilbxm.html

Java: // 手写递归
来源：http://hz.jinyuanbaomall.cn/gtnuqlpsin.html

Go:   // 手写递归
来源：http://hz.hammf.cn/gtxzqavcdb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shzxlz.cn/gtovxcmzrz.html

C#:   // 手写递归
来源：http://hz.ehwqpu.com/gtnnegmnff.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xziqi.cn/gtfaceqjqr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.feifeiyinyue.top/gttubpckvb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.pengpengdd.cyou/gtdnrhrnxk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cdnleiting.top/gthiiserxf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.redwolf501.top/gtseschgtu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jiagoushi.top/gtznqfyztf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hysaishi.cn/gtlfszxexu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.wangshuangyany.cn/gtrgvwlwja.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.feifeiyinyue.top/gtvixgqxib.html

================================================================================
来源：http://hz.andypj.xyz/gtiksoptrt.html

O. 并发与异步
来源：http://hz.shuidangran.top/gtiaungfre.html

================================================================================
来源：http://hz.tianlin.xyz/gtyydzsisv.html

[O01] 启动一个线程
来源：http://hz.zhaomingkeji.xyz/gtyewkbafm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ehwqpu.com/gtzobzpeeq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhixingplan.top/gtpnfbgxld.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ywan-chungtsiang.top/gtkxnhngcx.html

TS:   // 同 JS
来源：http://hz.guowangkeji.top/gtdrlahawf.html

Java: new Thread(() -> f()).start()
来源：http://hz.zycfv.cn/gtpaobhojh.html

Go:   go f()
来源：http://hz.yonumen.top/gtnrjusedl.html

Ruby: Thread.new { f }
来源：http://hz.svipenyu.cn/gtwuppmmva.html

C#:   Task.Run(() => F());
来源：http://hz.gotoacloud.top/gtwhldiqhw.html


<!-- 参考信息 -->