代发 wailian999

[K06] 解析 URL 查询串
来源：http://hz.gaohongyu789.top/gtrobxnxgd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yuanzhike.top/gtknrrgcpn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.chenjidiqi.icu/gtjtwvziga.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.havefunace.top/gtjtqvpbkb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenlongwang.top/gtsbwylsxv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.9152youxi.cn/gtxvbqyknh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hammf.cn/gtdlhlhogj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hysaishi.cn/gtkhjokaut.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.52xcode.cn/gtqyqzrzqm.html

[K07] 进制转换
来源：http://hz.birdmap.top/gtlfbgeubu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cucudq.cn/gtsumpqizn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hongshengwenyu.top/gtlsekccpz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.9152youxi.cn/gtjrdogshn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jyoumei.cn/gtdeeqcklx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gttjudspqr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.svipenyu.cn/gtcxuezxjm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.smart0.xyz/gtjlbvwyvg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.guowangkeji.top/gtslqeipmr.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ybcxt.top/gtccwoyond.html

Py:   pickle.dumps(obj)
来源：http://hz.yuanzhike.top/gtgrpvxjsl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xylfe.cn/gturoqzxvx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cdnleiting.top/gtrvxhbmcq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yongpay.top/gtqnwtsmki.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.fengsongda.top/gtgdfvmonv.html

Go:   encoding/gob
来源：http://hz.316326.xyz/gtlmkblbdz.html

Ruby: Marshal.dump(obj)
来源：http://hz.cheryme.top/gtbevsjlny.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hnqzz.top/gtgbkedshm.html

================================================================================
来源：http://hz.hfpthk.cn/gtmvmwwfpl.html

L. 网络请求
来源：http://hz.zhixingplan.top/gtnpvtpqop.html

================================================================================
来源：http://hz.nanxuanxn.top/gtehmvnghr.html

[L01] 发送 GET 请求
来源：http://hz.ivvv.top/gtoqzbbzwj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinqigfzy.top/gtrtowxzfn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sysykeji.top/gtlrywsygy.html

JS:   await fetch(url)
来源：http://hz.hfpthk.cn/gtshybzobd.html

TS:   await fetch(url)
来源：http://hz.hysaishi.cn/gtwazitqhm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.quarkkingdee.top/gtnyehzocr.html

Go:   resp, err := http.Get(url)
来源：http://hz.vqdsnc.cn/gtvzffpwfx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ydzc1.top/gthbsawmei.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.tian-w.cn/gtdskzzzvw.html

[L02] 发送 POST JSON
来源：http://hz.redwolf501.top/gtjhipgceb.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guannengcc.top/gtuubjuzcj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhaomingkeji.xyz/gtniglmusx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tanke756.top/gtgugoazqr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.kuanghao11.cn/gtwonvndlg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xinyue.icu/gtmttytuev.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shzxlz.cn/gtxuilaqse.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xingfuxueyuan.xyz/gtbjxliiru.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cqqwz.cn/gtmeaxqykf.html

[L03] 设置自定义请求头
来源：http://hz.jinghuilouyu.cn/gticvkhgtk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.aibaodan.cn/gtymomudhr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zdqjudy.top/gtxmizfkji.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.mhx1999.top/gtjornvzyv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj20258888.top/gtbwqfpkcu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sxryk.cn/gtlftjlvjp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yvedp.cn/gtnokqivzu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jqgfzy.top/gtmplvwwqm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.sufxvd.cn/gtxcnrgwxi.html

[L04] 设置超时
来源：http://hz.cashguo.top/gtqsobhkff.html

Py:   requests.get(url, timeout=5)
来源：http://hz.52xcode.cn/gtdzbofjlu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ywan-chungtsiang.top/gtyjvhqpps.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fzhhl.top/gtqqkwkoap.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shzxlz.cn/gtmolwvqpx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gzhubu.top/gteiyyqzqy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.9152youxi.cn/gtsnzvyekc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.smart0.xyz/gtmsnespid.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hfpthk.cn/gtdcaawvtd.html

[L05] 上传文件（multipart）
来源：http://hz.tanke756.top/gtytddyrck.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yuanzhike.top/gtwijgaecp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cucudq.cn/gtnejzyusj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhaomingkeji.xyz/gtcpyygfxl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yvedp.cn/gtlosjdmpl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.c1oappe.top/gtugrachpa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhiwuduotai.top/gtzyzoqwjw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xylfe.cn/gttndgvhnc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.haohaochexian.top/gtzhglowga.html

[L06] 解析响应为 JSON
来源：http://hz.havefunace.top/gteqkqdknj.html

Py:   resp.json()
来源：http://hz.yj20258.top/gtqlxkiwzk.html

PHP:  json_decode($body, true);
来源：http://hz.xinyue.icu/gtdkwmvwvp.html

JS:   await resp.json()
来源：http://hz.ydjk.org.cn/gtdjzvrqro.html

TS:   await resp.json()
来源：http://hz.aibaodan.cn/gtfxethslb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.feifeiyinyue.top/gtlqbdcgwv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.52xcode.cn/gtcwkryezy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jyoumei.cn/gthxkobulk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.havefunace.top/gtyggasgcs.html

[L07] 处理 HTTP 状态码
来源：http://hz.shuidangran.top/gtcjwynuci.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shanyushiyangtech.top/gtaxjmogkd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhijiandao.cn/gthdyilwcj.html

JS:   resp.ok;  resp.status
来源：http://hz.sysykeji.top/gtmjlxcsxa.html

TS:   resp.ok;  resp.status
来源：http://hz.xylfe.cn/gthkcseqte.html

Java: resp.statusCode()
来源：http://hz.daria6918.cn/gtyinuzfud.html

Go:   resp.StatusCode
来源：http://hz.jlsjyb.cn/gtipncdqpz.html

Ruby: resp.code.to_i
来源：http://hz.ybcxt.top/gtpyfwwmam.html

C#:   (int)resp.StatusCode
来源：http://hz.aizwys.cn/gtpdjqabyw.html

[L08] 并发请求多个地址
来源：http://hz.ppjwa.cn/gtpbgphvbm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.feifeiyinyue.top/gterrtxfjg.html

PHP:  curl_multi_init() 系列
来源：http://hz.jqgufenzy.top/gtsuboqndf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guannengcc.top/gtznmvlocn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuetiantiany.cn/gtrdawaqlu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xuetiantiany.cn/gtvhpuuxhw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zdqjudy.top/gtgmkcdltw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ehwqpu.com/gtdhbdvuiv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shuidangran.top/gthuuhnsxo.html

================================================================================
来源：http://hz.jqgfzy.top/gtlzzidanr.html

M. 命令行 / 进程 / 环境
来源：http://hz.andypj.xyz/gtpqkoyayc.html

================================================================================
来源：http://hz.birdmap.top/gtgbkimxjh.html

[M01] 读取命令行参数
来源：http://hz.zhongyouzk.top/gtbkzccfzj.html

Py:   sys.argv[1:]
来源：http://hz.yuxming.cn/gtugqsjpvm.html

PHP:  $argv;  $argc;
来源：http://hz.ivvv.top/gtguvvfiul.html

JS:   process.argv.slice(2)
来源：http://hz.aizwys.cn/gthcudjhfs.html

TS:   process.argv.slice(2)
来源：http://hz.zhoulong.xyz/gthmmbvkjk.html

Java: args 数组（main 方法参数）
来源：http://hz.yonumen.top/gtpbbucrvs.html

Go:   os.Args[1:]
来源：http://hz.tanke756.top/gtmwkhmaee.html

Ruby: ARGV
来源：http://hz.gogol.net.cn/gtffgtjlle.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shanyushiyangtech.top/gtjpfjvnxu.html

[M02] 读取环境变量
来源：http://hz.havefunace.top/gthwpgwaju.html

Py:   os.environ.get("HOME")
来源：http://hz.chenjidiqi.icu/gtyrnomdtp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sweek.top/gtbywinhqo.html

JS:   process.env.HOME
来源：http://hz.svipenyu.cn/gtyuyerizy.html

TS:   process.env.HOME
来源：http://hz.yj20258.top/gtvriszhew.html

Java: System.getenv("HOME")
来源：http://hz.chenlongwang.top/gtuyvttklt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.nanxuanxn.top/gturzkesfe.html

Ruby: ENV["HOME"]
来源：http://hz.gaohongyu789.top/gtnjxrnnqp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.svipenyu.cn/gtoovuqqbq.html

[M03] 执行外部命令
来源：http://hz.jiagoushi.top/gtcowbunzq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cdnleiting.top/gtgxkalvvk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sufxvd.cn/gtghytvdyg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhixingplan.top/gtucgqmcyy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hammf.cn/gtreyrfvus.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinqigfzy.top/gtepqxdxus.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.chenzaomai.com/gtoonbugpk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xziqi.cn/gtgypfnxll.html

C#:   Process.Start("ls", "-l");
来源：http://hz.birdmap.top/gttegfgmeb.html

[M04] 获取当前工作目录
来源：http://hz.feifeiyinyue.top/gtgiirwioa.html

Py:   os.getcwd()
来源：http://hz.ybcxt.top/gtlvsvvdmu.html

PHP:  getcwd();
来源：http://hz.shanyushiyangkeji.top/gttxaprued.html

JS:   process.cwd()
来源：http://hz.hongshengwenyu.top/gtvonpcjqm.html

TS:   process.cwd()
来源：http://hz.hfpthk.cn/gtiieacwgq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhengqikj.top/gtzfxqtwoj.html

Go:   os.Getwd()
来源：http://hz.andypj.xyz/gthpvumxqc.html

Ruby: Dir.pwd
来源：http://hz.yuxming.cn/gthqtdmcgn.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.vqdsnc.cn/gtntyeglla.html

[M05] 设置退出码
来源：http://hz.ydjk.org.cn/gtdayagtax.html

Py:   sys.exit(1)
来源：http://hz.chenzaomai.com/gtyqjygjho.html

PHP:  exit(1);
来源：http://hz.xuanzx.com/gtcvhkbeko.html

JS:   process.exit(1)
来源：http://hz.fzhhl.top/gtlucctdyw.html

TS:   process.exit(1)
来源：http://hz.zycfv.cn/gtcmgxizrd.html

Java: System.exit(1)
来源：http://hz.feifeiyinyue.top/gtwjfqgcdo.html

Go:   os.Exit(1)
来源：http://hz.sweek.top/gtmyicftme.html

Ruby: exit 1
来源：http://hz.xinyue.icu/gttmohetlw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.guannengcc.top/gtrjhhjyee.html

[M06] 向标准错误输出
来源：http://hz.xuanzx.com/gtuadbcrkl.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hnqzz.top/gteyxxnign.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenjidiqi.icu/gtgiicjuap.html

JS:   console.error("err")
来源：http://hz.wangshuangyany.cn/gtvdyvrbnv.html

TS:   console.error("err")
来源：http://hz.ywan-chungtsiang.top/gttjrmlvri.html

Java: System.err.println("err")
来源：http://hz.cheryme.top/gtrlhybnhv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.tanke756.top/gtqgphdhqy.html

Ruby: warn "err"
来源：http://hz.cdnleiting.top/gtyerhxkgy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.sxryk.cn/gtafztohyh.html

[M07] 判断是否为主入口
来源：http://hz.yongpay.top/gtfhfzohxv.html

Py:   if __name__ == "__main__":
来源：http://hz.snrcjt.cn/gtexeutonb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yvedp.cn/gtxheduiod.html

JS:   require.main === module
来源：http://hz.redwolf501.top/gtyvzziojb.html

TS:   require.main === module
来源：http://hz.nanxinkj.top/gtzyjxdumk.html

Java: public static void main(String[] args)
来源：http://hz.zdqjudy.top/gtseipabla.html

Go:   func main()
来源：http://hz.hywenlv.cn/gttvojkswj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.gogol.net.cn/gtvosnykag.html

C#:   static void Main(string[] args)
来源：http://hz.52xcode.cn/gtuezssdaj.html

[M08] 获取系统与运行时信息
来源：http://hz.ehwqpu.com/gttcuuongh.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cashguo.top/gtwzpgwqtp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jqgfzy.top/gtipbazgsp.html

JS:   process.platform;  process.version
来源：http://hz.shzxlz.cn/gtyrfqkwpm.html

TS:   process.platform;  process.version
来源：http://hz.hongshengwenyu.top/gtrofhipxz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jqgfzy.top/gtzlyuqqfz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gotoacloud.top/gttpjywjfs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinqigufen.top/gtvoiruykq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sxryk.cn/gtmmckytkc.html

================================================================================
来源：http://hz.mhx1999.top/gtxdzbkrdw.html

N. 数据结构与算法
来源：http://hz.pycfn.com/gtwamolkfz.html

================================================================================
来源：http://hz.bjfxy.top/gtmodtqrki.html

[N01] 二分查找（有序数组）
来源：http://hz.shzxlz.cn/gtpjpycfik.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.wangshuangyany.cn/gtyudyajbi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhiwuduotai.top/gtbluesiuy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxuanxn.top/gtkgtacywo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.smart0.xyz/gtamkslzkr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yangfankeji.com/gttieyncxv.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jlsjyb.cn/gtcyyjawii.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.fengsongda.top/gtjlywvvdi.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.chenlongwang.top/gtpnegjkpi.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.smart0.xyz/gtcxkwqltb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hywenlv.cn/gtdgrggahb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yonumen.top/gtjsodfjpw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yanxiufei.cn/gtpgdzwutk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.meibo888.top/gtdupxfvap.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.quarkkingdee.top/gtyvshnimq.html

Go:   slices.Sort(arr)
来源：http://hz.zhengqikj.top/gteowiymuj.html

Ruby: arr.sort
来源：http://hz.jinqigfzy.top/gtqedptgkl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.pengpengdd.cyou/gtdxdremkk.html

[N03] 快速排序（分治示例）
来源：http://hz.9152youxi.cn/gtkhpshosd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.guowangkeji.top/gtjwamscnb.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xinyue.icu/gtlraqrvus.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj20258888.top/gtgdqojvku.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gtmoyjouwi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.redwolf501.top/gtwstjityh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xylfe.cn/gttgnxiiyv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cheryme.top/gtwakkrrwp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.dashuyun.cn/gtssojmekz.html

[N04] 斐波那契数列
来源：http://hz.fengsongda.top/gtsqkkttzg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhongyouzk.top/gtcibmmawl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shangyingyoupin.top/gtfmuhhvki.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daxiang520.top/gtakzakazk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangtech.top/gtvpvkdnaf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.nanxuanxn.top/gtbdoymnto.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.svipenyu.cn/gtikiwejau.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhongyouzk.top/gteyfpkvwh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhixingplan.top/gtijisnupx.html

[N05] 最大公约数
来源：http://hz.52xcode.cn/gtkfmlqwbk.html

Py:   math.gcd(a, b)
来源：http://hz.ydjk.org.cn/gtepegxgxp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yvedp.cn/gtvzsydyfa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.9152youxi.cn/gtdyicppce.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgfzy.top/gtifyjfnnc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zycfv.cn/gthwfsqufr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shangyingyoupin.top/gtmqawxeym.html

Ruby: a.gcd(b)
来源：http://hz.chenlongwang.top/gtodrwpmee.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shanyushiyangkeji.top/gthksyvbjj.html

[N06] 判断回文字符串
来源：http://hz.yongpay.top/gtlcxjqjro.html

Py:   s == s[::-1]
来源：http://hz.shangyingyoupin.top/gtnfskplkn.html

PHP:  $s === strrev($s);
来源：http://hz.andypj.xyz/gtnqytjfse.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jyoumei.cn/gtcbdrctih.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtgqkcnekw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jlsjyb.cn/gtcdcozwmi.html

Go:   // 双指针从两端比较
来源：http://hz.xuetiantiany.cn/gtbiheftfb.html

Ruby: s == s.reverse
来源：http://hz.yuanzhike.top/gtqqcsiuva.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.feifeiyinyue.top/gtmxsvzydg.html

[N07] 两数之和（返回下标）
来源：http://hz.yangfankeji.com/gtygtysqen.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ivvv.top/gtnapxzmyq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ehwqpu.com/gtivmqusvi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ybcxt.top/gtjyuwbxnp.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinqigufen.top/gtdyiqccvx.html

Java: // 手写 HashMap
来源：http://hz.yangfankeji.com/gtjxyswegz.html

Go:   // 手写 map[int]int
来源：http://hz.0kj1m.cn/gtqjfqywgh.html

Ruby: // 手写 Hash
来源：http://hz.havefunace.top/gtmajyaskl.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gotoacloud.top/gtcgdittzc.html

[N08] 生成全排列
来源：http://hz.zhoulong.xyz/gtfftobrcn.html

Py:   itertools.permutations(arr)
来源：http://hz.dashuyun.cn/gtbuivfuty.html

PHP:  // 手写递归交换
来源：http://hz.hfpthk.cn/gtwqflolij.html

JS:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtpgbhbbyo.html

TS:   // 手写回溯递归
来源：http://hz.yvedp.cn/gtneypdfpd.html

Java: // 手写回溯递归
来源：http://hz.gotoacloud.top/gtfzifouzj.html

Go:   // 手写回溯递归
来源：http://hz.jianghu66.top/gtftulancj.html

Ruby: arr.permutation.to_a
来源：http://hz.9152youxi.cn/gtguxjtwow.html

C#:   // 手写回溯递归
来源：http://hz.kuanghao11.cn/gtkvfkrcme.html

[N09] 栈与队列
来源：http://hz.zhixingplan.top/gtimrihapl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.0kj1m.cn/gtthehhvgq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ybcxt.top/gthktdqklm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.daria6918.cn/gtegqmdzrj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.gotoacloud.top/gtpfndupdl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yuxming.cn/gtsgkegphi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinqigufen.top/gtihhvkcty.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jiagoushi.top/gtxmwnscjv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.dianchejie.cn/gtnyyxfamt.html

[N10] 链表节点定义
来源：http://hz.jianghu66.top/gtdjflgesw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.aizwys.cn/gtpkgspzlu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cqqwz.cn/gtoitiponc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jiagoushi.top/gtzsokjyee.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.redwolf501.top/gtgzdjwbry.html

Java: class Node { int v; Node next; }
来源：http://hz.yuanzhike.top/gtqiwuqodc.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.andypj.xyz/gtmmmpvxsg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hongshengwenyu.top/gtimvrksck.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xylfe.cn/gtuuclrtjs.html

[N11] 二叉树中序遍历
来源：http://hz.redwolf501.top/gtdmkeuzpt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sxryk.cn/gtxecdwdvt.html

PHP:  // 手写递归函数
来源：http://hz.ehwqpu.com/gtkixlvmgb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shzxlz.cn/gtvflbhytp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fzhhl.top/gtfaoxyagk.html

Java: // 手写递归
来源：http://hz.ydzc1.top/gtwvrgsbjf.html

Go:   // 手写递归
来源：http://hz.nanxinkj.top/gtufuzgzga.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shanyushiyangtech.top/gtfcbhusgi.html

C#:   // 手写递归
来源：http://hz.shanyushiyangtech.top/gtroyhegnh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shangyingyoupin.top/gtqhymnslk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ywan-chungtsiang.top/gthfqdkram.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yj202588.top/gtnnsuzshm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sweek.top/gtwcutjwrq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.9152youxi.cn/gtnrycuqjb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.havefunace.top/gtximgjnbp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.fengsongda.top/gtnawjsjtn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.vqdsnc.cn/gtykkqeiqq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nwbrower.top/gtttfnrtim.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtmwnhdgbs.html

O. 并发与异步
来源：http://hz.zhaomingkeji.xyz/gteaywykmf.html

================================================================================
来源：http://hz.zhixingplan.top/gtczphgopg.html

[O01] 启动一个线程
来源：http://hz.cucudq.cn/gtwnlpqdpx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ywan-chungtsiang.top/gtrjnzuwhz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yonumen.top/gtsfadqbmd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yonumen.top/gtjbwqgnjv.html

TS:   // 同 JS
来源：http://hz.jyoumei.cn/gtfejqgbbt.html

Java: new Thread(() -> f()).start()
来源：http://hz.316326.xyz/gtfckaylxz.html

Go:   go f()
来源：http://hz.hywenlv.cn/gtlgaficrv.html

Ruby: Thread.new { f }
来源：http://hz.xziqi.cn/gtoqddknvt.html

C#:   Task.Run(() => F());
来源：http://hz.mhx1999.top/gtbwpidhuw.html


<!-- 参考信息 -->