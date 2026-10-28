代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xinyue.icu/gtkpematzi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenlongwang.top/gtucwhfaaq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zdqjudy.top/gtgjyuniwv.html

[K05] 深拷贝对象
来源：http://hz.jinqigufen.top/gtbaihtmny.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj202588.top/gtdmpuscks.html

PHP:  unserialize(serialize($obj));
来源：http://hz.dashuyun.cn/gtqrxeigup.html

JS:   structuredClone(obj)
来源：http://hz.zycfv.cn/gtdtwmyime.html

TS:   structuredClone(obj)
来源：http://hz.iojbl.cn/gtkntxzeeh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hysaishi.cn/gtzirdwjid.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shzxlz.cn/gtkfrxlyhp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yonumen.top/gtnfhoxtom.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.chenjidiqi.icu/gtyqvcqjtn.html

[K06] 解析 URL 查询串
来源：http://hz.9152youxi.cn/gtiqpzsjis.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cashguo.top/gtopvwhmvn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nanxinkj.top/gteyqieggr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pycfn.com/gtaegemfxb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuanzhike.top/gtoghumlgf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xingfuxueyuan.xyz/gtnpejkojt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.tanke756.top/gtbagexxxn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtugwikavf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.meibo888.top/gtrbbxgqyb.html

[K07] 进制转换
来源：http://hz.shuidangran.top/gtmnyrgbnp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.svipenyu.cn/gtgrlybylj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yanxiufei.cn/gtmisvuuok.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhixingplan.top/gtwalvpjok.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtgojssylt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.feifeiyinyue.top/gtwfbcbrom.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.andypj.xyz/gtdsabixxf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hnqzz.top/gtdtwrfxhf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.birdmap.top/gtzadngtbl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zdqjudy.top/gtvezvxgum.html

Py:   pickle.dumps(obj)
来源：http://hz.yuanzhike.top/gtjfgffjsc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xylfe.cn/gtvmwkjkhn.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yj202588.top/gtbbhzwlqe.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hysaishi.cn/gtyejwkuhd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zdqjudy.top/gttztmeria.html

Go:   encoding/gob
来源：http://hz.snrcjt.cn/gtpmdokjqk.html

Ruby: Marshal.dump(obj)
来源：http://hz.cheryme.top/gtxsbliagi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.tianlin.xyz/gtmnazafow.html

================================================================================
来源：http://hz.hnxiangtu.top/gtfnzbjxed.html

L. 网络请求
来源：http://hz.zhixingplan.top/gtirzjwdrt.html

================================================================================
来源：http://hz.gogol.net.cn/gtsecricii.html

[L01] 发送 GET 请求
来源：http://hz.zhoulong.xyz/gtlnhqyhme.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.havefunace.top/gtmhdcibla.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenlongwang.top/gtlbnbmosy.html

JS:   await fetch(url)
来源：http://hz.yangfankeji.com/gtjxhdafzz.html

TS:   await fetch(url)
来源：http://hz.andypj.xyz/gtepoadplv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jianghu66.top/gtyhwbkiug.html

Go:   resp, err := http.Get(url)
来源：http://hz.yangfankeji.com/gtxehqtysh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shanyushiyangtech.top/gtqqgghayk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shanyushiyangtech.top/gtafzhjpcg.html

[L02] 发送 POST JSON
来源：http://hz.xuetiantiany.cn/gthrrnmxhs.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yvedp.cn/gtbquqydxd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hongshengwenyu.top/gtqxqwlozv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xylfe.cn/gtkwfcnwxn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuanzhike.top/gttrkjkecl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jlsjyb.cn/gtcpbjoubj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.chenjidiqi.icu/gtahcrwodm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.havefunace.top/gtywfyfsxs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.chenjidiqi.icu/gtgkdglpxs.html

[L03] 设置自定义请求头
来源：http://hz.ybcxt.top/gtfuyeljxi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.feifeiyinyue.top/gtjxnbxush.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jianghu66.top/gtiurmcgdj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yvedp.cn/gtjbbyydvr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj20258.top/gtuhlumwav.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jlsjyb.cn/gtfgscomfm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shanyushiyangkeji.top/gtegfhubpl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.chenzaomai.com/gtunjfqlat.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.havefunace.top/gtaqegzskw.html

[L04] 设置超时
来源：http://hz.cqqwz.cn/gthqoarqgs.html

Py:   requests.get(url, timeout=5)
来源：http://hz.kuanghao11.cn/gtrkqeaxyb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.smart0.xyz/gtvyzgkdsw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258.top/gtjtuyzhqr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgufenzy.top/gtwzqffxxc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jqgfzy.top/gtfperiyub.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hfpthk.cn/gtowqpwmzr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tian-w.cn/gtplhklrre.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.feifeiyinyue.top/gtukzvdxjs.html

[L05] 上传文件（multipart）
来源：http://hz.hongshengwenyu.top/gtvzuighnu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gotoacloud.top/gtqvgdidsi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.9152youxi.cn/gttddadfjo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.guowangkeji.top/gtthrlfsgb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.guannengcc.top/gtsldosbrm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jinqigufen.top/gttwxwfeaa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.kuanghao11.cn/gtfzzddnpt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.nanxinkj.top/gtjxowxolr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yvedp.cn/gtdeeljugx.html

[L06] 解析响应为 JSON
来源：http://hz.haohaochexian.top/gtjyugyjqh.html

Py:   resp.json()
来源：http://hz.xylfe.cn/gtzghdgfkd.html

PHP:  json_decode($body, true);
来源：http://hz.birdmap.top/gtwjjtxbfy.html

JS:   await resp.json()
来源：http://hz.pengpengdd.cyou/gtbimgdsmu.html

TS:   await resp.json()
来源：http://hz.hfpthk.cn/gtfsmjabtv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hongshengwenyu.top/gtcushpisu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zdqjudy.top/gtijzqijmw.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hnqzz.top/gticjbmbgq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.daria6918.cn/gtpfdcpfvq.html

[L07] 处理 HTTP 状态码
来源：http://hz.shanyushiyangtech.top/gtbbooyqit.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ppjwa.cn/gtkdhhnfxk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.andypj.xyz/gtmnjjrgzp.html

JS:   resp.ok;  resp.status
来源：http://hz.yuxming.cn/gtqbrcflfh.html

TS:   resp.ok;  resp.status
来源：http://hz.shangyingyoupin.top/gtjjksbjcn.html

Java: resp.statusCode()
来源：http://hz.gzhubu.top/gtrrtkymti.html

Go:   resp.StatusCode
来源：http://hz.guannengcc.top/gthotfzjeg.html

Ruby: resp.code.to_i
来源：http://hz.yuxming.cn/gtepvqqjkn.html

C#:   (int)resp.StatusCode
来源：http://hz.jiagoushi.top/gtkiwfybks.html

[L08] 并发请求多个地址
来源：http://hz.snrcjt.cn/gtgbwowelg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zycfv.cn/gtxofzkejn.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangdashe.top/gtxltltmho.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shzxlz.cn/gtglgxifop.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guowangkeji.top/gtayrkkszu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.kuanghao11.cn/gtmqfsaxcx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.chenjidiqi.icu/gtocudhpto.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.daxiang520.top/gtluzqpbhn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xylfe.cn/gtpanufhrq.html

================================================================================
来源：http://hz.c1oappe.top/gtxqrallsj.html

M. 命令行 / 进程 / 环境
来源：http://hz.cdnleiting.top/gttgctrqqq.html

================================================================================
来源：http://hz.svipenyu.cn/gttxenagyl.html

[M01] 读取命令行参数
来源：http://hz.ehwqpu.com/gthsxhbmtz.html

Py:   sys.argv[1:]
来源：http://hz.quarkkingdee.top/gtnthddmnr.html

PHP:  $argv;  $argc;
来源：http://hz.jinghuilouyu.cn/gtppyovpum.html

JS:   process.argv.slice(2)
来源：http://hz.shanyushiyangkeji.top/gtfpdexpqi.html

TS:   process.argv.slice(2)
来源：http://hz.dianchejie.cn/gtkhmgsjav.html

Java: args 数组（main 方法参数）
来源：http://hz.ppjwa.cn/gtrnypfhyp.html

Go:   os.Args[1:]
来源：http://hz.nwbrower.top/gtbmpwvick.html

Ruby: ARGV
来源：http://hz.feifeiyinyue.top/gtfmtfnerk.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nwbrower.top/gtzokiskrk.html

[M02] 读取环境变量
来源：http://hz.pengpengdd.cyou/gtlcqcyyzr.html

Py:   os.environ.get("HOME")
来源：http://hz.haohaochexian.top/gtscsqbppt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.aibaodan.cn/gtsgkrbpde.html

JS:   process.env.HOME
来源：http://hz.wangshuangyany.cn/gtbqvgixkr.html

TS:   process.env.HOME
来源：http://hz.nanxuanxn.top/gttsphmnqn.html

Java: System.getenv("HOME")
来源：http://hz.shzxlz.cn/gtgxfsifkx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gaohongyu789.top/gtrfudevzz.html

Ruby: ENV["HOME"]
来源：http://hz.jianghu66.top/gtyvwuqjdt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenjidiqi.icu/gtwzfrikju.html

[M03] 执行外部命令
来源：http://hz.hnxiangtu.top/gtyghgtjqd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.haohaochexian.top/gttbtrunoq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.c1oappe.top/gtfucgbxts.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgfzy.top/gtnsbcjcxz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xziqi.cn/gtkflqhvvc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ydzc1.top/gtomcbgftw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.aibaodan.cn/gtczblfset.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.nanxinkj.top/gtdzbborjx.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hongshengwenyu.top/gtxflsxspp.html

[M04] 获取当前工作目录
来源：http://hz.sufxvd.cn/gtuyfdludy.html

Py:   os.getcwd()
来源：http://hz.zhijiandao.cn/gtphnspygn.html

PHP:  getcwd();
来源：http://hz.tian-w.cn/gtqcjzrddc.html

JS:   process.cwd()
来源：http://hz.jinyuanbaomall.cn/gthafkcqoi.html

TS:   process.cwd()
来源：http://hz.yueranfly.top/gtxnyobwdw.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.dashuyun.cn/gtmkageflv.html

Go:   os.Getwd()
来源：http://hz.ywan-chungtsiang.top/gtkyofcjnu.html

Ruby: Dir.pwd
来源：http://hz.yangfankeji.com/gthyhatzvy.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhongyouzk.top/gtdtmozgqq.html

[M05] 设置退出码
来源：http://hz.jinghuilouyu.cn/gtsiazsytw.html

Py:   sys.exit(1)
来源：http://hz.gaohongyu789.top/gtigrsacts.html

PHP:  exit(1);
来源：http://hz.havefunace.top/gtlpwxwdii.html

JS:   process.exit(1)
来源：http://hz.zhiwuduotai.top/gtyfhagxsv.html

TS:   process.exit(1)
来源：http://hz.zycfv.cn/gtdvbrjaev.html

Java: System.exit(1)
来源：http://hz.nwbrower.top/gtrzxngyri.html

Go:   os.Exit(1)
来源：http://hz.316326.xyz/gtqcsmzmbn.html

Ruby: exit 1
来源：http://hz.ywan-chungtsiang.top/gtsqumrpqo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yangfankeji.com/gtcotiants.html

[M06] 向标准错误输出
来源：http://hz.52xcode.cn/gtykhjswsb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ydzc1.top/gtotgsiqmo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ivvv.top/gtucwbrjly.html

JS:   console.error("err")
来源：http://hz.cdnleiting.top/gtxuobcihe.html

TS:   console.error("err")
来源：http://hz.jinghuilouyu.cn/gtfkrmfmgg.html

Java: System.err.println("err")
来源：http://hz.bjfxy.top/gthltnkvwh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.meibo888.top/gtofshntzt.html

Ruby: warn "err"
来源：http://hz.fengsongda.top/gtxhlmndew.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.pycfn.com/gtsbrdewlh.html

[M07] 判断是否为主入口
来源：http://hz.yj202588.top/gtowrjanuw.html

Py:   if __name__ == "__main__":
来源：http://hz.jqgufenzy.top/gtwwgzxtyf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.vqdsnc.cn/gtwwvnsgaq.html

JS:   require.main === module
来源：http://hz.redwolf501.top/gtmchyobtb.html

TS:   require.main === module
来源：http://hz.aizwys.cn/gtfmloxlab.html

Java: public static void main(String[] args)
来源：http://hz.quarkkingdee.top/gtncyowupg.html

Go:   func main()
来源：http://hz.daxiang520.top/gtwldjixny.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yuanzhike.top/gtmiqfduzt.html

C#:   static void Main(string[] args)
来源：http://hz.xingfuxueyuan.xyz/gtcwnxeyzx.html

[M08] 获取系统与运行时信息
来源：http://hz.jinqigufen.top/gtmkqvuwfh.html

Py:   platform.system();  platform.python_version()
来源：http://hz.birdmap.top/gtgqhjmukj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.smart0.xyz/gtxlpitbnv.html

JS:   process.platform;  process.version
来源：http://hz.tian-w.cn/gtxaromkgm.html

TS:   process.platform;  process.version
来源：http://hz.zhaomingkeji.xyz/gtkcslfnsw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.fengsongda.top/gthdfxsvan.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.iojbl.cn/gtnmrmckwy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.feifeiyinyue.top/gtcrqpiznc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.gzhubu.top/gtrqxfwtca.html

================================================================================
来源：http://hz.cucudq.cn/gtaifpelhu.html

N. 数据结构与算法
来源：http://hz.cucudq.cn/gtatuzyaqw.html

================================================================================
来源：http://hz.andypj.xyz/gtkwxwxjka.html

[N01] 二分查找（有序数组）
来源：http://hz.wangshuangyany.cn/gttytikmeh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jiagoushi.top/gtcbizpqdr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gogol.net.cn/gtuizwsumw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tanke756.top/gtbknituzr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.bjfxy.top/gtpefehptp.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhijiandao.cn/gtikbsdfrc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.dianchejie.cn/gtsddchunf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.havefunace.top/gtyfjydhkq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.kuanghao11.cn/gtwbrpbkha.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.pycfn.com/gtdymjzbex.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj20258.top/gtizkekeqn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tianlin.xyz/gtxijewmrk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.bjfxy.top/gtthbidnyr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xziqi.cn/gtjlsksqrz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cucudq.cn/gtbaowfgyu.html

Go:   slices.Sort(arr)
来源：http://hz.jinqigfzy.top/gtrpqcsefe.html

Ruby: arr.sort
来源：http://hz.shanyushiyangtech.top/gtqqzbvhxx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.c1oappe.top/gtdjmbjcoe.html

[N03] 快速排序（分治示例）
来源：http://hz.hfpthk.cn/gttldmimzu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ivvv.top/gtvajiitfp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.feifeiyinyue.top/gtgaahfvdr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.redwolf501.top/gtoxltblvr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aizwys.cn/gtrkihtghl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jianghu66.top/gtcyhaffsk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.mhx1999.top/gtrogeytxd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cucudq.cn/gtdonvxjcz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.feifeiyinyue.top/gtcrijlosn.html

[N04] 斐波那契数列
来源：http://hz.snrcjt.cn/gtjpratsqv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jqgfzy.top/gtxbgsktcx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.gotoacloud.top/gtnegtgypi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.guowangkeji.top/gtdbodlwbq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gthshmsyeb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hywenlv.cn/gtyzxyxcfx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yj202588.top/gtgxmlwsan.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.aizwys.cn/gtckbacdxk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.aibaodan.cn/gtrtbvhsxe.html

[N05] 最大公约数
来源：http://hz.xziqi.cn/gtoeovvqqh.html

Py:   math.gcd(a, b)
来源：http://hz.yj20258888.top/gtjmtlsxsq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.mhx1999.top/gtyvoggsnn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhoulong.xyz/gtehfbeuko.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sysykeji.top/gtyxahgnwh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cucudq.cn/gtzbjivrdc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cashguo.top/gtkzlngyof.html

Ruby: a.gcd(b)
来源：http://hz.wangshuangyany.cn/gtjmbuhyhz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.wangdashe.top/gthgndwrvy.html

[N06] 判断回文字符串
来源：http://hz.shuidangran.top/gtwnbzjxgb.html

Py:   s == s[::-1]
来源：http://hz.sweek.top/gtrcxydvve.html

PHP:  $s === strrev($s);
来源：http://hz.yanxiufei.cn/gtqzxnizts.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jqgufenzy.top/gtneshumma.html

TS:   s === [...s].reverse().join("")
来源：http://hz.daxiang520.top/gtwbbxivkb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zdqjudy.top/gtthrsrwtt.html

Go:   // 双指针从两端比较
来源：http://hz.zhiwuduotai.top/gtqeodqfdl.html

Ruby: s == s.reverse
来源：http://hz.chenlongwang.top/gtqpsldffk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangtech.top/gtnrsamnkc.html

[N07] 两数之和（返回下标）
来源：http://hz.yongpay.top/gtlwzvdyuw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hnxiangtu.top/gtkozzxkjw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yj20258888.top/gtzjtnxrmz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nanxuanxn.top/gtzwnqghen.html

TS:   // 手写 Map<string, number>
来源：http://hz.shanyushiyangtech.top/gtkuoraknl.html

Java: // 手写 HashMap
来源：http://hz.xziqi.cn/gtoperazrc.html

Go:   // 手写 map[int]int
来源：http://hz.jlsjyb.cn/gtqzipbkcx.html

Ruby: // 手写 Hash
来源：http://hz.c1oappe.top/gtfdgzukyx.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.nanxuanxn.top/gtbvymcyzz.html

[N08] 生成全排列
来源：http://hz.guannengcc.top/gtkdwzqbxl.html

Py:   itertools.permutations(arr)
来源：http://hz.zhixingplan.top/gtywrukvhc.html

PHP:  // 手写递归交换
来源：http://hz.c1oappe.top/gtslpxywgs.html

JS:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtwircfffr.html

TS:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtroqwryvm.html

Java: // 手写回溯递归
来源：http://hz.guannengcc.top/gtfezwzoaw.html

Go:   // 手写回溯递归
来源：http://hz.cheryme.top/gtxlrcgcxl.html

Ruby: arr.permutation.to_a
来源：http://hz.kuanghao11.cn/gtwiwkjuep.html

C#:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtiuxsikgz.html

[N09] 栈与队列
来源：http://hz.quarkkingdee.top/gtibjgpdgx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.haohaochexian.top/gthbckuegy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.haohaochexian.top/gtramscqfr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.aizwys.cn/gtekruupra.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jqgfzy.top/gtljhdvhqh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sweek.top/gttuccysjl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yongpay.top/gtauxydiel.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.gzhubu.top/gtbutvujkm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.tian-w.cn/gtdkmymcte.html

[N10] 链表节点定义
来源：http://hz.ywan-chungtsiang.top/gtrbxmsldx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gzhubu.top/gtohytddez.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hnqzz.top/gtapgzvmtr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gotoacloud.top/gtkymjiigy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhengqikj.top/gtuvckohtc.html

Java: class Node { int v; Node next; }
来源：http://hz.zhijiandao.cn/gtiwycxxzp.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinqigfzy.top/gtaokrvoqh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yj20258.top/gtwtklnugz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jinyuanbaomall.cn/gtlrdrqacz.html

[N11] 二叉树中序遍历
来源：http://hz.chenzaomai.com/gtowhyguxw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zycfv.cn/gtzokxpsgy.html

PHP:  // 手写递归函数
来源：http://hz.sxryk.cn/gtrnngmyjx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.feifeiyinyue.top/gtivqjxfmj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nwbrower.top/gtzupabgfc.html

Java: // 手写递归
来源：http://hz.andypj.xyz/gtjpnhnnal.html

Go:   // 手写递归
来源：http://hz.gogol.net.cn/gtrllncrtf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.c1oappe.top/gtxixxlovp.html

C#:   // 手写递归
来源：http://hz.hysaishi.cn/gtzsvvvwss.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jlsjyb.cn/gtsplnakeb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xuetiantiany.cn/gthaitqvxz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yuanzhike.top/gtebulggmn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.haohaochexian.top/gtjgfmesvh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hywenlv.cn/gtmmpjjhxl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenlongwang.top/gtytyaiwki.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hysaishi.cn/gtutfmycby.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinyuanbaomall.cn/gtaweogwqj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pengpengdd.cyou/gtqlaydiip.html


<!-- 参考信息 -->