代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cucudq.cn/gtqiqyblhc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shuidangran.top/gtttuhpfby.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.guannengcc.top/gtgikigwyq.html

[K05] 深拷贝对象
来源：http://hz.jyoumei.cn/gtsekergjk.html

Py:   copy.deepcopy(obj)
来源：http://hz.yongpay.top/gtdunxiaol.html

PHP:  unserialize(serialize($obj));
来源：http://hz.nanxinkj.top/gtqkzerjus.html

JS:   structuredClone(obj)
来源：http://hz.hammf.cn/gtifnatbwe.html

TS:   structuredClone(obj)
来源：http://hz.shangyingyoupin.top/gtuwdrygur.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.havefunace.top/gtbvtfbneo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.nanxuanxn.top/gtqwblngnm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shanyushiyangkeji.top/gtvyqsxkbj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.pycfn.com/gtbmoimbsj.html

[K06] 解析 URL 查询串
来源：http://hz.aizwys.cn/gtdltyeijs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hywenlv.cn/gtlwlzqtlb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hfpthk.cn/gtiynsdhjb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gaohongyu789.top/gtccnehpea.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sweek.top/gtbaptkjrj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ydzc1.top/gtrvrrqzqs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jlsjyb.cn/gtqgvoeekc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.nanxuanxn.top/gttbfvmcmi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.dashuyun.cn/gttoonpscx.html

[K07] 进制转换
来源：http://hz.svipenyu.cn/gtdnuhyatq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cashguo.top/gtebahwqgf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ydzc1.top/gtjyohhyio.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tian-w.cn/gthkktuyrw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.havefunace.top/gtwimgorfh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gtrmvgizhm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hnxiangtu.top/gtofugqmxu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shanyushiyangkeji.top/gteyxogcoo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.fengsongda.top/gtlbmjtgsd.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.fzhhl.top/gtwlpdprxf.html

Py:   pickle.dumps(obj)
来源：http://hz.9152youxi.cn/gtcskgzopz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhoulong.xyz/gtdjumejzo.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.birdmap.top/gtajtsqabd.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.guannengcc.top/gtpsweqjwj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yongpay.top/gtcofcjipg.html

Go:   encoding/gob
来源：http://hz.wangdashe.top/gtzfxstmky.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhiwuduotai.top/gtswsydcyz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj20258.top/gtuzrajmzh.html

================================================================================
来源：http://hz.9152youxi.cn/gtuagpeccu.html

L. 网络请求
来源：http://hz.yongpay.top/gtvenccgll.html

================================================================================
来源：http://hz.yvedp.cn/gtuxiclglw.html

[L01] 发送 GET 请求
来源：http://hz.yj20258.top/gtvzycdatn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jiagoushi.top/gturubgphn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.guowangkeji.top/gtkiplkzpq.html

JS:   await fetch(url)
来源：http://hz.aizwys.cn/gtgshtlojy.html

TS:   await fetch(url)
来源：http://hz.wangshuangyany.cn/gteliduzqz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sxryk.cn/gtgsswsgdd.html

Go:   resp, err := http.Get(url)
来源：http://hz.fzhhl.top/gtkvyurefy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hfpthk.cn/gtdgdidbvh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zycfv.cn/gtoysycbpo.html

[L02] 发送 POST JSON
来源：http://hz.ppjwa.cn/gthasgwqwj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.quarkkingdee.top/gtvebrfxhd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gotoacloud.top/gtrshsurto.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hongshengwenyu.top/gtdcmvyhxh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangshuangyany.cn/gtyujsnytl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj202588.top/gtiewzhidi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jianghu66.top/gtbafqeudw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shanyushiyangtech.top/gtvfpkqdig.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cdnleiting.top/gtzibuhlhu.html

[L03] 设置自定义请求头
来源：http://hz.sufxvd.cn/gtntzimoes.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinghuilouyu.cn/gtvuuotnyf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cheryme.top/gtoreshduy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhaomingkeji.xyz/gtqmsbrzxv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenlongwang.top/gthibvwmad.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yj20258.top/gtdmdwvkyo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sxryk.cn/gtppckyjja.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhaomingkeji.xyz/gttuyukvgi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.chenjidiqi.icu/gttuzgpgcb.html

[L04] 设置超时
来源：http://hz.smart0.xyz/gtdbztayng.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ydjk.org.cn/gtucivyfkq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.9152youxi.cn/gtoelwqssy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shanyushiyangtech.top/gtbctrtqhe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.redwolf501.top/gtiuqqcnva.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sxryk.cn/gtuhdquxvc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.bjfxy.top/gtptrqerce.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.kuanghao11.cn/gtozfbwcat.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.snrcjt.cn/gtorcqrzdl.html

[L05] 上传文件（multipart）
来源：http://hz.cucudq.cn/gtcakkwsti.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.tian-w.cn/gtubfbsojg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhoulong.xyz/gtzgowmlgv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuanzhike.top/gtccelbtck.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydzc1.top/gtqqmvenlq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xingfuxueyuan.xyz/gtbewlzwco.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xylfe.cn/gtdkpkccqs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shuidangran.top/gttabfbwkp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cdnleiting.top/gtlezeyxlh.html

[L06] 解析响应为 JSON
来源：http://hz.andypj.xyz/gtzudonukt.html

Py:   resp.json()
来源：http://hz.fengsongda.top/gtyebxcfwp.html

PHP:  json_decode($body, true);
来源：http://hz.shzxlz.cn/gtccnoeuis.html

JS:   await resp.json()
来源：http://hz.chenzaomai.com/gtbupbdhww.html

TS:   await resp.json()
来源：http://hz.gogol.net.cn/gtbfyyxbse.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xuetiantiany.cn/gtjapohcid.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jianghu66.top/gtdqbieflh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yj202588.top/gtjbjrcrnp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.aizwys.cn/gteapikcqa.html

[L07] 处理 HTTP 状态码
来源：http://hz.nanxinkj.top/gtapajjpoh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhengqikj.top/gtfzljlihk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinghuilouyu.cn/gtcbcncvne.html

JS:   resp.ok;  resp.status
来源：http://hz.chenjidiqi.icu/gtwdzbinbt.html

TS:   resp.ok;  resp.status
来源：http://hz.ydjk.org.cn/gtzicenvfa.html

Java: resp.statusCode()
来源：http://hz.bjfxy.top/gtldmrwxbn.html

Go:   resp.StatusCode
来源：http://hz.zhengqikj.top/gtffpccznp.html

Ruby: resp.code.to_i
来源：http://hz.havefunace.top/gtdeyhdxou.html

C#:   (int)resp.StatusCode
来源：http://hz.wangshuangyany.cn/gthdkizpea.html

[L08] 并发请求多个地址
来源：http://hz.yj20258888.top/gtxldrjybb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.andypj.xyz/gtsmbsrpbc.html

PHP:  curl_multi_init() 系列
来源：http://hz.daria6918.cn/gtugniemfw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258.top/gtrqzswwlu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj202588.top/gtshuvpgps.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhijiandao.cn/gtbmrhqcll.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xingfuxueyuan.xyz/gthambleuc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yanxiufei.cn/gtqpnkunjf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xylfe.cn/gtfksczxqe.html

================================================================================
来源：http://hz.hammf.cn/gthvxcifnd.html

M. 命令行 / 进程 / 环境
来源：http://hz.yj202588.top/gtoejddynd.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtzaggeunw.html

[M01] 读取命令行参数
来源：http://hz.zycfv.cn/gtndjliqju.html

Py:   sys.argv[1:]
来源：http://hz.yj20258.top/gtepjaanog.html

PHP:  $argv;  $argc;
来源：http://hz.xingfuxueyuan.xyz/gttbstvnuc.html

JS:   process.argv.slice(2)
来源：http://hz.nanxuanxn.top/gtcuaowhzb.html

TS:   process.argv.slice(2)
来源：http://hz.jyoumei.cn/gtoojutuqy.html

Java: args 数组（main 方法参数）
来源：http://hz.kuanghao11.cn/gtbisyjats.html

Go:   os.Args[1:]
来源：http://hz.sysykeji.top/gtphxuokqo.html

Ruby: ARGV
来源：http://hz.cheryme.top/gtywjdvhza.html

C#:   args 数组（Main 方法参数）
来源：http://hz.smart0.xyz/gtlwmvckps.html

[M02] 读取环境变量
来源：http://hz.zhijiandao.cn/gtnksyfhah.html

Py:   os.environ.get("HOME")
来源：http://hz.ydzc1.top/gtegiljrou.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.52xcode.cn/gtyzndeiww.html

JS:   process.env.HOME
来源：http://hz.ivvv.top/gtaongqxyf.html

TS:   process.env.HOME
来源：http://hz.zhaomingkeji.xyz/gtenhuqwng.html

Java: System.getenv("HOME")
来源：http://hz.sysykeji.top/gtbuhhtjkk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sweek.top/gtnhjlyxxk.html

Ruby: ENV["HOME"]
来源：http://hz.dashuyun.cn/gtvmoituzy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xinyue.icu/gtxoaofxxy.html

[M03] 执行外部命令
来源：http://hz.zhiwuduotai.top/gtxidkhntf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.tianlin.xyz/gtehfttzfl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xinyue.icu/gtsnywnqtm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.daxiang520.top/gtgqjzfxtv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.dianchejie.cn/gtzfhvqoiz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zycfv.cn/gthecmotfb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.birdmap.top/gtwjeadhqa.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.andypj.xyz/gtqitjxxbc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xuetiantiany.cn/gtnvnnztgx.html

[M04] 获取当前工作目录
来源：http://hz.ydjk.org.cn/gtwxsuomxt.html

Py:   os.getcwd()
来源：http://hz.yuxming.cn/gtpgyyruzj.html

PHP:  getcwd();
来源：http://hz.andypj.xyz/gtlyzodwel.html

JS:   process.cwd()
来源：http://hz.zycfv.cn/gttkwpmuwo.html

TS:   process.cwd()
来源：http://hz.hnqzz.top/gtwagiosof.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hywenlv.cn/gtgmyxzpdh.html

Go:   os.Getwd()
来源：http://hz.havefunace.top/gtgxytbfdk.html

Ruby: Dir.pwd
来源：http://hz.hnxiangtu.top/gtpiihxeda.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hfpthk.cn/gtrbijxcze.html

[M05] 设置退出码
来源：http://hz.vqdsnc.cn/gtceetqdqc.html

Py:   sys.exit(1)
来源：http://hz.jqgufenzy.top/gtrzgzfhbz.html

PHP:  exit(1);
来源：http://hz.chenzaomai.com/gtvlsaxorp.html

JS:   process.exit(1)
来源：http://hz.guowangkeji.top/gtvwczawux.html

TS:   process.exit(1)
来源：http://hz.redwolf501.top/gtalnbzdlq.html

Java: System.exit(1)
来源：http://hz.wangdashe.top/gtukcmasxa.html

Go:   os.Exit(1)
来源：http://hz.vqdsnc.cn/gtvxxwyygx.html

Ruby: exit 1
来源：http://hz.fengsongda.top/gtjbuqhdkg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ydzc1.top/gtakgieusi.html

[M06] 向标准错误输出
来源：http://hz.zhiwuduotai.top/gthkgscxdq.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jiagoushi.top/gtxpwrohei.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.meibo888.top/gtnuhzucuc.html

JS:   console.error("err")
来源：http://hz.yanxiufei.cn/gtmqxzipnl.html

TS:   console.error("err")
来源：http://hz.snrcjt.cn/gtllakoeyl.html

Java: System.err.println("err")
来源：http://hz.zhijiandao.cn/gtxuuzbghh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ydjk.org.cn/gtlaetgsip.html

Ruby: warn "err"
来源：http://hz.yj202588.top/gtmxikzabl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yangfankeji.com/gtqplqtrjl.html

[M07] 判断是否为主入口
来源：http://hz.sxryk.cn/gttzyqfprl.html

Py:   if __name__ == "__main__":
来源：http://hz.bjfxy.top/gtrdggklqa.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.nanxuanxn.top/gtfvhhfohh.html

JS:   require.main === module
来源：http://hz.kuanghao11.cn/gtkkzyiyty.html

TS:   require.main === module
来源：http://hz.iojbl.cn/gtbhqkpvyo.html

Java: public static void main(String[] args)
来源：http://hz.nanxuanxn.top/gtlnezkujh.html

Go:   func main()
来源：http://hz.jinghuilouyu.cn/gtaetzretu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cashguo.top/gtyooufztp.html

C#:   static void Main(string[] args)
来源：http://hz.aibaodan.cn/gtkmgskpqx.html

[M08] 获取系统与运行时信息
来源：http://hz.andypj.xyz/gtdegdvtkx.html

Py:   platform.system();  platform.python_version()
来源：http://hz.guowangkeji.top/gtxmoujfnn.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hfpthk.cn/gtobntokit.html

JS:   process.platform;  process.version
来源：http://hz.zhongyouzk.top/gtfogkstpl.html

TS:   process.platform;  process.version
来源：http://hz.daria6918.cn/gtowvnczdj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.meibo888.top/gtwedvntal.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shanyushiyangtech.top/gtfdmsccvb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.52xcode.cn/gtcxrshrpr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ivvv.top/gtuhixkkmt.html

================================================================================
来源：http://hz.jianghu66.top/gtwczbxauk.html

N. 数据结构与算法
来源：http://hz.jinghuilouyu.cn/gtzbxejvhp.html

================================================================================
来源：http://hz.zdqjudy.top/gtxwnvvrqv.html

[N01] 二分查找（有序数组）
来源：http://hz.316326.xyz/gtdagkqdku.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj20258888.top/gtdvcqemok.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.0kj1m.cn/gtyatgaoza.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydjk.org.cn/gtypcwzrgd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ywan-chungtsiang.top/gtsqzpwxzq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cdnleiting.top/gtwplmepww.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtpwhhbpji.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.dashuyun.cn/gtcdnzqjwj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nwbrower.top/gtdupjankt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.aibaodan.cn/gtbcxiahci.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cheryme.top/gtpyisermx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhoulong.xyz/gtyicoevyx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.c1oappe.top/gtwapunmpe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258888.top/gtyeiqbjin.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zycfv.cn/gtdcifisgl.html

Go:   slices.Sort(arr)
来源：http://hz.jiagoushi.top/gtpzuvisqt.html

Ruby: arr.sort
来源：http://hz.chenlongwang.top/gtodhjilfa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinqigfzy.top/gtqodknsfz.html

[N03] 快速排序（分治示例）
来源：http://hz.pycfn.com/gtyksfwrju.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gotoacloud.top/gtuufikcui.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nwbrower.top/gtklybmdgh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ivvv.top/gtyxdibzoq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydjk.org.cn/gtjftkyyes.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.fzhhl.top/gtpddvbbtk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jqgufenzy.top/gtndiztefb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.daria6918.cn/gtpdxguxdn.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cqqwz.cn/gthxqsgfig.html

[N04] 斐波那契数列
来源：http://hz.feifeiyinyue.top/gtjpjqkldc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.gaohongyu789.top/gtixsmrkbz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.9152youxi.cn/gtrrljgder.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ywan-chungtsiang.top/gtrzyvdmzy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenzaomai.com/gtteisypas.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.redwolf501.top/gttoenmjbf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gogol.net.cn/gtywpbnpwn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.chenzaomai.com/gtiwdnjglf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ehwqpu.com/gtcijzgcud.html

[N05] 最大公约数
来源：http://hz.yuanzhike.top/gtwcufaenq.html

Py:   math.gcd(a, b)
来源：http://hz.aibaodan.cn/gtsktcyyqd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shuidangran.top/gtvjslkilm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dianchejie.cn/gtbrmqaria.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gzhubu.top/gtsbbezixp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yuanzhike.top/gtftxhjbyt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.dashuyun.cn/gtrvtoailu.html

Ruby: a.gcd(b)
来源：http://hz.dashuyun.cn/gtkzyxfzgx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hywenlv.cn/gtrwrpoizv.html

[N06] 判断回文字符串
来源：http://hz.quarkkingdee.top/gtzmcmdvet.html

Py:   s == s[::-1]
来源：http://hz.yj20258.top/gtdnbmkntm.html

PHP:  $s === strrev($s);
来源：http://hz.zycfv.cn/gtfhvbprka.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ivvv.top/gtyrmtbwkl.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jinghuilouyu.cn/gtuagqqavm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shanyushiyangtech.top/gtpllfhmhn.html

Go:   // 双指针从两端比较
来源：http://hz.havefunace.top/gtfizhmskr.html

Ruby: s == s.reverse
来源：http://hz.jqgfzy.top/gtlibwfume.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zycfv.cn/gtyjjnmdxu.html

[N07] 两数之和（返回下标）
来源：http://hz.ivvv.top/gteseivgww.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.aibaodan.cn/gtekighgnj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.quarkkingdee.top/gtpedqltwk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.meibo888.top/gtglbncvkd.html

TS:   // 手写 Map<string, number>
来源：http://hz.cqqwz.cn/gtagyayqkw.html

Java: // 手写 HashMap
来源：http://hz.yangfankeji.com/gtwszleeqj.html

Go:   // 手写 map[int]int
来源：http://hz.hfpthk.cn/gttfizxaqv.html

Ruby: // 手写 Hash
来源：http://hz.zhaomingkeji.xyz/gtfnetrglv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yuanzhike.top/gtqmfvmhjx.html

[N08] 生成全排列
来源：http://hz.c1oappe.top/gttoirjdas.html

Py:   itertools.permutations(arr)
来源：http://hz.aizwys.cn/gttrowfoev.html

PHP:  // 手写递归交换
来源：http://hz.cdnleiting.top/gtexakavcr.html

JS:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtcllvlrln.html

TS:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gttasrjgow.html

Java: // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtexuforio.html

Go:   // 手写回溯递归
来源：http://hz.dianchejie.cn/gtolmpleod.html

Ruby: arr.permutation.to_a
来源：http://hz.xingfuxueyuan.xyz/gttfycshut.html

C#:   // 手写回溯递归
来源：http://hz.yj20258.top/gtksllvvod.html

[N09] 栈与队列
来源：http://hz.jlsjyb.cn/gtdlohxzgj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yvedp.cn/gtpddmdioa.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.dashuyun.cn/gtokmkvjet.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.fengsongda.top/gtlxfldtbx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yuanzhike.top/gtbgyunklx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gzhubu.top/gtoemxxgbh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.haohaochexian.top/gtgpklxjof.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yangfankeji.com/gtqipmgpho.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gzhubu.top/gtzplyfkwl.html

[N10] 链表节点定义
来源：http://hz.316326.xyz/gtvefyhzib.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhoulong.xyz/gtgmdicrdr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.chenlongwang.top/gtyfqahqjv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sysykeji.top/gtehgmsrxm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gaohongyu789.top/gttxnmhlwa.html

Java: class Node { int v; Node next; }
来源：http://hz.hongshengwenyu.top/gtutlaxepa.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jqgufenzy.top/gteipxytxm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yongpay.top/gtztwlthdv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yonumen.top/gtmwbwqvpx.html

[N11] 二叉树中序遍历
来源：http://hz.gogol.net.cn/gtjmdpyszb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hongshengwenyu.top/gtrkzqzdnf.html

PHP:  // 手写递归函数
来源：http://hz.wangshuangyany.cn/gtsslzegbr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jiagoushi.top/gtiziwoqkm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shanyushiyangkeji.top/gtuttnwgmk.html

Java: // 手写递归
来源：http://hz.hywenlv.cn/gtogimflju.html

Go:   // 手写递归
来源：http://hz.fengsongda.top/gtvzskzedg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.wangdashe.top/gtljkjxjie.html

C#:   // 手写递归
来源：http://hz.yonumen.top/gthhmlzljo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yangfankeji.com/gthfquwzcz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhijiandao.cn/gtgqvklmxm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xuetiantiany.cn/gtpgzgwint.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.c1oappe.top/gtimcrmmhr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gzhubu.top/gtvmsfouxs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gzhubu.top/gtxhxggssu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xziqi.cn/gtziunnhig.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yanxiufei.cn/gtmtzzdexa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yueranfly.top/gtmornbenq.html


<!-- 参考信息 -->