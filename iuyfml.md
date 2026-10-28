代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hfpthk.cn/gthwuxicze.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhengqikj.top/gtbcwnaehs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sxryk.cn/gtddmxvqfw.html

[K05] 深拷贝对象
来源：http://hz.sweek.top/gtqdolnpyb.html

Py:   copy.deepcopy(obj)
来源：http://hz.tianlin.xyz/gtyahltzys.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hfpthk.cn/gtmyzjisds.html

JS:   structuredClone(obj)
来源：http://hz.shzxlz.cn/gtvteexwtu.html

TS:   structuredClone(obj)
来源：http://hz.tian-w.cn/gtvijmmnwl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cqqwz.cn/gtldffctil.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenlongwang.top/gteghrojwh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.smart0.xyz/gtsagwqixq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.chenlongwang.top/gtclazdgwk.html

[K06] 解析 URL 查询串
来源：http://hz.nwbrower.top/gtfaturton.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.wangshuangyany.cn/gttjsbqyhm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jianghu66.top/gtgqomrusx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xingfuxueyuan.xyz/gtoeddaidf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yangfankeji.com/gtjiudrndz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shanyushiyangtech.top/gtekmkjseb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xuetiantiany.cn/gtuhvcsovy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.birdmap.top/gtgpuvgarm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhiwuduotai.top/gtttreexai.html

[K07] 进制转换
来源：http://hz.hnqzz.top/gtyemucdvh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.chenjidiqi.icu/gtidnsemot.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xylfe.cn/gtvdesryrm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.9152youxi.cn/gtbdenznwy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yuanzhike.top/gtwyyrzwaf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yj202588.top/gtmvlbquch.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yonumen.top/gtgwnpvphu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nanxinkj.top/gthroacofb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shuidangran.top/gtszfvkxsu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.havefunace.top/gtrpkoyyyb.html

Py:   pickle.dumps(obj)
来源：http://hz.zhongyouzk.top/gtqecbedzo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhongyouzk.top/gtqkzgtqsr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gotoacloud.top/gtvbyvvtju.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hysaishi.cn/gtpyvsajkq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenjidiqi.icu/gtgqauvwsj.html

Go:   encoding/gob
来源：http://hz.zdqjudy.top/gtocqyfuuy.html

Ruby: Marshal.dump(obj)
来源：http://hz.sweek.top/gtuybkmfdm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.andypj.xyz/gtbxcblmwb.html

================================================================================
来源：http://hz.xuanzx.com/gtjzzyeyuf.html

L. 网络请求
来源：http://hz.iojbl.cn/gtvkkbayov.html

================================================================================
来源：http://hz.jlsjyb.cn/gtizqduudu.html

[L01] 发送 GET 请求
来源：http://hz.shangyingyoupin.top/gtbldnogrq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.wangshuangyany.cn/gtkzdabcvh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jqgfzy.top/gtccfrrlqf.html

JS:   await fetch(url)
来源：http://hz.guowangkeji.top/gtgoqpbafq.html

TS:   await fetch(url)
来源：http://hz.hnxiangtu.top/gtxpyngshn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xinyue.icu/gtmrxmebmh.html

Go:   resp, err := http.Get(url)
来源：http://hz.xylfe.cn/gtfxlqweju.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.fengsongda.top/gtbwuirrjo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.vqdsnc.cn/gtxukdajkl.html

[L02] 发送 POST JSON
来源：http://hz.sysykeji.top/gtdpyyyval.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hongshengwenyu.top/gtjzukjntp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yj202588.top/gttokoixfs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pycfn.com/gtbpihtnzj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zycfv.cn/gtcbtmuzli.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yueranfly.top/gtnewuttlu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zdqjudy.top/gtokoboobl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.gzhubu.top/gtchyfokmo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.c1oappe.top/gtyuxnbbon.html

[L03] 设置自定义请求头
来源：http://hz.dashuyun.cn/gtbniuzzwe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.pengpengdd.cyou/gtzjrfuyqt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hfpthk.cn/gtjnqehxhu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhengqikj.top/gtrqwxbbni.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sufxvd.cn/gthtlqyxxr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.svipenyu.cn/gtmdcwaaho.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yueranfly.top/gtcwunuute.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhaomingkeji.xyz/gtsnvtsxjr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhijiandao.cn/gttkmjtvlk.html

[L04] 设置超时
来源：http://hz.iojbl.cn/gtaiewuehh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhongyouzk.top/gtpgdxxfme.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.vqdsnc.cn/gteaxovlsz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yueranfly.top/gtuuhxnzfq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhiwuduotai.top/gtpwblfqck.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.nanxuanxn.top/gtqmtyayei.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhixingplan.top/gtyyhwpwmk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tanke756.top/gtafniohpa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinqigfzy.top/gtbchvgjnw.html

[L05] 上传文件（multipart）
来源：http://hz.hammf.cn/gtvyabbdaj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.sufxvd.cn/gtvyfwvfwq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.kuanghao11.cn/gtwfbzjceh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhiwuduotai.top/gtvplwdmvb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cheryme.top/gtqvfrolfr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.pengpengdd.cyou/gtjgjfvyqi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.9152youxi.cn/gtstjprivk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.svipenyu.cn/gtvngvsiei.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhaomingkeji.xyz/gtzvpvfupp.html

[L06] 解析响应为 JSON
来源：http://hz.aibaodan.cn/gtcswahewl.html

Py:   resp.json()
来源：http://hz.dianchejie.cn/gtjkfpcngy.html

PHP:  json_decode($body, true);
来源：http://hz.zhijiandao.cn/gtpalmskpf.html

JS:   await resp.json()
来源：http://hz.gaohongyu789.top/gtwkkaztgs.html

TS:   await resp.json()
来源：http://hz.yongpay.top/gtxecvjdly.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ybcxt.top/gtemxjyrsa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jiagoushi.top/gtrmbcouhh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.quarkkingdee.top/gtsvhimwrp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.andypj.xyz/gtmmxgvvuz.html

[L07] 处理 HTTP 状态码
来源：http://hz.shuidangran.top/gtzmojvdyu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.nwbrower.top/gtuloadqyr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj20258.top/gtmoybygdx.html

JS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gthgkqduez.html

TS:   resp.ok;  resp.status
来源：http://hz.vqdsnc.cn/gtjauykxlg.html

Java: resp.statusCode()
来源：http://hz.yuxming.cn/gtboiuiexv.html

Go:   resp.StatusCode
来源：http://hz.nanxinkj.top/gtcuukftvj.html

Ruby: resp.code.to_i
来源：http://hz.ybcxt.top/gtwyyrtlsw.html

C#:   (int)resp.StatusCode
来源：http://hz.meibo888.top/gtbmutnisx.html

[L08] 并发请求多个地址
来源：http://hz.zhaomingkeji.xyz/gtnodhxztz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hnqzz.top/gtndlodavo.html

PHP:  curl_multi_init() 系列
来源：http://hz.pycfn.com/gtxnqtfpjz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.feifeiyinyue.top/gtxphqoffh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zdqjudy.top/gtqahhnzxi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tianlin.xyz/gtjlzaktzv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yvedp.cn/gtndytrdrt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cashguo.top/gtqgivrcmq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ehwqpu.com/gtfjbigufk.html

================================================================================
来源：http://hz.sufxvd.cn/gtheznaple.html

M. 命令行 / 进程 / 环境
来源：http://hz.yuxming.cn/gtbmngbgfe.html

================================================================================
来源：http://hz.zdqjudy.top/gtcfcjcoxg.html

[M01] 读取命令行参数
来源：http://hz.snrcjt.cn/gtjjjivltg.html

Py:   sys.argv[1:]
来源：http://hz.zhengqikj.top/gtfpvehbnx.html

PHP:  $argv;  $argc;
来源：http://hz.cheryme.top/gtnmjtpqzi.html

JS:   process.argv.slice(2)
来源：http://hz.yanxiufei.cn/gtjjizvaeq.html

TS:   process.argv.slice(2)
来源：http://hz.shanyushiyangkeji.top/gtvikkbiwl.html

Java: args 数组（main 方法参数）
来源：http://hz.gotoacloud.top/gtmkhctrdh.html

Go:   os.Args[1:]
来源：http://hz.nanxinkj.top/gtzbvcdimj.html

Ruby: ARGV
来源：http://hz.feifeiyinyue.top/gtkjxunruv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.52xcode.cn/gtsafticiv.html

[M02] 读取环境变量
来源：http://hz.shuidangran.top/gtxzxakqbc.html

Py:   os.environ.get("HOME")
来源：http://hz.cucudq.cn/gtkoceprqu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhoulong.xyz/gtscrcskvp.html

JS:   process.env.HOME
来源：http://hz.jianghu66.top/gtzkcdfldw.html

TS:   process.env.HOME
来源：http://hz.zhongyouzk.top/gtqzplccji.html

Java: System.getenv("HOME")
来源：http://hz.0kj1m.cn/gthocedgzd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhijiandao.cn/gtialanloa.html

Ruby: ENV["HOME"]
来源：http://hz.dianchejie.cn/gtjwkrefgz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.mhx1999.top/gtmuvjyvdv.html

[M03] 执行外部命令
来源：http://hz.zhixingplan.top/gtntzatwjm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yueranfly.top/gttgvnenoi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jyoumei.cn/gthwpweafe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.svipenyu.cn/gtqkxdsxfq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhengqikj.top/gtsexvvhcr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj20258888.top/gthsdrcsmn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhijiandao.cn/gtxssdezcx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jqgufenzy.top/gtquhdierb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.dianchejie.cn/gtiolrrfos.html

[M04] 获取当前工作目录
来源：http://hz.feifeiyinyue.top/gtfvnvntpo.html

Py:   os.getcwd()
来源：http://hz.chenzaomai.com/gtclptvlox.html

PHP:  getcwd();
来源：http://hz.jqgufenzy.top/gtkmtxjihp.html

JS:   process.cwd()
来源：http://hz.svipenyu.cn/gtzklntavy.html

TS:   process.cwd()
来源：http://hz.yangfankeji.com/gtnfsijclp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jqgfzy.top/gttnmgvqxk.html

Go:   os.Getwd()
来源：http://hz.xuanzx.com/gtomlzjxrf.html

Ruby: Dir.pwd
来源：http://hz.yj20258888.top/gtuifkofyl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.nanxuanxn.top/gtrtfffvmh.html

[M05] 设置退出码
来源：http://hz.xziqi.cn/gtypuwfbrx.html

Py:   sys.exit(1)
来源：http://hz.jinyuanbaomall.cn/gthyoznlpd.html

PHP:  exit(1);
来源：http://hz.hywenlv.cn/gtxagjgjkc.html

JS:   process.exit(1)
来源：http://hz.cheryme.top/gtniqycuub.html

TS:   process.exit(1)
来源：http://hz.zhongyouzk.top/gtptglthxz.html

Java: System.exit(1)
来源：http://hz.hfpthk.cn/gtzyzbsrtw.html

Go:   os.Exit(1)
来源：http://hz.havefunace.top/gtemeomila.html

Ruby: exit 1
来源：http://hz.tianlin.xyz/gtnuzmxhkv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shzxlz.cn/gtcatqsfbh.html

[M06] 向标准错误输出
来源：http://hz.daria6918.cn/gtzcofalee.html

Py:   print("err", file=sys.stderr)
来源：http://hz.svipenyu.cn/gtcelktfwa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zdqjudy.top/gtcyzfotty.html

JS:   console.error("err")
来源：http://hz.nwbrower.top/gtgopfqscd.html

TS:   console.error("err")
来源：http://hz.jlsjyb.cn/gtzjfeoofy.html

Java: System.err.println("err")
来源：http://hz.yuxming.cn/gtehmqihve.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xylfe.cn/gtkjwzstqp.html

Ruby: warn "err"
来源：http://hz.zhongyouzk.top/gtjslijfmu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.fengsongda.top/gtgxesvwnp.html

[M07] 判断是否为主入口
来源：http://hz.chenzaomai.com/gtzubuciwl.html

Py:   if __name__ == "__main__":
来源：http://hz.jqgufenzy.top/gtspfiocph.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.nwbrower.top/gtwbhteofl.html

JS:   require.main === module
来源：http://hz.gzhubu.top/gtflamzrmt.html

TS:   require.main === module
来源：http://hz.ywan-chungtsiang.top/gtagumccjm.html

Java: public static void main(String[] args)
来源：http://hz.cdnleiting.top/gtcgsmrrty.html

Go:   func main()
来源：http://hz.xingfuxueyuan.xyz/gtfvwojszd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jiagoushi.top/gtuxawwnkq.html

C#:   static void Main(string[] args)
来源：http://hz.xinyue.icu/gtvjnpvimn.html

[M08] 获取系统与运行时信息
来源：http://hz.zdqjudy.top/gteoblnfcp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.316326.xyz/gtimplhefw.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.nwbrower.top/gtotrxrqnr.html

JS:   process.platform;  process.version
来源：http://hz.tianlin.xyz/gtrssmtfrn.html

TS:   process.platform;  process.version
来源：http://hz.kuanghao11.cn/gtlhtgppat.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cashguo.top/gtfbuuogcn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sysykeji.top/gtzesywocx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gzhubu.top/gtymdjmsyq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.tianlin.xyz/gtndbapdqj.html

================================================================================
来源：http://hz.xinyue.icu/gtjtsedqbq.html

N. 数据结构与算法
来源：http://hz.bjfxy.top/gtgsuohvwr.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtsylijgiw.html

[N01] 二分查找（有序数组）
来源：http://hz.redwolf501.top/gtwwvngvqn.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.vqdsnc.cn/gtfedwapdq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.0kj1m.cn/gtstroiram.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tanke756.top/gtnjtqxywv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinyuanbaomall.cn/gtevtsgefy.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jinqigfzy.top/gtlfrjrlbz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.sufxvd.cn/gtxxbubffs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.tian-w.cn/gthrjinwsn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ppjwa.cn/gtiwmkudkc.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ydjk.org.cn/gtrrosmimh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.redwolf501.top/gtahydkbxa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.pengpengdd.cyou/gtwlkiiosj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhijiandao.cn/gtkbidlynt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ybcxt.top/gtyserhkwl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cdnleiting.top/gtljafylsm.html

Go:   slices.Sort(arr)
来源：http://hz.cheryme.top/gtgalgynnh.html

Ruby: arr.sort
来源：http://hz.zhijiandao.cn/gtksjxmdis.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xziqi.cn/gtzrusazag.html

[N03] 快速排序（分治示例）
来源：http://hz.shanyushiyangkeji.top/gtavbmbrhz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shanyushiyangkeji.top/gtmqisxgbu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sweek.top/gttuptkqrx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.vqdsnc.cn/gtuucsfuif.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jiagoushi.top/gtxlgmsxvx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cheryme.top/gtueqmnkep.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.havefunace.top/gtpgixvaba.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.daria6918.cn/gtjdefislo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.smart0.xyz/gtqpfkyepu.html

[N04] 斐波那契数列
来源：http://hz.sysykeji.top/gtdezishez.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.iojbl.cn/gtmlhwwtxw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.iojbl.cn/gtmhckbltw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhongyouzk.top/gtbribtosw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.quarkkingdee.top/gtfwgwopqf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xuanzx.com/gtkieogyiy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ydjk.org.cn/gtrswbyajk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.wangdashe.top/gtmfpravro.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhongyouzk.top/gtcmoddfij.html

[N05] 最大公约数
来源：http://hz.meibo888.top/gtpupzmati.html

Py:   math.gcd(a, b)
来源：http://hz.zhaomingkeji.xyz/gtlwveywny.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinqigufen.top/gtvaeamdwl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.kuanghao11.cn/gtxsydxjeh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.havefunace.top/gtqfxkjeht.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.bjfxy.top/gtqnygcior.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhoulong.xyz/gtemwedjog.html

Ruby: a.gcd(b)
来源：http://hz.jlsjyb.cn/gtbjemvsya.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.tanke756.top/gtfkebsaga.html

[N06] 判断回文字符串
来源：http://hz.shzxlz.cn/gtdfgesmid.html

Py:   s == s[::-1]
来源：http://hz.hfpthk.cn/gtgrqvjbbu.html

PHP:  $s === strrev($s);
来源：http://hz.yueranfly.top/gtiiybsmxh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtidzwapfq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gtjktvumxb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.gzhubu.top/gtqljlmccw.html

Go:   // 双指针从两端比较
来源：http://hz.jiagoushi.top/gtxymikciv.html

Ruby: s == s.reverse
来源：http://hz.hysaishi.cn/gtnkcnvxzf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yuxming.cn/gtlmytfhhd.html

[N07] 两数之和（返回下标）
来源：http://hz.zhoulong.xyz/gttpombcxk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xziqi.cn/gtaqjhgosy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.haohaochexian.top/gtaamzowgq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xylfe.cn/gthrmmklok.html

TS:   // 手写 Map<string, number>
来源：http://hz.cashguo.top/gtepoyrinv.html

Java: // 手写 HashMap
来源：http://hz.nanxuanxn.top/gtpelvpgec.html

Go:   // 手写 map[int]int
来源：http://hz.birdmap.top/gtvzaewckq.html

Ruby: // 手写 Hash
来源：http://hz.xuanzx.com/gtemgyghei.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gaohongyu789.top/gtdgmeaxrb.html

[N08] 生成全排列
来源：http://hz.jlsjyb.cn/gtkxnagviy.html

Py:   itertools.permutations(arr)
来源：http://hz.hammf.cn/gtdixbckjy.html

PHP:  // 手写递归交换
来源：http://hz.birdmap.top/gtsxnsfavz.html

JS:   // 手写回溯递归
来源：http://hz.xinyue.icu/gthitqluuy.html

TS:   // 手写回溯递归
来源：http://hz.jqgfzy.top/gtyhsonvrv.html

Java: // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtdoqlgzsp.html

Go:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtndldbijx.html

Ruby: arr.permutation.to_a
来源：http://hz.cheryme.top/gtydhpxzau.html

C#:   // 手写回溯递归
来源：http://hz.ivvv.top/gtqtvimllw.html

[N09] 栈与队列
来源：http://hz.sufxvd.cn/gtyvdsrmng.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yangfankeji.com/gtsquqbzkc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.iojbl.cn/gtiotepczf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.52xcode.cn/gtacvpfult.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhengqikj.top/gtkvmoanuh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.tianlin.xyz/gthxwvndak.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhijiandao.cn/gtaflpddaw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.bjfxy.top/gtekoisgve.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gotoacloud.top/gtnswmqvge.html

[N10] 链表节点定义
来源：http://hz.gaohongyu789.top/gtpuwisxcq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hammf.cn/gtidvzysee.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.9152youxi.cn/gtxatvahqv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.redwolf501.top/gtcxmppfwc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.mhx1999.top/gtyzubhksy.html

Java: class Node { int v; Node next; }
来源：http://hz.ivvv.top/gtxcgmfmmt.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yongpay.top/gtiqsffyqk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zdqjudy.top/gtcxucpigm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xuanzx.com/gtjmxiistk.html

[N11] 二叉树中序遍历
来源：http://hz.shangyingyoupin.top/gtmfixmptu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hnxiangtu.top/gtbedxtqyv.html

PHP:  // 手写递归函数
来源：http://hz.aizwys.cn/gtrdrldnav.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yongpay.top/gtmehzkrbh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgfzy.top/gtmczovygz.html

Java: // 手写递归
来源：http://hz.zhixingplan.top/gtjxigcmgs.html

Go:   // 手写递归
来源：http://hz.gogol.net.cn/gtirioecri.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jqgufenzy.top/gtslyceykb.html

C#:   // 手写递归
来源：http://hz.ywan-chungtsiang.top/gtarhulodk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.sxryk.cn/gtrkqjgpau.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ydjk.org.cn/gteqzijzwl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gogol.net.cn/gtxgcaldcf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenzaomai.com/gtyltojfve.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangshuangyany.cn/gtnkphuiyg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.daria6918.cn/gtavrrsqvg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhijiandao.cn/gtavwzxyvx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hongshengwenyu.top/gtxwgufxzs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.meibo888.top/gtuhfampoh.html


<!-- 参考信息 -->