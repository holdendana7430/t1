代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://hz.guowangkeji.top/gtabessakj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tian-w.cn/gtppulprum.html

JS:   structuredClone(obj)
来源：http://hz.zycfv.cn/gtzfkdhofi.html

TS:   structuredClone(obj)
来源：http://hz.yongpay.top/gtgyrmjzno.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hywenlv.cn/gtvcxfoweh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.aizwys.cn/gtgbkaepgp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.fengsongda.top/gtagshowgu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj20258.top/gtwchsukag.html

[K06] 解析 URL 查询串
来源：http://hz.haohaochexian.top/gtwtlilrkg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yueranfly.top/gtningktme.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.9152youxi.cn/gtploqttfk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.svipenyu.cn/gtisfwfyry.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangshuangyany.cn/gtspeohhrh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sweek.top/gtpdnmptbs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gzhubu.top/gtbucvmght.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hfpthk.cn/gtlxfacmoe.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.kuanghao11.cn/gtmmvtfmew.html

[K07] 进制转换
来源：http://hz.xziqi.cn/gtvpkgegyt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.redwolf501.top/gtvlbhjhei.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yuxming.cn/gtoeeegvuu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj20258888.top/gtguwodzje.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtcdwqgwno.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.nwbrower.top/gtfrupqknc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinqigufen.top/gtqyqavvgn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gotoacloud.top/gtdbdqstsd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhixingplan.top/gtlhsurjae.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.quarkkingdee.top/gtdndcfaoh.html

Py:   pickle.dumps(obj)
来源：http://hz.dianchejie.cn/gtoxbceouy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.pycfn.com/gttsnbcxxm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jianghu66.top/gtixlxodma.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.birdmap.top/gtqbcfobem.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.bjfxy.top/gtlhwmbukp.html

Go:   encoding/gob
来源：http://hz.zhengqikj.top/gtllvoqqai.html

Ruby: Marshal.dump(obj)
来源：http://hz.meibo888.top/gtguaateda.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.nwbrower.top/gthtxgshhx.html

================================================================================
来源：http://hz.gotoacloud.top/gtonyhhqjm.html

L. 网络请求
来源：http://hz.chenjidiqi.icu/gtcnwsasuj.html

================================================================================
来源：http://hz.hysaishi.cn/gtastsugcp.html

[L01] 发送 GET 请求
来源：http://hz.chenzaomai.com/gtszujjnjz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zycfv.cn/gtwsdjejgm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jianghu66.top/gtcoynkavo.html

JS:   await fetch(url)
来源：http://hz.guowangkeji.top/gtfcrvnwji.html

TS:   await fetch(url)
来源：http://hz.chenlongwang.top/gttkyktetb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.chenzaomai.com/gtgngsyfcy.html

Go:   resp, err := http.Get(url)
来源：http://hz.xylfe.cn/gttlmdkpwl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gaohongyu789.top/gtycamoqxo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jqgufenzy.top/gtfughetra.html

[L02] 发送 POST JSON
来源：http://hz.xingfuxueyuan.xyz/gtkeknvbzp.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xziqi.cn/gtgmsuumoo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hnxiangtu.top/gtaewqzmng.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jlsjyb.cn/gtoupixopk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xingfuxueyuan.xyz/gtnraflltx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yanxiufei.cn/gtxkqxdfnu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hammf.cn/gtbppjsvky.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.tian-w.cn/gtwdtewwzf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.chenjidiqi.icu/gtvemipojm.html

[L03] 设置自定义请求头
来源：http://hz.svipenyu.cn/gtijrkhycg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinqigufen.top/gtuevbxgow.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jlsjyb.cn/gtjeldhnmn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxinkj.top/gtgkxrxrtd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pycfn.com/gtfqcsfxre.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shanyushiyangkeji.top/gtqfgkeqof.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.daria6918.cn/gtuynkimqg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xuetiantiany.cn/gtquxpoxzq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hysaishi.cn/gtvukkngqh.html

[L04] 设置超时
来源：http://hz.aibaodan.cn/gtiuvaffvl.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cdnleiting.top/gthcpezklj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhixingplan.top/gthqrttetd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhiwuduotai.top/gtrjizhebu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cucudq.cn/gtzlbrbflt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yonumen.top/gtzuhhlkty.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shangyingyoupin.top/gtmvoucjjt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinqigfzy.top/gtjhyweapc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ydjk.org.cn/gtnuzzkpwz.html

[L05] 上传文件（multipart）
来源：http://hz.gaohongyu789.top/gtzdzozzbh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ybcxt.top/gtdoglvjrk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zycfv.cn/gttuncedav.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangtech.top/gttzyhcbiy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhongyouzk.top/gtstkmhjby.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.quarkkingdee.top/gtsafteaca.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.gaohongyu789.top/gtisnntgoi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hnqzz.top/gtfsodsbkx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhaomingkeji.xyz/gtxtitcixw.html

[L06] 解析响应为 JSON
来源：http://hz.andypj.xyz/gtycjwspmd.html

Py:   resp.json()
来源：http://hz.hongshengwenyu.top/gtvbzrqssg.html

PHP:  json_decode($body, true);
来源：http://hz.shuidangran.top/gtfjbbqrxs.html

JS:   await resp.json()
来源：http://hz.yangfankeji.com/gtoalwsqsh.html

TS:   await resp.json()
来源：http://hz.gzhubu.top/gtgbtwecti.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cqqwz.cn/gtzxvyrztf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.aibaodan.cn/gtgiqvzhok.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xinyue.icu/gtwzvemkkd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hnqzz.top/gthwriwenr.html

[L07] 处理 HTTP 状态码
来源：http://hz.c1oappe.top/gtcygdoaew.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shuidangran.top/gtsgggpuzi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zdqjudy.top/gteqibmkxr.html

JS:   resp.ok;  resp.status
来源：http://hz.meibo888.top/gtmrksvoec.html

TS:   resp.ok;  resp.status
来源：http://hz.aibaodan.cn/gtlnwshbwq.html

Java: resp.statusCode()
来源：http://hz.jinqigfzy.top/gtqbkjtuyx.html

Go:   resp.StatusCode
来源：http://hz.tanke756.top/gtwlvcauqn.html

Ruby: resp.code.to_i
来源：http://hz.birdmap.top/gtgzzfqkke.html

C#:   (int)resp.StatusCode
来源：http://hz.zhixingplan.top/gtsrcwzzzc.html

[L08] 并发请求多个地址
来源：http://hz.ywan-chungtsiang.top/gtgcriucpr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.snrcjt.cn/gtguafuyin.html

PHP:  curl_multi_init() 系列
来源：http://hz.feifeiyinyue.top/gtrtspoeyd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yonumen.top/gthnodgcop.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtvjhcjxhv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.dianchejie.cn/gtqpbeppol.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yuxming.cn/gtteldkohu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.sufxvd.cn/gttdiayovl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.iojbl.cn/gtvlydkvfn.html

================================================================================
来源：http://hz.sweek.top/gtmbhpkvpr.html

M. 命令行 / 进程 / 环境
来源：http://hz.sxryk.cn/gtlrimskmt.html

================================================================================
来源：http://hz.tian-w.cn/gtodoalyhl.html

[M01] 读取命令行参数
来源：http://hz.yuanzhike.top/gtlglogavp.html

Py:   sys.argv[1:]
来源：http://hz.ppjwa.cn/gtxjqgekqy.html

PHP:  $argv;  $argc;
来源：http://hz.jqgufenzy.top/gtvembrnuh.html

JS:   process.argv.slice(2)
来源：http://hz.hnqzz.top/gtqurlqxrd.html

TS:   process.argv.slice(2)
来源：http://hz.wangdashe.top/gtqzrmjfwr.html

Java: args 数组（main 方法参数）
来源：http://hz.jinqigfzy.top/gtglxgebls.html

Go:   os.Args[1:]
来源：http://hz.havefunace.top/gtjmfvgmrc.html

Ruby: ARGV
来源：http://hz.9152youxi.cn/gtavvpvvny.html

C#:   args 数组（Main 方法参数）
来源：http://hz.iojbl.cn/gtphrypahz.html

[M02] 读取环境变量
来源：http://hz.cqqwz.cn/gtzlugtpjz.html

Py:   os.environ.get("HOME")
来源：http://hz.316326.xyz/gthvlgyyok.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenlongwang.top/gttavzpbeh.html

JS:   process.env.HOME
来源：http://hz.pycfn.com/gtzqcgtgao.html

TS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtgjqerwrp.html

Java: System.getenv("HOME")
来源：http://hz.kuanghao11.cn/gtvplgxxcj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.pengpengdd.cyou/gtpdckfbms.html

Ruby: ENV["HOME"]
来源：http://hz.svipenyu.cn/gtodbcltiw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shanyushiyangtech.top/gtchvlfrad.html

[M03] 执行外部命令
来源：http://hz.hongshengwenyu.top/gtrcvbtkko.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.meibo888.top/gtthghegbh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhixingplan.top/gtoqcgozbf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj20258.top/gtszvinheo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinghuilouyu.cn/gtoipnhneo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.pycfn.com/gthywmxdjr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cashguo.top/gtlqkkzzbp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hnxiangtu.top/gtnyajtjbk.html

C#:   Process.Start("ls", "-l");
来源：http://hz.haohaochexian.top/gtftcmjhmq.html

[M04] 获取当前工作目录
来源：http://hz.jiagoushi.top/gtcbrvozwg.html

Py:   os.getcwd()
来源：http://hz.kuanghao11.cn/gtxcgddvqw.html

PHP:  getcwd();
来源：http://hz.svipenyu.cn/gtgwvrpnny.html

JS:   process.cwd()
来源：http://hz.yueranfly.top/gtvrmwfggv.html

TS:   process.cwd()
来源：http://hz.9152youxi.cn/gteoxjrawi.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shzxlz.cn/gtpyzxmipx.html

Go:   os.Getwd()
来源：http://hz.shanyushiyangkeji.top/gtoijzwaan.html

Ruby: Dir.pwd
来源：http://hz.hnxiangtu.top/gtwfmhjqlv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.tanke756.top/gtqdcduysc.html

[M05] 设置退出码
来源：http://hz.jinqigfzy.top/gtwnzgewtp.html

Py:   sys.exit(1)
来源：http://hz.jyoumei.cn/gtwywycdsa.html

PHP:  exit(1);
来源：http://hz.ywan-chungtsiang.top/gtgxrsblvn.html

JS:   process.exit(1)
来源：http://hz.jianghu66.top/gtosxdqpem.html

TS:   process.exit(1)
来源：http://hz.zhixingplan.top/gtxfdepmlf.html

Java: System.exit(1)
来源：http://hz.pycfn.com/gtikynjogm.html

Go:   os.Exit(1)
来源：http://hz.dianchejie.cn/gtvmahcmpw.html

Ruby: exit 1
来源：http://hz.ydjk.org.cn/gtbrcskrll.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nanxinkj.top/gtojmdkztg.html

[M06] 向标准错误输出
来源：http://hz.chenjidiqi.icu/gtkmjlaiwf.html

Py:   print("err", file=sys.stderr)
来源：http://hz.quarkkingdee.top/gtfargwaqr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenzaomai.com/gtujyryolg.html

JS:   console.error("err")
来源：http://hz.zycfv.cn/gtftkhkxof.html

TS:   console.error("err")
来源：http://hz.hfpthk.cn/gtddqhracs.html

Java: System.err.println("err")
来源：http://hz.chenlongwang.top/gtpssfnrqq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.tianlin.xyz/gtnttxkoyd.html

Ruby: warn "err"
来源：http://hz.zhixingplan.top/gtdmikjjtp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xuetiantiany.cn/gtnkdvtjbp.html

[M07] 判断是否为主入口
来源：http://hz.aibaodan.cn/gtikgwnjjw.html

Py:   if __name__ == "__main__":
来源：http://hz.jianghu66.top/gtlxbshcju.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gaohongyu789.top/gtrsvhjhbh.html

JS:   require.main === module
来源：http://hz.cqqwz.cn/gtmwfdiuhc.html

TS:   require.main === module
来源：http://hz.zdqjudy.top/gtvmpvfchu.html

Java: public static void main(String[] args)
来源：http://hz.sxryk.cn/gthcliqvoh.html

Go:   func main()
来源：http://hz.sweek.top/gtpvbdmenu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ivvv.top/gtxaldajfi.html

C#:   static void Main(string[] args)
来源：http://hz.zhongyouzk.top/gtkcyuoasp.html

[M08] 获取系统与运行时信息
来源：http://hz.hysaishi.cn/gtvwcboxbj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xuetiantiany.cn/gtomespsxi.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yangfankeji.com/gtfizvpjfe.html

JS:   process.platform;  process.version
来源：http://hz.0kj1m.cn/gtpqdxsjaj.html

TS:   process.platform;  process.version
来源：http://hz.redwolf501.top/gtqexpkfdd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xylfe.cn/gtxfhislra.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.fzhhl.top/gtoklwaess.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jqgufenzy.top/gtjkjralhc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shzxlz.cn/gtgimuoxjz.html

================================================================================
来源：http://hz.gzhubu.top/gtbjdmvrmd.html

N. 数据结构与算法
来源：http://hz.jlsjyb.cn/gthmezouin.html

================================================================================
来源：http://hz.mhx1999.top/gtisxbssfs.html

[N01] 二分查找（有序数组）
来源：http://hz.ybcxt.top/gtrdqzicuf.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hammf.cn/gtitttwokt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hammf.cn/gtzlbnvjqj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.bjfxy.top/gtamemykkd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhaomingkeji.xyz/gtajfkpxfh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtcmhzhume.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtlxhqypoq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhoulong.xyz/gtnyozzeiu.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ydzc1.top/gtuaffoihc.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shangyingyoupin.top/gtrhdjsxeq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xinyue.icu/gtupknhvnl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhoulong.xyz/gtxxdnnzgv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yvedp.cn/gttqmqwtnw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxinkj.top/gtwyfbycao.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xziqi.cn/gtbpipwysy.html

Go:   slices.Sort(arr)
来源：http://hz.shzxlz.cn/gtkjighoyf.html

Ruby: arr.sort
来源：http://hz.jlsjyb.cn/gtkfditxtr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinqigfzy.top/gtmfhtcull.html

[N03] 快速排序（分治示例）
来源：http://hz.jianghu66.top/gttdgglulo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.316326.xyz/gtgnaymluh.html

PHP:  // 递归实现，或用 usort
来源：http://hz.pycfn.com/gtnxiuyzsr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinghuilouyu.cn/gtiagulowo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xinyue.icu/gtrvzdehgq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jqgufenzy.top/gtbtuxrmxg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinqigfzy.top/gtqtbdyjsq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.pycfn.com/gtllecegmp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yonumen.top/gtxvrgqviv.html

[N04] 斐波那契数列
来源：http://hz.tian-w.cn/gtwgbhydhk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cqqwz.cn/gtyidhfsnl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.iojbl.cn/gtcyvfdeqr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuanzhike.top/gtpcmnxecb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fengsongda.top/gtniqlqcnn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhixingplan.top/gtmdwanbhw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hammf.cn/gtcvzhgqpd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yongpay.top/gtapqvnwyp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.snrcjt.cn/gtyyvzpcwi.html

[N05] 最大公约数
来源：http://hz.tian-w.cn/gtcrtidwti.html

Py:   math.gcd(a, b)
来源：http://hz.yj202588.top/gtngfvpkna.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.gzhubu.top/gtdpisfjyd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.meibo888.top/gtvluqnvxa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daria6918.cn/gtcjgwimog.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhoulong.xyz/gtchtqxypo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jqgfzy.top/gttdexjfny.html

Ruby: a.gcd(b)
来源：http://hz.cashguo.top/gtxxbrmdng.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhongyouzk.top/gtcotuteum.html

[N06] 判断回文字符串
来源：http://hz.dianchejie.cn/gtzpgnslat.html

Py:   s == s[::-1]
来源：http://hz.iojbl.cn/gtisburiol.html

PHP:  $s === strrev($s);
来源：http://hz.jinyuanbaomall.cn/gtbgviyosd.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtfeonwesq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hfpthk.cn/gtyljrzxkf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.fengsongda.top/gtuznachby.html

Go:   // 双指针从两端比较
来源：http://hz.kuanghao11.cn/gtwixbpjrb.html

Ruby: s == s.reverse
来源：http://hz.9152youxi.cn/gtpefrlslj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.andypj.xyz/gthczrtngo.html

[N07] 两数之和（返回下标）
来源：http://hz.zhiwuduotai.top/gtxesdavav.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.0kj1m.cn/gtzsuflhzm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sweek.top/gtbtdtfygh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinqigufen.top/gtxwycryln.html

TS:   // 手写 Map<string, number>
来源：http://hz.andypj.xyz/gthotdwmdl.html

Java: // 手写 HashMap
来源：http://hz.tian-w.cn/gtrmweoadv.html

Go:   // 手写 map[int]int
来源：http://hz.tanke756.top/gtkauwfeew.html

Ruby: // 手写 Hash
来源：http://hz.shuidangran.top/gtjkoljraj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.andypj.xyz/gtcjeearri.html

[N08] 生成全排列
来源：http://hz.shuidangran.top/gtpzjqvdaz.html

Py:   itertools.permutations(arr)
来源：http://hz.snrcjt.cn/gtwmgevrzr.html

PHP:  // 手写递归交换
来源：http://hz.316326.xyz/gtpfvgsrfa.html

JS:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtqjxlxytz.html

TS:   // 手写回溯递归
来源：http://hz.cashguo.top/gtijdugbvt.html

Java: // 手写回溯递归
来源：http://hz.tianlin.xyz/gtrhwgbfph.html

Go:   // 手写回溯递归
来源：http://hz.birdmap.top/gtvtsvbudj.html

Ruby: arr.permutation.to_a
来源：http://hz.xziqi.cn/gtojqtslsb.html

C#:   // 手写回溯递归
来源：http://hz.sweek.top/gtejrnicon.html

[N09] 栈与队列
来源：http://hz.0kj1m.cn/gtmajpcwty.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jinqigufen.top/gtkcsvossx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zycfv.cn/gtkzgxwnfu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.guowangkeji.top/gtlqjoykbm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.chenjidiqi.icu/gteysmhfbf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.cashguo.top/gtyaqotjqk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.guowangkeji.top/gtstswsbak.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.gaohongyu789.top/gtqbnosxck.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.aizwys.cn/gtxjtjrpgx.html

[N10] 链表节点定义
来源：http://hz.ivvv.top/gthbqmnutz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.wangdashe.top/gtgwhqpaig.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zycfv.cn/gtibwwrmqk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.redwolf501.top/gtttoqkdus.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.nanxinkj.top/gtaqdikclj.html

Java: class Node { int v; Node next; }
来源：http://hz.shuidangran.top/gtkwixumqh.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.snrcjt.cn/gtnocwrbzz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xinyue.icu/gtheismfda.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yuanzhike.top/gtqnwhgpay.html

[N11] 二叉树中序遍历
来源：http://hz.chenjidiqi.icu/gtedtmwysp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.kuanghao11.cn/gtslimmhpj.html

PHP:  // 手写递归函数
来源：http://hz.zhengqikj.top/gtmucedsev.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ywan-chungtsiang.top/gtmujzsabh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hysaishi.cn/gtudxxrqzs.html

Java: // 手写递归
来源：http://hz.svipenyu.cn/gtcuhygrsy.html

Go:   // 手写递归
来源：http://hz.shangyingyoupin.top/gtgyajeogx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.9152youxi.cn/gthphjcrnh.html

C#:   // 手写递归
来源：http://hz.ppjwa.cn/gtjhkqvkya.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.nanxinkj.top/gtagsqugul.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.snrcjt.cn/gtbkwlbzzs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.wangdashe.top/gtgofxkkvp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhengqikj.top/gtnepqqoql.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jlsjyb.cn/gtcrhjxzhv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ywan-chungtsiang.top/gtwlvhwoig.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ydzc1.top/gtozjyykmm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ppjwa.cn/gtftdslvqg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgfzy.top/gtzttdpetl.html

================================================================================
来源：http://hz.nanxinkj.top/gtdbajmqww.html

O. 并发与异步
来源：http://hz.0kj1m.cn/gtcxpsumhj.html

================================================================================
来源：http://hz.jqgfzy.top/gtubxwlcbd.html

[O01] 启动一个线程
来源：http://hz.shanyushiyangtech.top/gtpahmngzb.html


<!-- 参考信息 -->