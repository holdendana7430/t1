代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://hz.birdmap.top/gtlcgdyvfy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.nwbrower.top/gtunktazjq.html

JS:   structuredClone(obj)
来源：http://hz.chenzaomai.com/gtdfyktuqr.html

TS:   structuredClone(obj)
来源：http://hz.zhixingplan.top/gtaqybwzzw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhiwuduotai.top/gteeokptnx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hammf.cn/gtboaewulx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hnqzz.top/gtbamyrenc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gogol.net.cn/gtlyxzslyu.html

[K06] 解析 URL 查询串
来源：http://hz.yvedp.cn/gtowgyaqet.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xziqi.cn/gthwuzwxcc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tianlin.xyz/gtcwawotvw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtvxjzarxm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhijiandao.cn/gtmcpvgssv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.guowangkeji.top/gtzewnrwmj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.pycfn.com/gttdglueuo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xuanzx.com/gtrtapglyj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hfpthk.cn/gtxxtowccn.html

[K07] 进制转换
来源：http://hz.jlsjyb.cn/gtybnhxytr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cqqwz.cn/gtscvdapjm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sxryk.cn/gteijpcbol.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shangyingyoupin.top/gtdwyfqtti.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gtqztkbach.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.fengsongda.top/gtcrlemzgl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sysykeji.top/gtuodqyzjq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yuxming.cn/gtjgzzkvnt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xziqi.cn/gtyxedjddw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.mhx1999.top/gtvoyipcme.html

Py:   pickle.dumps(obj)
来源：http://hz.nanxinkj.top/gtytrzurux.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gaohongyu789.top/gtmoqcflmh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.316326.xyz/gtinfdcxei.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yuanzhike.top/gtllkemjsb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xziqi.cn/gttjsglskg.html

Go:   encoding/gob
来源：http://hz.xuanzx.com/gtytpxmtnl.html

Ruby: Marshal.dump(obj)
来源：http://hz.gzhubu.top/gtxboihiph.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.tianlin.xyz/gtfijojgqq.html

================================================================================
来源：http://hz.zhongyouzk.top/gtrncyuqsk.html

L. 网络请求
来源：http://hz.yangfankeji.com/gtkozuvbau.html

================================================================================
来源：http://hz.wangdashe.top/gtaemlzafo.html

[L01] 发送 GET 请求
来源：http://hz.shzxlz.cn/gtlnehoohd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zdqjudy.top/gtjcpgkqhv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhongyouzk.top/gtfhtuqmry.html

JS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gtpytytqrf.html

TS:   await fetch(url)
来源：http://hz.hywenlv.cn/gtunyzwbyw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cashguo.top/gtlcshsxms.html

Go:   resp, err := http.Get(url)
来源：http://hz.c1oappe.top/gtrkobysxd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hammf.cn/gtzkcztsxm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cdnleiting.top/gtwjlbosjl.html

[L02] 发送 POST JSON
来源：http://hz.9152youxi.cn/gtgtldnrjc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.tanke756.top/gtgdmrypiv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gotoacloud.top/gtwjpipoof.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shzxlz.cn/gtzhhvuihw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shzxlz.cn/gtplizcswj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zycfv.cn/gtewsjjnlu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hfpthk.cn/gtdusbzamk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cucudq.cn/gtzklkqqwk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cqqwz.cn/gtcyctnisa.html

[L03] 设置自定义请求头
来源：http://hz.yj202588.top/gtvypsysrd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.snrcjt.cn/gtjemkukgm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xziqi.cn/gtznoaurgk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.smart0.xyz/gtulzbjzrj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangshuangyany.cn/gtokugvlmj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.smart0.xyz/gtupalimku.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinqigufen.top/gttemsadlw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.316326.xyz/gtiucqvcfk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuxming.cn/gtfjvcndgb.html

[L04] 设置超时
来源：http://hz.jinqigufen.top/gtsrqggfwn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.vqdsnc.cn/gtpxqmqsjk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yanxiufei.cn/gtrjycmmqu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.iojbl.cn/gtwpcbwjjo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.snrcjt.cn/gtedujrjls.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.316326.xyz/gtlhbssoen.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jiagoushi.top/gtzrjfslou.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.daxiang520.top/gtpcwmqkxe.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.bjfxy.top/gtmluskafp.html

[L05] 上传文件（multipart）
来源：http://hz.dianchejie.cn/gtbgvqgjpg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ydzc1.top/gtugwlcefb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.9152youxi.cn/gtisbfzzdo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258888.top/gtbryqolyy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.fzhhl.top/gtiadkznmi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jlsjyb.cn/gtblsbsxsz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.daria6918.cn/gtvpwkgqth.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ivvv.top/gtyaifuepk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yueranfly.top/gtdnjnddxr.html

[L06] 解析响应为 JSON
来源：http://hz.bjfxy.top/gtcjnmihht.html

Py:   resp.json()
来源：http://hz.bjfxy.top/gtgpzucxlu.html

PHP:  json_decode($body, true);
来源：http://hz.c1oappe.top/gtoxhegniq.html

JS:   await resp.json()
来源：http://hz.gogol.net.cn/gtotnzrkbd.html

TS:   await resp.json()
来源：http://hz.sufxvd.cn/gtqexjstgr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jyoumei.cn/gtzmbbmvqt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.nanxuanxn.top/gtqvveuqxb.html

Ruby: JSON.parse(resp.body)
来源：http://hz.daxiang520.top/gtbfshuwrk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cheryme.top/gtomjjgohu.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhaomingkeji.xyz/gtgmvetrsj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yueranfly.top/gtiepjwsqy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhengqikj.top/gtvexvxxts.html

JS:   resp.ok;  resp.status
来源：http://hz.pycfn.com/gtzanttrsm.html

TS:   resp.ok;  resp.status
来源：http://hz.daxiang520.top/gtsmsxbvop.html

Java: resp.statusCode()
来源：http://hz.tianlin.xyz/gtfdlubxxz.html

Go:   resp.StatusCode
来源：http://hz.jinqigfzy.top/gtsiguamyi.html

Ruby: resp.code.to_i
来源：http://hz.jyoumei.cn/gtznffaiai.html

C#:   (int)resp.StatusCode
来源：http://hz.yongpay.top/gtaapjflhp.html

[L08] 并发请求多个地址
来源：http://hz.xinyue.icu/gtgmwtvliu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.aizwys.cn/gtilifslei.html

PHP:  curl_multi_init() 系列
来源：http://hz.shangyingyoupin.top/gtfyoxwwte.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pengpengdd.cyou/gtlcyfjwam.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258888.top/gtyjnnxwbu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cashguo.top/gtxxyyjbch.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tianlin.xyz/gtlgmwwbbv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.chenjidiqi.icu/gtdvzeahnj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.havefunace.top/gtewbllage.html

================================================================================
来源：http://hz.shuidangran.top/gtlhhpoiwn.html

M. 命令行 / 进程 / 环境
来源：http://hz.shzxlz.cn/gtqmsfnxhz.html

================================================================================
来源：http://hz.sxryk.cn/gtchsdlhoa.html

[M01] 读取命令行参数
来源：http://hz.daxiang520.top/gtylyhuosn.html

Py:   sys.argv[1:]
来源：http://hz.andypj.xyz/gthyyztssn.html

PHP:  $argv;  $argc;
来源：http://hz.yanxiufei.cn/gtkjxizwkh.html

JS:   process.argv.slice(2)
来源：http://hz.jinqigfzy.top/gtepeslnnv.html

TS:   process.argv.slice(2)
来源：http://hz.xylfe.cn/gtbmsmeywq.html

Java: args 数组（main 方法参数）
来源：http://hz.zhixingplan.top/gthsuzihjk.html

Go:   os.Args[1:]
来源：http://hz.daxiang520.top/gtulerkwmh.html

Ruby: ARGV
来源：http://hz.ppjwa.cn/gtmyajvmun.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhongyouzk.top/gtscfdhxff.html

[M02] 读取环境变量
来源：http://hz.cucudq.cn/gtfidfpukm.html

Py:   os.environ.get("HOME")
来源：http://hz.gotoacloud.top/gtkyswkodp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ivvv.top/gttiqepnbe.html

JS:   process.env.HOME
来源：http://hz.kuanghao11.cn/gtfzwljzub.html

TS:   process.env.HOME
来源：http://hz.kuanghao11.cn/gtpjgevqaz.html

Java: System.getenv("HOME")
来源：http://hz.ybcxt.top/gtceqlzhaa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shanyushiyangkeji.top/gtmmyriiio.html

Ruby: ENV["HOME"]
来源：http://hz.smart0.xyz/gtccmtjkuj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.meibo888.top/gtnydprrof.html

[M03] 执行外部命令
来源：http://hz.dashuyun.cn/gtcgzromfg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.birdmap.top/gtmspfvazj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinghuilouyu.cn/gtmnaovgib.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.gotoacloud.top/gtvbawmkaz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ehwqpu.com/gtenadqjqq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zycfv.cn/gtyeahirjl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ybcxt.top/gttzbfacsk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xinyue.icu/gthdcvonvn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.svipenyu.cn/gtpivngbvu.html

[M04] 获取当前工作目录
来源：http://hz.guannengcc.top/gthgarrmyi.html

Py:   os.getcwd()
来源：http://hz.svipenyu.cn/gtmcxwujrs.html

PHP:  getcwd();
来源：http://hz.xinyue.icu/gtqczzmfkq.html

JS:   process.cwd()
来源：http://hz.xuetiantiany.cn/gtgjoyyiwl.html

TS:   process.cwd()
来源：http://hz.svipenyu.cn/gtmddiloeh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xingfuxueyuan.xyz/gtsenvylxt.html

Go:   os.Getwd()
来源：http://hz.sysykeji.top/gtuppvqeec.html

Ruby: Dir.pwd
来源：http://hz.xinyue.icu/gtyyhiqmvi.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.birdmap.top/gtwlufwfvi.html

[M05] 设置退出码
来源：http://hz.yongpay.top/gtwnfqewbx.html

Py:   sys.exit(1)
来源：http://hz.yanxiufei.cn/gtnagdgsul.html

PHP:  exit(1);
来源：http://hz.jinqigufen.top/gtqujiqpxt.html

JS:   process.exit(1)
来源：http://hz.nwbrower.top/gtbyfrjpkl.html

TS:   process.exit(1)
来源：http://hz.tanke756.top/gtgywnkujp.html

Java: System.exit(1)
来源：http://hz.yvedp.cn/gtpvfociqf.html

Go:   os.Exit(1)
来源：http://hz.ehwqpu.com/gtmwixmkht.html

Ruby: exit 1
来源：http://hz.daxiang520.top/gtzjbxvmxc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yongpay.top/gtkgjacwof.html

[M06] 向标准错误输出
来源：http://hz.c1oappe.top/gtosnjagqg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ywan-chungtsiang.top/gtdtzjabdh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yj20258.top/gtxrnimgwu.html

JS:   console.error("err")
来源：http://hz.yonumen.top/gtnvetfxma.html

TS:   console.error("err")
来源：http://hz.tanke756.top/gtbxddweau.html

Java: System.err.println("err")
来源：http://hz.zhongyouzk.top/gtpnxwfyqo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.fengsongda.top/gtvpdbkpqp.html

Ruby: warn "err"
来源：http://hz.yj20258888.top/gtwehsmazy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.fzhhl.top/gtgcirrhxu.html

[M07] 判断是否为主入口
来源：http://hz.pengpengdd.cyou/gtffnaglkj.html

Py:   if __name__ == "__main__":
来源：http://hz.xuanzx.com/gtikctmqwm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.guowangkeji.top/gtcaueeini.html

JS:   require.main === module
来源：http://hz.zhaomingkeji.xyz/gtjcmtrifo.html

TS:   require.main === module
来源：http://hz.fzhhl.top/gtbmhxtjha.html

Java: public static void main(String[] args)
来源：http://hz.tianlin.xyz/gtndrqfyut.html

Go:   func main()
来源：http://hz.pycfn.com/gtngbhgzyl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.dashuyun.cn/gttwwpxehg.html

C#:   static void Main(string[] args)
来源：http://hz.sufxvd.cn/gtqbpksttj.html

[M08] 获取系统与运行时信息
来源：http://hz.sufxvd.cn/gtytbilhkj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gotoacloud.top/gtbahgzkjt.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gogol.net.cn/gtqoiudjdr.html

JS:   process.platform;  process.version
来源：http://hz.9152youxi.cn/gtnzqqauhv.html

TS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtrtkvfrus.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.chenzaomai.com/gtjbgwhzrv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jqgufenzy.top/gtjuqyawrk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gotoacloud.top/gtggudfzin.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.quarkkingdee.top/gtvjfnksmi.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtiorasrxv.html

N. 数据结构与算法
来源：http://hz.ydjk.org.cn/gtjdjaxgye.html

================================================================================
来源：http://hz.iojbl.cn/gtzcpanojn.html

[N01] 二分查找（有序数组）
来源：http://hz.yangfankeji.com/gtfunwhrzh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.mhx1999.top/gtljvzdzlb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.daria6918.cn/gteaklqpbe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sysykeji.top/gtjqmoaupa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnxiangtu.top/gtfqrdwtcj.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zdqjudy.top/gtankjdcuo.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.redwolf501.top/gtffliamxu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xinyue.icu/gtctptvfvg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jianghu66.top/gtynvnbsmn.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.dashuyun.cn/gtnefgshxc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hnxiangtu.top/gtpbmilnjn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cashguo.top/gtjrkrwuqa.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.9152youxi.cn/gtifpffmjx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ydjk.org.cn/gtatnyqkow.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yanxiufei.cn/gtyxqpsedc.html

Go:   slices.Sort(arr)
来源：http://hz.xylfe.cn/gtufbnxpgl.html

Ruby: arr.sort
来源：http://hz.zhengqikj.top/gtewrpdxpe.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.birdmap.top/gtbrieghod.html

[N03] 快速排序（分治示例）
来源：http://hz.vqdsnc.cn/gtilpyeule.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shanyushiyangtech.top/gtvmpankvx.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yonumen.top/gtndjkjyhy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhijiandao.cn/gteziilpla.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tanke756.top/gtkpqfnzaq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.0kj1m.cn/gtrqnohdew.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.havefunace.top/gtbnyzhemt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xziqi.cn/gtzqzotiat.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhengqikj.top/gturkrlwta.html

[N04] 斐波那契数列
来源：http://hz.xinyue.icu/gtbcowqpky.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.smart0.xyz/gthojzsyzq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sysykeji.top/gtoaluxuvc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yongpay.top/gtgfcqsctv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigufen.top/gtmfkcphku.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hywenlv.cn/gtizzlfqil.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.tianlin.xyz/gtmyxmophu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xziqi.cn/gtwrokgdfh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.pengpengdd.cyou/gtmfjtgcwz.html

[N05] 最大公约数
来源：http://hz.jyoumei.cn/gtiqglscog.html

Py:   math.gcd(a, b)
来源：http://hz.jlsjyb.cn/gtwnnanysx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.fzhhl.top/gtxqczawwe.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.svipenyu.cn/gtmgvetqjs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pycfn.com/gthfabjclk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gaohongyu789.top/gtnnpfkuou.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.tianlin.xyz/gtsmxnwuxu.html

Ruby: a.gcd(b)
来源：http://hz.havefunace.top/gtxqshvxcg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.dianchejie.cn/gtuqtsbbil.html

[N06] 判断回文字符串
来源：http://hz.redwolf501.top/gtcnnfkasz.html

Py:   s == s[::-1]
来源：http://hz.havefunace.top/gtnpntsoco.html

PHP:  $s === strrev($s);
来源：http://hz.zhijiandao.cn/gtcsdeepou.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhixingplan.top/gtqqdmolol.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tanke756.top/gtmxmyemei.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.snrcjt.cn/gtibtgdnbm.html

Go:   // 双指针从两端比较
来源：http://hz.birdmap.top/gtvinfafgf.html

Ruby: s == s.reverse
来源：http://hz.cucudq.cn/gtmlolpbrp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhengqikj.top/gteadrhvji.html

[N07] 两数之和（返回下标）
来源：http://hz.guowangkeji.top/gttnesaxdt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.chenlongwang.top/gtvelobonn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gzhubu.top/gtcxbmuflp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hnxiangtu.top/gtcxvsngzt.html

TS:   // 手写 Map<string, number>
来源：http://hz.9152youxi.cn/gtzcvxxvri.html

Java: // 手写 HashMap
来源：http://hz.hongshengwenyu.top/gtjjlzccey.html

Go:   // 手写 map[int]int
来源：http://hz.xylfe.cn/gtfqubxmzl.html

Ruby: // 手写 Hash
来源：http://hz.meibo888.top/gtfogcacne.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yueranfly.top/gtnmnirocs.html

[N08] 生成全排列
来源：http://hz.kuanghao11.cn/gtjyzlpche.html

Py:   itertools.permutations(arr)
来源：http://hz.cqqwz.cn/gtfqbpxdah.html

PHP:  // 手写递归交换
来源：http://hz.yanxiufei.cn/gtzjxiescc.html

JS:   // 手写回溯递归
来源：http://hz.cheryme.top/gtyoyjvuxl.html

TS:   // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtgzmxdyqt.html

Java: // 手写回溯递归
来源：http://hz.ydzc1.top/gtujbkhllu.html

Go:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtwxbmlipe.html

Ruby: arr.permutation.to_a
来源：http://hz.c1oappe.top/gttudcuyyu.html

C#:   // 手写回溯递归
来源：http://hz.yj202588.top/gtztgulblh.html

[N09] 栈与队列
来源：http://hz.gaohongyu789.top/gttlkgjcqd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.guannengcc.top/gtdyequpol.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.birdmap.top/gtoqwjqeyv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhiwuduotai.top/gtyrckobiv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xziqi.cn/gtphvwazov.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.pengpengdd.cyou/gtwaswedmo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cdnleiting.top/gtqhohhidn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jqgfzy.top/gtvwurawek.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hammf.cn/gtrydeonmj.html

[N10] 链表节点定义
来源：http://hz.chenzaomai.com/gtogezchvx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.svipenyu.cn/gtoczlqsjy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.dashuyun.cn/gtapxsowrw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hammf.cn/gtvdqujjpc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yongpay.top/gtdqgatlkv.html

Java: class Node { int v; Node next; }
来源：http://hz.xylfe.cn/gtsorefelc.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.guannengcc.top/gtdoqtwwce.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hongshengwenyu.top/gtfkdlfjjv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.52xcode.cn/gtzhesmhll.html

[N11] 二叉树中序遍历
来源：http://hz.tianlin.xyz/gtvvabeajz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhiwuduotai.top/gtsjpyalgt.html

PHP:  // 手写递归函数
来源：http://hz.ivvv.top/gtlkckrifb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hysaishi.cn/gtrvwbezfi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gogol.net.cn/gtjafyehrt.html

Java: // 手写递归
来源：http://hz.svipenyu.cn/gtwugenogt.html

Go:   // 手写递归
来源：http://hz.sufxvd.cn/gtczuqcxgt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jinghuilouyu.cn/gtehyhuzls.html

C#:   // 手写递归
来源：http://hz.yueranfly.top/gtytuoapqx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yuxming.cn/gtllifdlva.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jlsjyb.cn/gtjewuvymq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ywan-chungtsiang.top/gtarapdbyv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgfzy.top/gttumirpsf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yangfankeji.com/gtnqhrjghy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinghuilouyu.cn/gtgcfketxj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.pengpengdd.cyou/gtbzrqkkpr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sxryk.cn/gtlglkpnwp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sufxvd.cn/gtopeiwhzo.html

================================================================================
来源：http://hz.nanxinkj.top/gtfaggkeeo.html

O. 并发与异步
来源：http://hz.zhengqikj.top/gtacuosgix.html

================================================================================
来源：http://hz.zycfv.cn/gthudgjwqr.html

[O01] 启动一个线程
来源：http://hz.mhx1999.top/gtfofoalal.html


<!-- 参考信息 -->