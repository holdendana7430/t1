代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258.top/gtcrgrhcet.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hysaishi.cn/gtksiygvyw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.316326.xyz/gthxavnvpy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gzhubu.top/gtfylkssfl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tian-w.cn/gtfcfnrnen.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.bjfxy.top/gtytwxkfzz.html

[K04] 读取 JSON 文件
来源：http://hz.ywan-chungtsiang.top/gtpkgssmjn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.guannengcc.top/gtwtlqvxrw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhengqikj.top/gtwtihzgzd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.feifeiyinyue.top/gtwbujnkuo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daxiang520.top/gtgrobiesd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cucudq.cn/gtwpibcstc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gtybsczqau.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.haohaochexian.top/gtcndfkhrt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sufxvd.cn/gthmnlumaw.html

[K05] 深拷贝对象
来源：http://hz.iojbl.cn/gtnuvgamxn.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhoulong.xyz/gtuywhgluq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hfpthk.cn/gtfbipxgyt.html

JS:   structuredClone(obj)
来源：http://hz.daxiang520.top/gtexltaojy.html

TS:   structuredClone(obj)
来源：http://hz.chenlongwang.top/gteihnvywv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jyoumei.cn/gtbavnjipe.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gotoacloud.top/gtkfmhlytq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.daxiang520.top/gtnuujhkpq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gogol.net.cn/gtnjhavmjm.html

[K06] 解析 URL 查询串
来源：http://hz.fengsongda.top/gtimjmikec.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.chenlongwang.top/gtfzluujfu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.quarkkingdee.top/gtsmabtqkl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.feifeiyinyue.top/gtenptgkti.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tian-w.cn/gtieffddqz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.smart0.xyz/gtldemnsiy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.dianchejie.cn/gtuycgutvq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ppjwa.cn/gttqrqntyb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ehwqpu.com/gtxilsoyhe.html

[K07] 进制转换
来源：http://hz.quarkkingdee.top/gtcanhmcql.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.mhx1999.top/gtgfcqxmnu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.vqdsnc.cn/gtrieuncuq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtfihziibr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yueranfly.top/gtqrzppndt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zycfv.cn/gthmjcngca.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.chenlongwang.top/gtwzpzvhoh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nwbrower.top/gtnopotxqm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.aizwys.cn/gtqynjvxxu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.wangdashe.top/gtuazrwkko.html

Py:   pickle.dumps(obj)
来源：http://hz.hywenlv.cn/gtupckjysx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ppjwa.cn/gtrnvljjlh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yanxiufei.cn/gtawlbzyyd.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yangfankeji.com/gtgatmprsl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.wangshuangyany.cn/gtgfzdsayf.html

Go:   encoding/gob
来源：http://hz.shanyushiyangtech.top/gtsekqiohx.html

Ruby: Marshal.dump(obj)
来源：http://hz.havefunace.top/gtatlynhyz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhijiandao.cn/gtaxuktjoy.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtqeuqmawi.html

L. 网络请求
来源：http://hz.vqdsnc.cn/gtawcvnzjf.html

================================================================================
来源：http://hz.ivvv.top/gtjdfzwiuy.html

[L01] 发送 GET 请求
来源：http://hz.jianghu66.top/gtwojkpmlp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhaomingkeji.xyz/gtgxujsnby.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ydjk.org.cn/gtjblosrhu.html

JS:   await fetch(url)
来源：http://hz.snrcjt.cn/gtkoqopqjr.html

TS:   await fetch(url)
来源：http://hz.ivvv.top/gthacehkke.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hysaishi.cn/gtzdjinjsg.html

Go:   resp, err := http.Get(url)
来源：http://hz.xinyue.icu/gtzqctigsg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.daria6918.cn/gtyzfptvuw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.daria6918.cn/gtvoxjretr.html

[L02] 发送 POST JSON
来源：http://hz.yvedp.cn/gtodhcnlod.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.snrcjt.cn/gttljllldp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhengqikj.top/gtfbpfmtsz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.daria6918.cn/gttxuexmtj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxuanxn.top/gtyakqyemq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gogol.net.cn/gtgmjywemy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jqgufenzy.top/gtubftuicg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xuanzx.com/gtaghtfjim.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xziqi.cn/gtfmauugng.html

[L03] 设置自定义请求头
来源：http://hz.ivvv.top/gtvtiucnil.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xylfe.cn/gtcsgyxdla.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xziqi.cn/gtiwqqqjlm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hammf.cn/gtjxcjkbaq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.snrcjt.cn/gtobwzxzsq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ppjwa.cn/gtbgljtpyw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinqigufen.top/gttxtzdsbx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhaomingkeji.xyz/gtvpxtqjfi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinyuanbaomall.cn/gtitlwsovg.html

[L04] 设置超时
来源：http://hz.zhijiandao.cn/gtamhjclxu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xuetiantiany.cn/gtkuykwjvu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.bjfxy.top/gtozcreoup.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuanzhike.top/gtrjgjtnie.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tanke756.top/gtevukjaer.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.meibo888.top/gtfftvqepy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.wangshuangyany.cn/gtyhsqpniu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ybcxt.top/gthpazdugd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xuetiantiany.cn/gtjclufdrb.html

[L05] 上传文件（multipart）
来源：http://hz.wangshuangyany.cn/gtssebalgu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.kuanghao11.cn/gtjbbgynrd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yuxming.cn/gtmegrrjnj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yueranfly.top/gtbtsegckm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgfzy.top/gtsskqazce.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.nwbrower.top/gtdpsnnmtv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ydzc1.top/gtrpyxtvmb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.aizwys.cn/gtzutqczsw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hywenlv.cn/gtasjusnls.html

[L06] 解析响应为 JSON
来源：http://hz.chenjidiqi.icu/gtxdcxrgiw.html

Py:   resp.json()
来源：http://hz.tian-w.cn/gtvbjmmzhs.html

PHP:  json_decode($body, true);
来源：http://hz.havefunace.top/gtgcmsmmgr.html

JS:   await resp.json()
来源：http://hz.gaohongyu789.top/gtowkpnuet.html

TS:   await resp.json()
来源：http://hz.aibaodan.cn/gtvuaatuqh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ybcxt.top/gtrypxgtlm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinghuilouyu.cn/gtwwexxlel.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yongpay.top/gtzfjaslbg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tian-w.cn/gtpxjbqwpn.html

[L07] 处理 HTTP 状态码
来源：http://hz.mhx1999.top/gtnmbvaywt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jqgufenzy.top/gtuicpzvjl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yangfankeji.com/gtksdhavot.html

JS:   resp.ok;  resp.status
来源：http://hz.svipenyu.cn/gtkhjlresf.html

TS:   resp.ok;  resp.status
来源：http://hz.gzhubu.top/gtcbesypiy.html

Java: resp.statusCode()
来源：http://hz.zhiwuduotai.top/gtujrywamm.html

Go:   resp.StatusCode
来源：http://hz.aibaodan.cn/gtamoaijmx.html

Ruby: resp.code.to_i
来源：http://hz.dianchejie.cn/gtxxupnaiu.html

C#:   (int)resp.StatusCode
来源：http://hz.vqdsnc.cn/gthqzuzgwo.html

[L08] 并发请求多个地址
来源：http://hz.zhoulong.xyz/gtzxfiqcpx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.iojbl.cn/gtlkjiewfu.html

PHP:  curl_multi_init() 系列
来源：http://hz.sxryk.cn/gtnvcgyflx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtykwxzlds.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxinkj.top/gtugymqaso.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yueranfly.top/gtgtxbqlhd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xziqi.cn/gtnytxsjvh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jyoumei.cn/gttcmgegim.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yueranfly.top/gtgzgtuutj.html

================================================================================
来源：http://hz.jlsjyb.cn/gtikhjkrxg.html

M. 命令行 / 进程 / 环境
来源：http://hz.shanyushiyangtech.top/gtovjeqgri.html

================================================================================
来源：http://hz.gotoacloud.top/gthzbkhciv.html

[M01] 读取命令行参数
来源：http://hz.cheryme.top/gtdyimiztz.html

Py:   sys.argv[1:]
来源：http://hz.ybcxt.top/gtcfddfzes.html

PHP:  $argv;  $argc;
来源：http://hz.jinqigufen.top/gtavhqslnk.html

JS:   process.argv.slice(2)
来源：http://hz.jlsjyb.cn/gtrynhttdq.html

TS:   process.argv.slice(2)
来源：http://hz.gzhubu.top/gtngcczmhg.html

Java: args 数组（main 方法参数）
来源：http://hz.cqqwz.cn/gtouupgqfp.html

Go:   os.Args[1:]
来源：http://hz.haohaochexian.top/gtvqtuhymf.html

Ruby: ARGV
来源：http://hz.zycfv.cn/gtxhkkkqbq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenzaomai.com/gtugexianf.html

[M02] 读取环境变量
来源：http://hz.ivvv.top/gtuczbvoeu.html

Py:   os.environ.get("HOME")
来源：http://hz.hammf.cn/gtiqglvrkk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.tian-w.cn/gtykguzkzc.html

JS:   process.env.HOME
来源：http://hz.jinqigufen.top/gtxoaouata.html

TS:   process.env.HOME
来源：http://hz.xinyue.icu/gtfccjgsee.html

Java: System.getenv("HOME")
来源：http://hz.shangyingyoupin.top/gtljoocbss.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hnqzz.top/gtmcwuvsju.html

Ruby: ENV["HOME"]
来源：http://hz.0kj1m.cn/gtceyxkyxe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gzhubu.top/gtwkyounds.html

[M03] 执行外部命令
来源：http://hz.mhx1999.top/gtuyyjjfbn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.redwolf501.top/gtdzdztcbl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jyoumei.cn/gtphrlchps.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhoulong.xyz/gtloquzrbx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigfzy.top/gtjnxwockb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.havefunace.top/gtsjmclswo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.pengpengdd.cyou/gtbarcswqc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jyoumei.cn/gtjrzwsrmo.html

C#:   Process.Start("ls", "-l");
来源：http://hz.guowangkeji.top/gteouvmtvy.html

[M04] 获取当前工作目录
来源：http://hz.ydjk.org.cn/gtygwnymfe.html

Py:   os.getcwd()
来源：http://hz.zhiwuduotai.top/gtwsgrvrkc.html

PHP:  getcwd();
来源：http://hz.bjfxy.top/gtpnuxkbtw.html

JS:   process.cwd()
来源：http://hz.yuanzhike.top/gtyybozhik.html

TS:   process.cwd()
来源：http://hz.svipenyu.cn/gtrylajrej.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.9152youxi.cn/gtbuabxejy.html

Go:   os.Getwd()
来源：http://hz.tanke756.top/gtaupgwgol.html

Ruby: Dir.pwd
来源：http://hz.sweek.top/gtavxrkcez.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.guannengcc.top/gtedgpbjki.html

[M05] 设置退出码
来源：http://hz.jinqigfzy.top/gtyumdeupp.html

Py:   sys.exit(1)
来源：http://hz.kuanghao11.cn/gtonmrofoa.html

PHP:  exit(1);
来源：http://hz.daxiang520.top/gtfvcjwpia.html

JS:   process.exit(1)
来源：http://hz.feifeiyinyue.top/gtuqbfcxer.html

TS:   process.exit(1)
来源：http://hz.sufxvd.cn/gtdsggfnec.html

Java: System.exit(1)
来源：http://hz.xuanzx.com/gtdcihqifa.html

Go:   os.Exit(1)
来源：http://hz.birdmap.top/gtzdvorbkn.html

Ruby: exit 1
来源：http://hz.xylfe.cn/gtnyrzzsps.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhixingplan.top/gtzhfgeiwv.html

[M06] 向标准错误输出
来源：http://hz.zhijiandao.cn/gtrucrahog.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yueranfly.top/gtlpnsmmmg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhijiandao.cn/gttjuvpdmk.html

JS:   console.error("err")
来源：http://hz.nanxuanxn.top/gtktjhrwjg.html

TS:   console.error("err")
来源：http://hz.52xcode.cn/gtuqiufkdw.html

Java: System.err.println("err")
来源：http://hz.svipenyu.cn/gtohzuzqre.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shangyingyoupin.top/gtxiamfqph.html

Ruby: warn "err"
来源：http://hz.sufxvd.cn/gtdyhypwof.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shangyingyoupin.top/gthxnmkkae.html

[M07] 判断是否为主入口
来源：http://hz.cheryme.top/gtupibkjtm.html

Py:   if __name__ == "__main__":
来源：http://hz.guowangkeji.top/gtheuloxou.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.fengsongda.top/gtxhumuxjg.html

JS:   require.main === module
来源：http://hz.tian-w.cn/gtqfvtbuuj.html

TS:   require.main === module
来源：http://hz.sufxvd.cn/gtfmztchdl.html

Java: public static void main(String[] args)
来源：http://hz.quarkkingdee.top/gtkcskqaaw.html

Go:   func main()
来源：http://hz.hongshengwenyu.top/gtonuzhtaw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ywan-chungtsiang.top/gtxkgbbgnf.html

C#:   static void Main(string[] args)
来源：http://hz.pycfn.com/gtslcqwsgc.html

[M08] 获取系统与运行时信息
来源：http://hz.zdqjudy.top/gtjmjokokq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yongpay.top/gtonncdydz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gogol.net.cn/gtgebraisl.html

JS:   process.platform;  process.version
来源：http://hz.haohaochexian.top/gthziuzjhl.html

TS:   process.platform;  process.version
来源：http://hz.ydjk.org.cn/gtcweubets.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.vqdsnc.cn/gtdryvrykn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.c1oappe.top/gtguscdrgg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.iojbl.cn/gtwjbiovse.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.andypj.xyz/gtcoodpjou.html

================================================================================
来源：http://hz.xylfe.cn/gtfghkrcgv.html

N. 数据结构与算法
来源：http://hz.gotoacloud.top/gtnttyrlyq.html

================================================================================
来源：http://hz.havefunace.top/gthnuvqsia.html

[N01] 二分查找（有序数组）
来源：http://hz.hongshengwenyu.top/gtwpmozfka.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.cqqwz.cn/gthtudmzxz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.fengsongda.top/gthywxrieq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.9152youxi.cn/gtundhzmzr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.meibo888.top/gtiddsgwvn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.tianlin.xyz/gtehkvplrz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yj20258.top/gtolblrkil.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.pycfn.com/gtpnkddaro.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xuanzx.com/gtoebdbnwb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zycfv.cn/gtncnbpxip.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ehwqpu.com/gtwwzmcaql.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.aizwys.cn/gthvtbthfh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhijiandao.cn/gtvfvlhbpg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangtech.top/gtbanoubcb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sysykeji.top/gtbeqxlafk.html

Go:   slices.Sort(arr)
来源：http://hz.svipenyu.cn/gtwtzqibdw.html

Ruby: arr.sort
来源：http://hz.nanxinkj.top/gtqbilxlcc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ppjwa.cn/gtadnmhway.html

[N03] 快速排序（分治示例）
来源：http://hz.andypj.xyz/gtltoxsmty.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhiwuduotai.top/gtfsovwjvo.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hongshengwenyu.top/gttookuqdt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.iojbl.cn/gtzzlifscl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yangfankeji.com/gtkirtasvi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.kuanghao11.cn/gtbtnevmci.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xuetiantiany.cn/gthqbjxfvn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yongpay.top/gtqtpkcbyo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jinghuilouyu.cn/gtdpxdiwik.html

[N04] 斐波那契数列
来源：http://hz.hnxiangtu.top/gtnpoqiyxz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xuetiantiany.cn/gtekitbgot.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cdnleiting.top/gtetwujpyw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigfzy.top/gtcbosegoz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daxiang520.top/gtarpjssyd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.c1oappe.top/gtcadxunxp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ydzc1.top/gtnmbbqqqn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.chenlongwang.top/gttfgtybcs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sysykeji.top/gtjtmjtsvj.html

[N05] 最大公约数
来源：http://hz.tian-w.cn/gttnykcdnx.html

Py:   math.gcd(a, b)
来源：http://hz.xinyue.icu/gthgvdmqlk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhaomingkeji.xyz/gtxagdnvzp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daria6918.cn/gtsrrnyoot.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fzhhl.top/gtsmauaftx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jianghu66.top/gtzbnuljmm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.mhx1999.top/gtmbzzvldb.html

Ruby: a.gcd(b)
来源：http://hz.yangfankeji.com/gtanryktsv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.redwolf501.top/gtyzowcmdo.html

[N06] 判断回文字符串
来源：http://hz.tian-w.cn/gtavpwglzn.html

Py:   s == s[::-1]
来源：http://hz.gotoacloud.top/gtyjqxfhjh.html

PHP:  $s === strrev($s);
来源：http://hz.9152youxi.cn/gthwvaqljl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtirslchya.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gtdijyesjj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.feifeiyinyue.top/gtrguedund.html

Go:   // 双指针从两端比较
来源：http://hz.c1oappe.top/gtmmjxpxsc.html

Ruby: s == s.reverse
来源：http://hz.yonumen.top/gtndrowqfi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tian-w.cn/gtazfejuxb.html

[N07] 两数之和（返回下标）
来源：http://hz.52xcode.cn/gtaoswstyj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.haohaochexian.top/gtawmfmvzb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.pycfn.com/gtjwkkocxk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shanyushiyangtech.top/gtlwpeaqjx.html

TS:   // 手写 Map<string, number>
来源：http://hz.yuanzhike.top/gtdmkpvtfx.html

Java: // 手写 HashMap
来源：http://hz.jinghuilouyu.cn/gthxskmwts.html

Go:   // 手写 map[int]int
来源：http://hz.redwolf501.top/gtlnizxpxa.html

Ruby: // 手写 Hash
来源：http://hz.yvedp.cn/gtmbpqdecv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xuetiantiany.cn/gtjicdrjqo.html

[N08] 生成全排列
来源：http://hz.wangshuangyany.cn/gtiwsskdxv.html

Py:   itertools.permutations(arr)
来源：http://hz.dianchejie.cn/gtwgtqfway.html

PHP:  // 手写递归交换
来源：http://hz.xuanzx.com/gtcbcczbeq.html

JS:   // 手写回溯递归
来源：http://hz.hnqzz.top/gthpqwznvu.html

TS:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtlxzqqcat.html

Java: // 手写回溯递归
来源：http://hz.yj20258.top/gtnxzvlvdx.html

Go:   // 手写回溯递归
来源：http://hz.cashguo.top/gtzptnqtvh.html

Ruby: arr.permutation.to_a
来源：http://hz.ydzc1.top/gttdkymcdp.html

C#:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtrshaeztz.html

[N09] 栈与队列
来源：http://hz.chenzaomai.com/gtbsqtwvjc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hnqzz.top/gtpicmjpkm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.fengsongda.top/gtrkciwtow.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xingfuxueyuan.xyz/gtgclsllhm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj20258.top/gtbizxqmni.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.nanxuanxn.top/gteivhgyzn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jqgufenzy.top/gtfkwelrfh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cashguo.top/gtqychixbz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinyuanbaomall.cn/gtbvdcyxli.html

[N10] 链表节点定义
来源：http://hz.sxryk.cn/gtdmxrrfdh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.chenlongwang.top/gtkyeburkh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.snrcjt.cn/gtvscuqopm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xylfe.cn/gthjqujmjp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jqgfzy.top/gturdsgjea.html

Java: class Node { int v; Node next; }
来源：http://hz.xuanzx.com/gtbsuppilw.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.meibo888.top/gtgsoilnre.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.redwolf501.top/gtalvxfvgs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.havefunace.top/gtvsavhsqn.html

[N11] 二叉树中序遍历
来源：http://hz.kuanghao11.cn/gtcvdxltou.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zycfv.cn/gtjkjyrgqg.html

PHP:  // 手写递归函数
来源：http://hz.hysaishi.cn/gtimoblysz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydzc1.top/gtukrziigh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydjk.org.cn/gtspoytnrm.html

Java: // 手写递归
来源：http://hz.zhongyouzk.top/gtgifswrat.html


<!-- 参考信息 -->