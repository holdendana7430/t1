代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenjidiqi.icu/gtomvpurpq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jianghu66.top/gtuuoplimk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.haohaochexian.top/gtzqxkesie.html

[K05] 深拷贝对象
来源：http://hz.shuidangran.top/gtxilundtg.html

Py:   copy.deepcopy(obj)
来源：http://hz.cucudq.cn/gtjtjrqtrs.html

PHP:  unserialize(serialize($obj));
来源：http://hz.daria6918.cn/gtgzravbqq.html

JS:   structuredClone(obj)
来源：http://hz.kuanghao11.cn/gtfztlplmz.html

TS:   structuredClone(obj)
来源：http://hz.redwolf501.top/gtfubmjxrd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.guowangkeji.top/gtpalujxod.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.dashuyun.cn/gtjqmgvefn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xuetiantiany.cn/gteuaglnmd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sufxvd.cn/gtrutypubb.html

[K06] 解析 URL 查询串
来源：http://hz.yuanzhike.top/gtefixjduf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinghuilouyu.cn/gteimvhtpa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gzhubu.top/gttzveeyaa.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.9152youxi.cn/gtdvrktblw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.birdmap.top/gtbafybxhl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hnxiangtu.top/gtbsfrwtrw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhijiandao.cn/gtefajosna.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ydzc1.top/gtuwssmkky.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xylfe.cn/gtqwlcwred.html

[K07] 进制转换
来源：http://hz.chenzaomai.com/gtqnbnuuyh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhengqikj.top/gtzchrtdgt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.pycfn.com/gtfufuzyrq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtvtobfjlx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jlsjyb.cn/gtiqqwrkyg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hnqzz.top/gtkmvilima.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ppjwa.cn/gteaterkrb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.guowangkeji.top/gtogqyjkaf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.pengpengdd.cyou/gtakikcekz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ydjk.org.cn/gtmtvyecnl.html

Py:   pickle.dumps(obj)
来源：http://hz.jinyuanbaomall.cn/gtemrjoylo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinghuilouyu.cn/gtawekvvxv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ivvv.top/gtaiwezboe.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ywan-chungtsiang.top/gtnqlpxsgu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ybcxt.top/gtvyaoifzo.html

Go:   encoding/gob
来源：http://hz.zycfv.cn/gttqzohoqy.html

Ruby: Marshal.dump(obj)
来源：http://hz.wangdashe.top/gtbpxxdzwb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shangyingyoupin.top/gtzqjgnovl.html

================================================================================
来源：http://hz.hammf.cn/gtnhyzfehg.html

L. 网络请求
来源：http://hz.hammf.cn/gtmgislnxf.html

================================================================================
来源：http://hz.yuxming.cn/gtksgjnyml.html

[L01] 发送 GET 请求
来源：http://hz.zhijiandao.cn/gtwfjquujr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jlsjyb.cn/gtbxpnkjyt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shanyushiyangtech.top/gtyunerugp.html

JS:   await fetch(url)
来源：http://hz.aizwys.cn/gtofdagdfm.html

TS:   await fetch(url)
来源：http://hz.meibo888.top/gtwwoggwej.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yj202588.top/gtqowfexfn.html

Go:   resp, err := http.Get(url)
来源：http://hz.9152youxi.cn/gtrqhpmdti.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.redwolf501.top/gtnmnsltrx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinyuanbaomall.cn/gtffhsudpm.html

[L02] 发送 POST JSON
来源：http://hz.aizwys.cn/gtctztcoup.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ydjk.org.cn/gtpfrzwabw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hnqzz.top/gtyuymhlem.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cdnleiting.top/gtcvmjtesp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jlsjyb.cn/gtkcjwadof.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.52xcode.cn/gtfjuzacfa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.daria6918.cn/gtaskcwhmw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yangfankeji.com/gtokgvgolj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cdnleiting.top/gteihjpdxa.html

[L03] 设置自定义请求头
来源：http://hz.zhiwuduotai.top/gtepyvxhaa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.pengpengdd.cyou/gtnghllwfq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.quarkkingdee.top/gtfedrrywi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.haohaochexian.top/gtqllhmicw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yvedp.cn/gtusvmcbee.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xuanzx.com/gtxddbcmld.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.fzhhl.top/gtrlvhziqf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.meibo888.top/gtsmgryfhm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yj20258888.top/gtcgkvgyfy.html

[L04] 设置超时
来源：http://hz.fzhhl.top/gtddwzzusn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.daria6918.cn/gtmiovtwtc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.wangdashe.top/gtjsbasyjm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigufen.top/gtpvuqzbaz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zycfv.cn/gtuaphhfqj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xinyue.icu/gtivyvkhmk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinqigufen.top/gttlrcivpp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.quarkkingdee.top/gtvviizotj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.vqdsnc.cn/gteiawxcfe.html

[L05] 上传文件（multipart）
来源：http://hz.zdqjudy.top/gtnbulzfxk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.aizwys.cn/gtmzpcqlfm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.dianchejie.cn/gtdvhwnpph.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hfpthk.cn/gtyuyyxfqr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenzaomai.com/gttubvwcbx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hywenlv.cn/gtbtpuipzd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nwbrower.top/gtmrmilhst.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.wangdashe.top/gtcxbdppbt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhijiandao.cn/gtgbrfvyvj.html

[L06] 解析响应为 JSON
来源：http://hz.pycfn.com/gtdowhgmpq.html

Py:   resp.json()
来源：http://hz.gaohongyu789.top/gtimwpknap.html

PHP:  json_decode($body, true);
来源：http://hz.hfpthk.cn/gtteowdyyy.html

JS:   await resp.json()
来源：http://hz.andypj.xyz/gtcmoqoksc.html

TS:   await resp.json()
来源：http://hz.xuanzx.com/gtwkrejzqb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.dashuyun.cn/gtcxlbsntf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhongyouzk.top/gtdbqgkoqu.html

Ruby: JSON.parse(resp.body)
来源：http://hz.svipenyu.cn/gtxcpxeruu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yj20258888.top/gtlljfesfe.html

[L07] 处理 HTTP 状态码
来源：http://hz.daxiang520.top/gtclymdowd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jinyuanbaomall.cn/gttuyioaxu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.quarkkingdee.top/gtogffxgum.html

JS:   resp.ok;  resp.status
来源：http://hz.hysaishi.cn/gtbecuozkx.html

TS:   resp.ok;  resp.status
来源：http://hz.sxryk.cn/gttjzmzhrx.html

Java: resp.statusCode()
来源：http://hz.cheryme.top/gtacfiyjak.html

Go:   resp.StatusCode
来源：http://hz.xinyue.icu/gttaqkpszc.html

Ruby: resp.code.to_i
来源：http://hz.shzxlz.cn/gtpjvqyhky.html

C#:   (int)resp.StatusCode
来源：http://hz.jiagoushi.top/gtuhdugfoc.html

[L08] 并发请求多个地址
来源：http://hz.zycfv.cn/gtydrtizqs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xuetiantiany.cn/gtlnfbgnkz.html

PHP:  curl_multi_init() 系列
来源：http://hz.fzhhl.top/gtailvhwnc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtowvtpdyp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gaohongyu789.top/gtjqnemgpv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hfpthk.cn/gthrcvytdj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gaohongyu789.top/gttsggdynj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jiagoushi.top/gtrlervuwg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.9152youxi.cn/gttfgltpsc.html

================================================================================
来源：http://hz.zhengqikj.top/gtupeoqkkr.html

M. 命令行 / 进程 / 环境
来源：http://hz.zycfv.cn/gtyxaqlbtu.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtebhrnibz.html

[M01] 读取命令行参数
来源：http://hz.wangdashe.top/gtyikvujfo.html

Py:   sys.argv[1:]
来源：http://hz.jianghu66.top/gtznwtufsf.html

PHP:  $argv;  $argc;
来源：http://hz.bjfxy.top/gtvfzxvdkn.html

JS:   process.argv.slice(2)
来源：http://hz.zhoulong.xyz/gtcpniqbdr.html

TS:   process.argv.slice(2)
来源：http://hz.aibaodan.cn/gtfblnszgu.html

Java: args 数组（main 方法参数）
来源：http://hz.tian-w.cn/gteyhiscls.html

Go:   os.Args[1:]
来源：http://hz.vqdsnc.cn/gtcmjerjrs.html

Ruby: ARGV
来源：http://hz.jinqigufen.top/gtiyvbwwmq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.dashuyun.cn/gtjwlvxxzl.html

[M02] 读取环境变量
来源：http://hz.aizwys.cn/gtkyjbsmgp.html

Py:   os.environ.get("HOME")
来源：http://hz.ydzc1.top/gtwqtfunoh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.redwolf501.top/gtwjvxdbkv.html

JS:   process.env.HOME
来源：http://hz.ywan-chungtsiang.top/gtzahuanlg.html

TS:   process.env.HOME
来源：http://hz.shangyingyoupin.top/gtvjvemyts.html

Java: System.getenv("HOME")
来源：http://hz.jinqigfzy.top/gtfvhkwjss.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.wangdashe.top/gtwgzbqzuj.html

Ruby: ENV["HOME"]
来源：http://hz.yvedp.cn/gtbfdlscmk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.dashuyun.cn/gtnwuivblf.html

[M03] 执行外部命令
来源：http://hz.smart0.xyz/gtlrtilarp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj20258888.top/gtlznmgriu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.52xcode.cn/gttxrpuzpx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenjidiqi.icu/gtzwtqvuhn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xingfuxueyuan.xyz/gtuiduwulk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hysaishi.cn/gturwqczzg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hongshengwenyu.top/gtxskzjqvv.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cucudq.cn/gtrvkgkzhw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ehwqpu.com/gtbyfayiut.html

[M04] 获取当前工作目录
来源：http://hz.jqgufenzy.top/gtdzahvewt.html

Py:   os.getcwd()
来源：http://hz.yj202588.top/gthvjcghra.html

PHP:  getcwd();
来源：http://hz.zhoulong.xyz/gtbufqehfq.html

JS:   process.cwd()
来源：http://hz.yangfankeji.com/gtdymorzok.html

TS:   process.cwd()
来源：http://hz.yonumen.top/gtvvpiywbb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gzhubu.top/gtzxcqvjue.html

Go:   os.Getwd()
来源：http://hz.xinyue.icu/gtgfgulpkf.html

Ruby: Dir.pwd
来源：http://hz.zhixingplan.top/gtfzepryku.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.andypj.xyz/gtgkqjjrdu.html

[M05] 设置退出码
来源：http://hz.yj202588.top/gtstivaety.html

Py:   sys.exit(1)
来源：http://hz.quarkkingdee.top/gtxyhjcdth.html

PHP:  exit(1);
来源：http://hz.sxryk.cn/gtuzwbwbit.html

JS:   process.exit(1)
来源：http://hz.ehwqpu.com/gtjifbogso.html

TS:   process.exit(1)
来源：http://hz.tian-w.cn/gtffhfxnwc.html

Java: System.exit(1)
来源：http://hz.jinqigfzy.top/gtxhtthmnl.html

Go:   os.Exit(1)
来源：http://hz.zhaomingkeji.xyz/gtkaqqshbx.html

Ruby: exit 1
来源：http://hz.kuanghao11.cn/gtdlpthexa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cqqwz.cn/gtzymaequd.html

[M06] 向标准错误输出
来源：http://hz.hongshengwenyu.top/gtinomefju.html

Py:   print("err", file=sys.stderr)
来源：http://hz.pengpengdd.cyou/gtlxxwtlin.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.guowangkeji.top/gtzrrtdmjb.html

JS:   console.error("err")
来源：http://hz.redwolf501.top/gtqxkynyhg.html

TS:   console.error("err")
来源：http://hz.smart0.xyz/gtunymuqrt.html

Java: System.err.println("err")
来源：http://hz.jiagoushi.top/gtgglswpnp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.bjfxy.top/gtplfhmrpk.html

Ruby: warn "err"
来源：http://hz.xylfe.cn/gtcoxadjxv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yj202588.top/gtdcqhahik.html

[M07] 判断是否为主入口
来源：http://hz.cashguo.top/gtxfcjzcqq.html

Py:   if __name__ == "__main__":
来源：http://hz.chenjidiqi.icu/gtmkyumewk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.iojbl.cn/gtfmzdtwbo.html

JS:   require.main === module
来源：http://hz.fzhhl.top/gtdjnvvage.html

TS:   require.main === module
来源：http://hz.aibaodan.cn/gtafszgqty.html

Java: public static void main(String[] args)
来源：http://hz.9152youxi.cn/gtvwipezvh.html

Go:   func main()
来源：http://hz.yj202588.top/gtzjnxuand.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ybcxt.top/gtmiedfwbz.html

C#:   static void Main(string[] args)
来源：http://hz.fengsongda.top/gtqtfrtlqk.html

[M08] 获取系统与运行时信息
来源：http://hz.yuxming.cn/gtoogiyzbv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.feifeiyinyue.top/gtbznufsgq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.wangdashe.top/gtjxkfemlq.html

JS:   process.platform;  process.version
来源：http://hz.zhixingplan.top/gtmoyvqrbn.html

TS:   process.platform;  process.version
来源：http://hz.andypj.xyz/gtislgqajh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sxryk.cn/gtdxwavvky.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.chenlongwang.top/gtatkofmaz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hysaishi.cn/gtvmwiovze.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ivvv.top/gtebkunkot.html

================================================================================
来源：http://hz.xuanzx.com/gtagpphjab.html

N. 数据结构与算法
来源：http://hz.jyoumei.cn/gtmeybeigz.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtuvuswvhz.html

[N01] 二分查找（有序数组）
来源：http://hz.wangshuangyany.cn/gtnwbaubsw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.cucudq.cn/gtnazthvqz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.iojbl.cn/gtpvqvzgmu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jiagoushi.top/gtpxmlipwg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ppjwa.cn/gtwcvrjwqf.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jlsjyb.cn/gtlmacnulm.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cheryme.top/gtrycynchm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shangyingyoupin.top/gtwriulykc.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.smart0.xyz/gtbhahgqhj.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.aibaodan.cn/gtzgxivbss.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.redwolf501.top/gtytardmdo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cheryme.top/gtweskhiqg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nwbrower.top/gtwyjwisex.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhiwuduotai.top/gttdpfqtke.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.gogol.net.cn/gtfohatgoy.html

Go:   slices.Sort(arr)
来源：http://hz.shangyingyoupin.top/gtcwepyiky.html

Ruby: arr.sort
来源：http://hz.fzhhl.top/gtdsdytkwh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zdqjudy.top/gtpystvjdn.html

[N03] 快速排序（分治示例）
来源：http://hz.zdqjudy.top/gtqibpmsbs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yvedp.cn/gtgodzihwh.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nanxuanxn.top/gtckajtxda.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.havefunace.top/gtyhwwqiof.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhijiandao.cn/gteponxzws.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj20258.top/gtcvjjmtbp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nanxuanxn.top/gtfyeqcsjd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yanxiufei.cn/gtuphxtvda.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.kuanghao11.cn/gtoeirsusj.html

[N04] 斐波那契数列
来源：http://hz.ehwqpu.com/gtchkftfgc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.dashuyun.cn/gtzjpilkvu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.chenjidiqi.icu/gtcjjmqgyz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnqzz.top/gtlrjvnswh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yangfankeji.com/gthjjuiaem.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.meibo888.top/gtkdaehwdn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shuidangran.top/gthgwrqhtc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cashguo.top/gtficxfziw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jiagoushi.top/gtdjqpjbwv.html

[N05] 最大公约数
来源：http://hz.havefunace.top/gtchovtcdm.html

Py:   math.gcd(a, b)
来源：http://hz.zdqjudy.top/gtiysdfhkh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yangfankeji.com/gtnpozsred.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgufenzy.top/gtvlhkqbhf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shzxlz.cn/gtdklngjnf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gaohongyu789.top/gtxrlxabep.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.nanxinkj.top/gtbmfgvxil.html

Ruby: a.gcd(b)
来源：http://hz.xylfe.cn/gtbctbslss.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.fengsongda.top/gtwomctmfh.html

[N06] 判断回文字符串
来源：http://hz.shzxlz.cn/gttyprforc.html

Py:   s == s[::-1]
来源：http://hz.redwolf501.top/gtjvnnemyz.html

PHP:  $s === strrev($s);
来源：http://hz.xuetiantiany.cn/gtoorzlrix.html

JS:   s === [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtidnnthjj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.pycfn.com/gtegogjwar.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sufxvd.cn/gtufyakqsi.html

Go:   // 双指针从两端比较
来源：http://hz.jqgufenzy.top/gtuhvwnrez.html

Ruby: s == s.reverse
来源：http://hz.sxryk.cn/gttcbnmfum.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xinyue.icu/gtqtrkextk.html

[N07] 两数之和（返回下标）
来源：http://hz.wangdashe.top/gtpxrfrxpz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhaomingkeji.xyz/gtwrzuvflw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sysykeji.top/gtarypgite.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shangyingyoupin.top/gttudjoezf.html

TS:   // 手写 Map<string, number>
来源：http://hz.svipenyu.cn/gtkzxgbwvl.html

Java: // 手写 HashMap
来源：http://hz.hywenlv.cn/gtxcmnlbrx.html

Go:   // 手写 map[int]int
来源：http://hz.xylfe.cn/gtmevvvlqg.html

Ruby: // 手写 Hash
来源：http://hz.c1oappe.top/gthopwqdfb.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gotoacloud.top/gtuklgkdcc.html

[N08] 生成全排列
来源：http://hz.yuxming.cn/gtrmmwuhwp.html

Py:   itertools.permutations(arr)
来源：http://hz.dianchejie.cn/gtozjjmbrb.html

PHP:  // 手写递归交换
来源：http://hz.jiagoushi.top/gtunhkybhz.html

JS:   // 手写回溯递归
来源：http://hz.havefunace.top/gtyusvsrxe.html

TS:   // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtwtznlbll.html

Java: // 手写回溯递归
来源：http://hz.zycfv.cn/gtqlbxemmf.html

Go:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtbsnucdal.html

Ruby: arr.permutation.to_a
来源：http://hz.gotoacloud.top/gtukbuzqgj.html

C#:   // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtmuisbbzq.html

[N09] 栈与队列
来源：http://hz.pycfn.com/gtbwjgneel.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.snrcjt.cn/gtjdouwbov.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.birdmap.top/gtrddtgrha.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.daxiang520.top/gtjgobdukc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zycfv.cn/gtkflnktsd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.bjfxy.top/gtjlcigvqo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xziqi.cn/gtahtetryn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yj202588.top/gtjkhfeupf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xingfuxueyuan.xyz/gtpvmpvbfg.html

[N10] 链表节点定义
来源：http://hz.aibaodan.cn/gtcdvufaug.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.guowangkeji.top/gtcbijrlbu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ydjk.org.cn/gtxquaphbu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.pengpengdd.cyou/gtwllonjwr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.0kj1m.cn/gtxqnbbtza.html

Java: class Node { int v; Node next; }
来源：http://hz.xziqi.cn/gtgvldwbju.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.chenzaomai.com/gtvcjfnlbt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yvedp.cn/gteyuemola.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shanyushiyangtech.top/gtuzljardv.html

[N11] 二叉树中序遍历
来源：http://hz.zhongyouzk.top/gtaukxjxmi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinqigfzy.top/gtrhjdqqoz.html

PHP:  // 手写递归函数
来源：http://hz.yangfankeji.com/gtjlfumlop.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenzaomai.com/gtrbkvgiuy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.9152youxi.cn/gtaveseahi.html

Java: // 手写递归
来源：http://hz.kuanghao11.cn/gtlboxpmar.html

Go:   // 手写递归
来源：http://hz.dianchejie.cn/gtkyknsixr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cheryme.top/gtabshfnxw.html

C#:   // 手写递归
来源：http://hz.yj20258.top/gttvpkxhdt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.dianchejie.cn/gtcbwefdvo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ydjk.org.cn/gtbhfsbxyx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.guowangkeji.top/gttopeeyyo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aibaodan.cn/gtaoszjfzl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuanzx.com/gtparupgda.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shuidangran.top/gtlugzpbot.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhijiandao.cn/gtlrrqnhdq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xuanzx.com/gttvdurxzf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yongpay.top/gtiylgohdb.html


<!-- 参考信息 -->