代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ywan-chungtsiang.top/gtwkixwryl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.guowangkeji.top/gtdntrylin.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ivvv.top/gtchwspbkp.html

[K05] 深拷贝对象
来源：http://hz.zhengqikj.top/gtuvllnpne.html

Py:   copy.deepcopy(obj)
来源：http://hz.0kj1m.cn/gtaiagcaom.html

PHP:  unserialize(serialize($obj));
来源：http://hz.0kj1m.cn/gtluwfupds.html

JS:   structuredClone(obj)
来源：http://hz.daria6918.cn/gtxjnxjdjw.html

TS:   structuredClone(obj)
来源：http://hz.zhoulong.xyz/gtcijjmsgv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jyoumei.cn/gtzuqjhnvv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.guannengcc.top/gtdcdfeufp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ivvv.top/gtwoctfsjx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jyoumei.cn/gtyvnjmjeh.html

[K06] 解析 URL 查询串
来源：http://hz.kuanghao11.cn/gtzneasutw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jqgfzy.top/gtfklksjwz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cheryme.top/gtzfrckcsp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gaohongyu789.top/gtwzrwezvt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.feifeiyinyue.top/gtmzcilfjf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.vqdsnc.cn/gtrnudxeed.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.wangshuangyany.cn/gtzehonmgc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xingfuxueyuan.xyz/gtrpdnzozd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yj20258888.top/gtxingurgg.html

[K07] 进制转换
来源：http://hz.andypj.xyz/gtazrykxuh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.iojbl.cn/gtlkhsdfgg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zycfv.cn/gthotbjfzx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gttzyxrmfy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cqqwz.cn/gtrddzzzob.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xuetiantiany.cn/gtplnpcvcg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jiagoushi.top/gtsfwplssl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sxryk.cn/gtrmphjvqb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jlsjyb.cn/gtmsfklidr.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.tanke756.top/gtvtbivqzl.html

Py:   pickle.dumps(obj)
来源：http://hz.zycfv.cn/gtpvpcecoh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.dashuyun.cn/gtnlydmaqr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yonumen.top/gtpgvrqhrg.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ybcxt.top/gtmibbqpdg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.c1oappe.top/gtozmmjsrj.html

Go:   encoding/gob
来源：http://hz.iojbl.cn/gtigiynszf.html

Ruby: Marshal.dump(obj)
来源：http://hz.yangfankeji.com/gtiwrtujqr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhijiandao.cn/gtsubojaxd.html

================================================================================
来源：http://hz.hnqzz.top/gtregqpjkz.html

L. 网络请求
来源：http://hz.snrcjt.cn/gtvjanmvmx.html

================================================================================
来源：http://hz.zhixingplan.top/gtxgigggdl.html

[L01] 发送 GET 请求
来源：http://hz.dianchejie.cn/gtspqybfxw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.andypj.xyz/gtqjstlktj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinghuilouyu.cn/gtyvzgklzk.html

JS:   await fetch(url)
来源：http://hz.zhixingplan.top/gttvyruoho.html

TS:   await fetch(url)
来源：http://hz.yj20258.top/gtahoenirr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jqgufenzy.top/gtkbmnmxxv.html

Go:   resp, err := http.Get(url)
来源：http://hz.svipenyu.cn/gtdrnvjbii.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.guannengcc.top/gtvlvzoqof.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhaomingkeji.xyz/gtjrmdcpdo.html

[L02] 发送 POST JSON
来源：http://hz.yj20258.top/gtltdpicwf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jinqigufen.top/gtqvgwdezo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhaomingkeji.xyz/gtitbwlgha.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gaohongyu789.top/gtljnkwdlk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnxiangtu.top/gtexvcnibe.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zycfv.cn/gtkelhzalr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yangfankeji.com/gthwrwwbfo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.chenzaomai.com/gtednkcoss.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.redwolf501.top/gtkksjboll.html

[L03] 设置自定义请求头
来源：http://hz.ppjwa.cn/gtxutokvqf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.redwolf501.top/gtfxlaeltu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ivvv.top/gtestyrlmr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangdashe.top/gtzzjnscrd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.haohaochexian.top/gtltstbbyu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cucudq.cn/gtlzohwmkl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.fzhhl.top/gtrjrfvjvh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhoulong.xyz/gtdhopocyc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.daria6918.cn/gtljagvvfg.html

[L04] 设置超时
来源：http://hz.jyoumei.cn/gtisskjrik.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhengqikj.top/gtmhtivsdn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jqgufenzy.top/gtvgehqzfd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cqqwz.cn/gtvgohpumw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cashguo.top/gttzgcgnyk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.fzhhl.top/gtsfzocfsp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xuetiantiany.cn/gtvcfljzba.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yongpay.top/gtkqpxeyex.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yj20258.top/gttcdjixth.html

[L05] 上传文件（multipart）
来源：http://hz.shangyingyoupin.top/gttixkyhyk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj202588.top/gtyrtgqkgx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.wangshuangyany.cn/gtxgyipuyh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shangyingyoupin.top/gtfboterzs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangdashe.top/gtxdorhuug.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shuidangran.top/gtnobwullw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.smart0.xyz/gtfhtwxwaq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yuxming.cn/gtrvzzxcwv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.daxiang520.top/gtddqfxlyn.html

[L06] 解析响应为 JSON
来源：http://hz.dashuyun.cn/gtxyzequfr.html

Py:   resp.json()
来源：http://hz.vqdsnc.cn/gtyhiteusv.html

PHP:  json_decode($body, true);
来源：http://hz.yongpay.top/gtzjfejnud.html

JS:   await resp.json()
来源：http://hz.sweek.top/gtehvfiyqe.html

TS:   await resp.json()
来源：http://hz.hammf.cn/gtvstuxcic.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gotoacloud.top/gtfnjsqlmp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.fengsongda.top/gtazxopljg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cucudq.cn/gtpzknwafj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.gzhubu.top/gtvzkajcbg.html

[L07] 处理 HTTP 状态码
来源：http://hz.ivvv.top/gtjzdqlxlk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shuidangran.top/gtmelcbjxp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hnqzz.top/gtyxqlrnxr.html

JS:   resp.ok;  resp.status
来源：http://hz.chenjidiqi.icu/gtshlpenqp.html

TS:   resp.ok;  resp.status
来源：http://hz.chenlongwang.top/gticelmghj.html

Java: resp.statusCode()
来源：http://hz.zycfv.cn/gtypzfymic.html

Go:   resp.StatusCode
来源：http://hz.tianlin.xyz/gtzwqubllo.html

Ruby: resp.code.to_i
来源：http://hz.kuanghao11.cn/gtrdddlnje.html

C#:   (int)resp.StatusCode
来源：http://hz.gaohongyu789.top/gtwcaaofgj.html

[L08] 并发请求多个地址
来源：http://hz.bjfxy.top/gtawvivnak.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ywan-chungtsiang.top/gtfkboeomw.html

PHP:  curl_multi_init() 系列
来源：http://hz.nanxuanxn.top/gtbtgwmebi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.smart0.xyz/gtaigfczac.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258.top/gteizfrmef.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shanyushiyangtech.top/gttigymfmt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhengqikj.top/gthraxvthl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhaomingkeji.xyz/gtgliumlmw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.pycfn.com/gtarrllbwr.html

================================================================================
来源：http://hz.jianghu66.top/gtkyqmdzcg.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhiwuduotai.top/gtpagesgwm.html

================================================================================
来源：http://hz.c1oappe.top/gtuwqkyeis.html

[M01] 读取命令行参数
来源：http://hz.dianchejie.cn/gtwgbtmley.html

Py:   sys.argv[1:]
来源：http://hz.yueranfly.top/gtbbxnqbdh.html

PHP:  $argv;  $argc;
来源：http://hz.yuanzhike.top/gtzzpujexa.html

JS:   process.argv.slice(2)
来源：http://hz.pengpengdd.cyou/gtcemtlxzb.html

TS:   process.argv.slice(2)
来源：http://hz.jiagoushi.top/gttilqwofm.html

Java: args 数组（main 方法参数）
来源：http://hz.yuxming.cn/gtixopzxmg.html

Go:   os.Args[1:]
来源：http://hz.daria6918.cn/gtnmmotxvz.html

Ruby: ARGV
来源：http://hz.sweek.top/gtowhmxmmh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.tianlin.xyz/gtzvwhtvho.html

[M02] 读取环境变量
来源：http://hz.yj202588.top/gtppythckv.html

Py:   os.environ.get("HOME")
来源：http://hz.tanke756.top/gtydrwhyfz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.tanke756.top/gtafxvjmhf.html

JS:   process.env.HOME
来源：http://hz.ydjk.org.cn/gtiprhdqwn.html

TS:   process.env.HOME
来源：http://hz.guowangkeji.top/gteugidvcg.html

Java: System.getenv("HOME")
来源：http://hz.xuanzx.com/gtparognee.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jyoumei.cn/gtmzzcssio.html

Ruby: ENV["HOME"]
来源：http://hz.xziqi.cn/gtiklczloj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zycfv.cn/gtsftjqutx.html

[M03] 执行外部命令
来源：http://hz.ehwqpu.com/gtphabqiqu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.pengpengdd.cyou/gtlozrwypw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gogol.net.cn/gtdtuzkakw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cdnleiting.top/gthmrtqjdc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.guannengcc.top/gtpzqxpjai.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.haohaochexian.top/gtlyylhrwm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hysaishi.cn/gtptctfvgt.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.pengpengdd.cyou/gtsewvfezl.html

C#:   Process.Start("ls", "-l");
来源：http://hz.havefunace.top/gtyojcaemj.html

[M04] 获取当前工作目录
来源：http://hz.tanke756.top/gtxsbclnky.html

Py:   os.getcwd()
来源：http://hz.ybcxt.top/gtykomyefx.html

PHP:  getcwd();
来源：http://hz.bjfxy.top/gtngpmhffo.html

JS:   process.cwd()
来源：http://hz.cashguo.top/gtcbdgifit.html

TS:   process.cwd()
来源：http://hz.9152youxi.cn/gtxsmrwkaw.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cheryme.top/gtebfkhaew.html

Go:   os.Getwd()
来源：http://hz.haohaochexian.top/gtgkagwwkw.html

Ruby: Dir.pwd
来源：http://hz.hammf.cn/gtgolbirfi.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xylfe.cn/gtlnwaurxk.html

[M05] 设置退出码
来源：http://hz.hnxiangtu.top/gtgatcqfkt.html

Py:   sys.exit(1)
来源：http://hz.dianchejie.cn/gtcarslwrd.html

PHP:  exit(1);
来源：http://hz.9152youxi.cn/gtdwqlufka.html

JS:   process.exit(1)
来源：http://hz.zhijiandao.cn/gtlcdbbvwr.html

TS:   process.exit(1)
来源：http://hz.sysykeji.top/gtsjrwmjlw.html

Java: System.exit(1)
来源：http://hz.yj20258888.top/gtcpojljgs.html

Go:   os.Exit(1)
来源：http://hz.shzxlz.cn/gttbblsqcn.html

Ruby: exit 1
来源：http://hz.ehwqpu.com/gtibrrwyyx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.aibaodan.cn/gtemrzebpr.html

[M06] 向标准错误输出
来源：http://hz.ivvv.top/gtrdezdtqa.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yj20258888.top/gtwtwvrmjd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yj20258.top/gtnbuwbpfv.html

JS:   console.error("err")
来源：http://hz.chenlongwang.top/gtmywylvzb.html

TS:   console.error("err")
来源：http://hz.birdmap.top/gtqoqgtwdk.html

Java: System.err.println("err")
来源：http://hz.xylfe.cn/gttnhpfbkw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.mhx1999.top/gtfakvywra.html

Ruby: warn "err"
来源：http://hz.ppjwa.cn/gtqajearve.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.dianchejie.cn/gtswexzwza.html

[M07] 判断是否为主入口
来源：http://hz.gzhubu.top/gttmxreofv.html

Py:   if __name__ == "__main__":
来源：http://hz.0kj1m.cn/gtttehnonk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinqigufen.top/gtywalnbha.html

JS:   require.main === module
来源：http://hz.cucudq.cn/gtsskqcquw.html

TS:   require.main === module
来源：http://hz.daxiang520.top/gtqimwmiwz.html

Java: public static void main(String[] args)
来源：http://hz.redwolf501.top/gtnqegdyik.html

Go:   func main()
来源：http://hz.hysaishi.cn/gtroxikelk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.birdmap.top/gtanuhrdvk.html

C#:   static void Main(string[] args)
来源：http://hz.0kj1m.cn/gtxhipghag.html

[M08] 获取系统与运行时信息
来源：http://hz.nanxinkj.top/gtqnajwuts.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zycfv.cn/gtbtlbmral.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ivvv.top/gtinkusdfd.html

JS:   process.platform;  process.version
来源：http://hz.cqqwz.cn/gtrzsdekqq.html

TS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtrcgaiqso.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shuidangran.top/gtxanbwvdj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sxryk.cn/gthlbgzadc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhoulong.xyz/gtbdhjppms.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sysykeji.top/gtlafpgquq.html

================================================================================
来源：http://hz.gaohongyu789.top/gtstshbogp.html

N. 数据结构与算法
来源：http://hz.ivvv.top/gtpalfvfjh.html

================================================================================
来源：http://hz.gaohongyu789.top/gtznvhpjmu.html

[N01] 二分查找（有序数组）
来源：http://hz.jinqigufen.top/gtafmwroes.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yuxming.cn/gtmtbpobro.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.bjfxy.top/gtunxuafsq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jianghu66.top/gtwbjisbzp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.52xcode.cn/gtmdyweqzs.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ehwqpu.com/gtbazspfek.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gogol.net.cn/gtdshrpjym.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.pycfn.com/gtncphdlsj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xinyue.icu/gtcablcxko.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xinyue.icu/gtuggvojtc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.bjfxy.top/gtqzlixiti.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yongpay.top/gtgwmflsis.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj202588.top/gtczvashin.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sxryk.cn/gtzexyojhz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.gaohongyu789.top/gtxnlpobcl.html

Go:   slices.Sort(arr)
来源：http://hz.hnqzz.top/gtgckkrkbj.html

Ruby: arr.sort
来源：http://hz.ydzc1.top/gtjggcarjd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.gogol.net.cn/gtthgnygwy.html

[N03] 快速排序（分治示例）
来源：http://hz.hywenlv.cn/gtcmbmvrvu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.fengsongda.top/gtxdhcyrcq.html

PHP:  // 递归实现，或用 usort
来源：http://hz.havefunace.top/gtuplhnyog.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.fzhhl.top/gtxjotwazj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gotoacloud.top/gtpijgoehx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ivvv.top/gtvxgoupji.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cheryme.top/gtbrykmfup.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.52xcode.cn/gtvadvheoz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yongpay.top/gtgjozqlzo.html

[N04] 斐波那契数列
来源：http://hz.dianchejie.cn/gtvgtnziuz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jlsjyb.cn/gtezhvtfsw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.redwolf501.top/gtiubdxsmu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daxiang520.top/gtozudfxci.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.redwolf501.top/gtjtpwoiaa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.52xcode.cn/gtjhuzfkun.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.quarkkingdee.top/gtbdlfghxz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ybcxt.top/gthrmykkwu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yuxming.cn/gttxanlzxx.html

[N05] 最大公约数
来源：http://hz.smart0.xyz/gtdxibbfrb.html

Py:   math.gcd(a, b)
来源：http://hz.tanke756.top/gteplfwwqf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.andypj.xyz/gtnwsiwycv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj20258.top/gtxklqomvp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.svipenyu.cn/gtestpqwhv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.316326.xyz/gtovjdarwi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cashguo.top/gtkmhfboau.html

Ruby: a.gcd(b)
来源：http://hz.zhijiandao.cn/gtouzdopxg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinqigufen.top/gtqazzzfom.html

[N06] 判断回文字符串
来源：http://hz.gaohongyu789.top/gtdsbgqdfd.html

Py:   s == s[::-1]
来源：http://hz.jinqigufen.top/gthobkjwbv.html

PHP:  $s === strrev($s);
来源：http://hz.xingfuxueyuan.xyz/gtsqtnfear.html

JS:   s === [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gtspzfffzk.html

TS:   s === [...s].reverse().join("")
来源：http://hz.pycfn.com/gtewlstegu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.tianlin.xyz/gtqnpumdau.html

Go:   // 双指针从两端比较
来源：http://hz.ppjwa.cn/gtcuwpkyqx.html

Ruby: s == s.reverse
来源：http://hz.c1oappe.top/gtqmlknxzh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ivvv.top/gtdgpunisp.html

[N07] 两数之和（返回下标）
来源：http://hz.nanxuanxn.top/gtrvsndkqr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinqigfzy.top/gtikywizpa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xuetiantiany.cn/gtswqepqyz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xinyue.icu/gtqafqhjdz.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj202588.top/gtklarabxv.html

Java: // 手写 HashMap
来源：http://hz.yj202588.top/gtudwdzlaw.html

Go:   // 手写 map[int]int
来源：http://hz.xylfe.cn/gtynsizkir.html

Ruby: // 手写 Hash
来源：http://hz.wangdashe.top/gtmzgvxeih.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yuanzhike.top/gtipocmmda.html

[N08] 生成全排列
来源：http://hz.tianlin.xyz/gtngrqglvz.html

Py:   itertools.permutations(arr)
来源：http://hz.xylfe.cn/gtlqljcvja.html

PHP:  // 手写递归交换
来源：http://hz.zhoulong.xyz/gtchxeoiqg.html

JS:   // 手写回溯递归
来源：http://hz.jqgufenzy.top/gtvsepxpqv.html

TS:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtgcownugl.html

Java: // 手写回溯递归
来源：http://hz.smart0.xyz/gtprorekij.html

Go:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtfgqnkpxx.html

Ruby: arr.permutation.to_a
来源：http://hz.haohaochexian.top/gttguaflbr.html

C#:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtvlxilvbf.html

[N09] 栈与队列
来源：http://hz.birdmap.top/gtklbmlmdp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sysykeji.top/gtfqjattbv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.gzhubu.top/gtwdqcduey.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yj20258.top/gtpiqnfddj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.daxiang520.top/gtflauuzme.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ydzc1.top/gtqjqpkcfd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shuidangran.top/gtoubbbbbm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.tanke756.top/gtubdzduvu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.tian-w.cn/gtapmsycmd.html

[N10] 链表节点定义
来源：http://hz.fzhhl.top/gtqzlhvpiz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yonumen.top/gtbyomimil.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cheryme.top/gtddfbvobg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xingfuxueyuan.xyz/gtgawetcmy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhiwuduotai.top/gtufzgsmtq.html

Java: class Node { int v; Node next; }
来源：http://hz.yongpay.top/gtjsmspjml.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cucudq.cn/gtnzdsuzbc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xuetiantiany.cn/gtdmqjinzo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.tianlin.xyz/gtjbpuanyq.html

[N11] 二叉树中序遍历
来源：http://hz.aizwys.cn/gtiqtxfdku.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hywenlv.cn/gtqhvranwe.html

PHP:  // 手写递归函数
来源：http://hz.yongpay.top/gthdtnfsjj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.snrcjt.cn/gtuffougit.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gogol.net.cn/gtidctllth.html

Java: // 手写递归
来源：http://hz.zycfv.cn/gthycxngxx.html

Go:   // 手写递归
来源：http://hz.sysykeji.top/gtelumssmw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ehwqpu.com/gtzlxcjety.html

C#:   // 手写递归
来源：http://hz.xuanzx.com/gtydomoeck.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yj20258888.top/gthhlwqwjv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yvedp.cn/gtowvwpfoe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinqigfzy.top/gtouffcmun.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydjk.org.cn/gtsquoulja.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hongshengwenyu.top/gtydolighf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigufen.top/gtmjghqcse.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shanyushiyangkeji.top/gtkwmkrgkm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhengqikj.top/gteccsrdhc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangkeji.top/gttnsogkcg.html


<!-- 参考信息 -->