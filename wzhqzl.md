代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nanxinkj.top/gtqkjbqecq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.c1oappe.top/gtqqgdvdkb.html

[K04] 读取 JSON 文件
来源：http://hz.nanxuanxn.top/gtqpxlsitg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sxryk.cn/gthhdnrlhd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinghuilouyu.cn/gtsdpnxtnf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.andypj.xyz/gtmyvesnsn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangkeji.top/gtmzlqemyb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yueranfly.top/gtfaygjipw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ehwqpu.com/gteblfmqoz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.havefunace.top/gtzhhwqljs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.guannengcc.top/gtvjljwhok.html

[K05] 深拷贝对象
来源：http://hz.zhaomingkeji.xyz/gtjrvyqjjf.html

Py:   copy.deepcopy(obj)
来源：http://hz.sxryk.cn/gtbozfadhi.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ppjwa.cn/gtjubrfhwz.html

JS:   structuredClone(obj)
来源：http://hz.shangyingyoupin.top/gtuyncmcnz.html

TS:   structuredClone(obj)
来源：http://hz.cheryme.top/gtviombpkc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.andypj.xyz/gtohqpgjqc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jqgfzy.top/gtkxeiaxle.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hysaishi.cn/gtswmezigb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.aizwys.cn/gtvxrnmlck.html

[K06] 解析 URL 查询串
来源：http://hz.9152youxi.cn/gtvrfyokkr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zdqjudy.top/gthtwstvqg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.wangdashe.top/gtkyztkade.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ywan-chungtsiang.top/gtzhchrcrx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jyoumei.cn/gtufwjsjvy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.tanke756.top/gtrleehpfv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj20258.top/gtgojbuglj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jiagoushi.top/gtvkvqfmco.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yonumen.top/gtdsipvvre.html

[K07] 进制转换
来源：http://hz.aizwys.cn/gtcfxkgceg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhijiandao.cn/gtnyoxntiw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhengqikj.top/gtkinrbiru.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.kuanghao11.cn/gtoiyqtqwp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shangyingyoupin.top/gttcmdgyqb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gtcrfvypqh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinqigufen.top/gtmkvdlorb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.chenjidiqi.icu/gtbyswzvqp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jiagoushi.top/gtrqatymqm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.bjfxy.top/gtzpvbouaa.html

Py:   pickle.dumps(obj)
来源：http://hz.yj20258.top/gttukmfwhc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinghuilouyu.cn/gteziaqgfm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.mhx1999.top/gtsjrizimh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yuxming.cn/gtigsbubar.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.vqdsnc.cn/gttpzcbpft.html

Go:   encoding/gob
来源：http://hz.nwbrower.top/gtatirgddi.html

Ruby: Marshal.dump(obj)
来源：http://hz.xinyue.icu/gtsoztinba.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ydzc1.top/gtjdskztii.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtqgxmfkfp.html

L. 网络请求
来源：http://hz.hywenlv.cn/gtttrgemnc.html

================================================================================
来源：http://hz.jiagoushi.top/gtgstoifce.html

[L01] 发送 GET 请求
来源：http://hz.jqgfzy.top/gtgzovlxsn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jiagoushi.top/gtezysxgvu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ydzc1.top/gtlklzckch.html

JS:   await fetch(url)
来源：http://hz.cdnleiting.top/gtqyilcpqm.html

TS:   await fetch(url)
来源：http://hz.chenzaomai.com/gtydlxalfe.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhixingplan.top/gtzhcecsey.html

Go:   resp, err := http.Get(url)
来源：http://hz.kuanghao11.cn/gtmatodcfz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.guannengcc.top/gtuwkufkcw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.tianlin.xyz/gtvzqqgidg.html

[L02] 发送 POST JSON
来源：http://hz.zhijiandao.cn/gtakioqwlm.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yj20258888.top/gtspwrpdho.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nanxuanxn.top/gtptuvbatx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ppjwa.cn/gtpwaapjfz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.haohaochexian.top/gttonkgqun.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.daxiang520.top/gtebnnhpln.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.tian-w.cn/gthhxwgjaj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.316326.xyz/gtbpgozmca.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.birdmap.top/gtrqsjalit.html

[L03] 设置自定义请求头
来源：http://hz.vqdsnc.cn/gttxyxpivf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cdnleiting.top/gtgsaitbmg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.guannengcc.top/gtrafhbkff.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gogol.net.cn/gtrnupisll.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aizwys.cn/gtwfcdpnkk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jianghu66.top/gtytgsihnr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hnqzz.top/gtagdjlpaw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jianghu66.top/gtdnwjsrfu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xinyue.icu/gtmasgcdgo.html

[L04] 设置超时
来源：http://hz.hywenlv.cn/gthjwdfany.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jianghu66.top/gtyydsncks.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.haohaochexian.top/gttppnjigt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ivvv.top/gtgvzyqpfy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhengqikj.top/gttpcvqeqt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ywan-chungtsiang.top/gtgjsjilpx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ehwqpu.com/gtzmlqqzxc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.iojbl.cn/gtogjmqfod.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.svipenyu.cn/gthjtxbbkd.html

[L05] 上传文件（multipart）
来源：http://hz.smart0.xyz/gtjhhxtszj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinqigufen.top/gtlqjzpclj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cdnleiting.top/gtycvtdnww.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhaomingkeji.xyz/gtxgazxwjo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.iojbl.cn/gtkllbhtlq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hysaishi.cn/gtykvwflqm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.c1oappe.top/gtwkccdzrs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.dianchejie.cn/gtucrzbudz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cashguo.top/gttximyqyh.html

[L06] 解析响应为 JSON
来源：http://hz.jyoumei.cn/gtbjjswacc.html

Py:   resp.json()
来源：http://hz.zycfv.cn/gtkcooqdmv.html

PHP:  json_decode($body, true);
来源：http://hz.cqqwz.cn/gtphssadqe.html

JS:   await resp.json()
来源：http://hz.jinqigufen.top/gtlswugwyc.html

TS:   await resp.json()
来源：http://hz.dashuyun.cn/gtfdfylojc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hysaishi.cn/gtmzkknlqx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.vqdsnc.cn/gtiempqzyz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yuxming.cn/gtdeukqivj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.havefunace.top/gtxujgiqec.html

[L07] 处理 HTTP 状态码
来源：http://hz.hnxiangtu.top/gtcunhqlmd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.nwbrower.top/gtraxdmjjr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.feifeiyinyue.top/gtitweszaa.html

JS:   resp.ok;  resp.status
来源：http://hz.c1oappe.top/gtwfxdlozi.html

TS:   resp.ok;  resp.status
来源：http://hz.zhengqikj.top/gtrggdkcsw.html

Java: resp.statusCode()
来源：http://hz.yj20258.top/gtvdockpsm.html

Go:   resp.StatusCode
来源：http://hz.tanke756.top/gtmvgojecv.html

Ruby: resp.code.to_i
来源：http://hz.ehwqpu.com/gtcpendtus.html

C#:   (int)resp.StatusCode
来源：http://hz.birdmap.top/gtxozmsotj.html

[L08] 并发请求多个地址
来源：http://hz.hammf.cn/gtyweiqaqp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.snrcjt.cn/gtcqchewml.html

PHP:  curl_multi_init() 系列
来源：http://hz.shzxlz.cn/gtbtmfmybv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pycfn.com/gtcwzsvqzz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yangfankeji.com/gtltfjhink.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sweek.top/gtcrdzujet.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.mhx1999.top/gtsxyidbmp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yueranfly.top/gtmgdffujk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hammf.cn/gtvyxfzufg.html

================================================================================
来源：http://hz.bjfxy.top/gtkfcaxqot.html

M. 命令行 / 进程 / 环境
来源：http://hz.wangshuangyany.cn/gtbuypudqz.html

================================================================================
来源：http://hz.jianghu66.top/gteckzults.html

[M01] 读取命令行参数
来源：http://hz.xuetiantiany.cn/gtmqzeniku.html

Py:   sys.argv[1:]
来源：http://hz.shangyingyoupin.top/gtfhpittzx.html

PHP:  $argv;  $argc;
来源：http://hz.havefunace.top/gtygujchvc.html

JS:   process.argv.slice(2)
来源：http://hz.yj20258888.top/gthzskgpwt.html

TS:   process.argv.slice(2)
来源：http://hz.yj20258888.top/gtkjvuapsc.html

Java: args 数组（main 方法参数）
来源：http://hz.jqgufenzy.top/gtesilzdru.html

Go:   os.Args[1:]
来源：http://hz.hywenlv.cn/gtdzcceayu.html

Ruby: ARGV
来源：http://hz.jianghu66.top/gtydavnsas.html

C#:   args 数组（Main 方法参数）
来源：http://hz.quarkkingdee.top/gtnkymqhac.html

[M02] 读取环境变量
来源：http://hz.ydzc1.top/gthqgrwlxy.html

Py:   os.environ.get("HOME")
来源：http://hz.gotoacloud.top/gtgwoosbbf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shanyushiyangtech.top/gtrcvygobm.html

JS:   process.env.HOME
来源：http://hz.jiagoushi.top/gthctocwbo.html

TS:   process.env.HOME
来源：http://hz.daria6918.cn/gtfxrpzkdg.html

Java: System.getenv("HOME")
来源：http://hz.fzhhl.top/gtwbgoaydr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ydjk.org.cn/gtzernvhgm.html

Ruby: ENV["HOME"]
来源：http://hz.pengpengdd.cyou/gtpinatwhd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.daria6918.cn/gtkuenjeiu.html

[M03] 执行外部命令
来源：http://hz.jianghu66.top/gtqxdoawet.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.nanxuanxn.top/gthillfjwn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhongyouzk.top/gtpeeurmdh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj20258888.top/gtvsqpvbon.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.pengpengdd.cyou/gtkrneovhu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.shanyushiyangkeji.top/gtmohqlwsn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.feifeiyinyue.top/gtispjhaxp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gaohongyu789.top/gtzucfwwkv.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhaomingkeji.xyz/gtnwewmcju.html

[M04] 获取当前工作目录
来源：http://hz.xinyue.icu/gtfnioeesl.html

Py:   os.getcwd()
来源：http://hz.cqqwz.cn/gthxitfmfq.html

PHP:  getcwd();
来源：http://hz.cqqwz.cn/gtpanvgleq.html

JS:   process.cwd()
来源：http://hz.sysykeji.top/gtcrdjjype.html

TS:   process.cwd()
来源：http://hz.feifeiyinyue.top/gtctkfgsfr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.smart0.xyz/gtfqnjxdxz.html

Go:   os.Getwd()
来源：http://hz.tanke756.top/gtmkvwksrk.html

Ruby: Dir.pwd
来源：http://hz.ywan-chungtsiang.top/gtgxvkihhe.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhiwuduotai.top/gtyekbeqbl.html

[M05] 设置退出码
来源：http://hz.52xcode.cn/gtpseedrjv.html

Py:   sys.exit(1)
来源：http://hz.meibo888.top/gtqgbzfsbn.html

PHP:  exit(1);
来源：http://hz.kuanghao11.cn/gtxifkqkxg.html

JS:   process.exit(1)
来源：http://hz.0kj1m.cn/gtnihrixfq.html

TS:   process.exit(1)
来源：http://hz.daria6918.cn/gtjophbkmo.html

Java: System.exit(1)
来源：http://hz.feifeiyinyue.top/gtiouwbysh.html

Go:   os.Exit(1)
来源：http://hz.cdnleiting.top/gtpkabppbm.html

Ruby: exit 1
来源：http://hz.nanxuanxn.top/gtudlbycaw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhiwuduotai.top/gtkvmljsge.html

[M06] 向标准错误输出
来源：http://hz.hfpthk.cn/gtaqstzayh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhaomingkeji.xyz/gteviblefb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinqigufen.top/gtzakjkujh.html

JS:   console.error("err")
来源：http://hz.nanxuanxn.top/gtqnfcgcjb.html

TS:   console.error("err")
来源：http://hz.shzxlz.cn/gtloqnburr.html

Java: System.err.println("err")
来源：http://hz.52xcode.cn/gtdzqjslfu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yangfankeji.com/gtzfwhibwo.html

Ruby: warn "err"
来源：http://hz.smart0.xyz/gtwxaybgmj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zdqjudy.top/gtlhcfvdvf.html

[M07] 判断是否为主入口
来源：http://hz.hfpthk.cn/gtvnspizxd.html

Py:   if __name__ == "__main__":
来源：http://hz.chenzaomai.com/gtkqoqsgdp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhixingplan.top/gtkdgafxzj.html

JS:   require.main === module
来源：http://hz.jinqigfzy.top/gtzgcippah.html

TS:   require.main === module
来源：http://hz.snrcjt.cn/gtrnqfwzau.html

Java: public static void main(String[] args)
来源：http://hz.ydjk.org.cn/gtyhcjlxfa.html

Go:   func main()
来源：http://hz.ybcxt.top/gtcukgqdaa.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.smart0.xyz/gtqnptygsp.html

C#:   static void Main(string[] args)
来源：http://hz.xylfe.cn/gtmkcuwurs.html

[M08] 获取系统与运行时信息
来源：http://hz.hywenlv.cn/gtwguhwdgt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.tian-w.cn/gtzpbyzahp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cashguo.top/gtlpuhilrc.html

JS:   process.platform;  process.version
来源：http://hz.quarkkingdee.top/gtmwvscjjv.html

TS:   process.platform;  process.version
来源：http://hz.birdmap.top/gtmrzokogj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ehwqpu.com/gtdgcswbyi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shzxlz.cn/gtzfncizca.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yanxiufei.cn/gtqzeeapxo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.tian-w.cn/gtdgbmlids.html

================================================================================
来源：http://hz.zhongyouzk.top/gtastogsel.html

N. 数据结构与算法
来源：http://hz.jinghuilouyu.cn/gtjlqjcshm.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtvbduneip.html

[N01] 二分查找（有序数组）
来源：http://hz.zhongyouzk.top/gtvqiomica.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yonumen.top/gtnfmxdgaq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ppjwa.cn/gtvicjtxrl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jianghu66.top/gtapkisgwf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.pycfn.com/gtpivmcftu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.aibaodan.cn/gtqaskwywq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xinyue.icu/gtwypwnrke.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.aizwys.cn/gttfbmmaam.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.pycfn.com/gtrptauelm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xziqi.cn/gtldzmrsil.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.guowangkeji.top/gthffwbgrr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.andypj.xyz/gtgmmnuxbf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.havefunace.top/gtvaxowqui.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sxryk.cn/gtpwbowjez.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.gotoacloud.top/gtunrdluqx.html

Go:   slices.Sort(arr)
来源：http://hz.chenlongwang.top/gtzbuiwwuv.html

Ruby: arr.sort
来源：http://hz.fengsongda.top/gtbryueohd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhoulong.xyz/gtroxqobpy.html

[N03] 快速排序（分治示例）
来源：http://hz.yuanzhike.top/gtgganneev.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.52xcode.cn/gtssgzkdpi.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yueranfly.top/gtbzakyfoy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guannengcc.top/gtdlsndcwp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydzc1.top/gtmksjwzua.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.gogol.net.cn/gtkplvpbfl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.0kj1m.cn/gtvppigigf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ydzc1.top/gtlngyjuez.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yuxming.cn/gttzsabfrc.html

[N04] 斐波那契数列
来源：http://hz.redwolf501.top/gtqehxwfsn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cucudq.cn/gtdqgrdhja.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xuetiantiany.cn/gtwkxgzxng.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.haohaochexian.top/gtfcyyizqo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.guowangkeji.top/gtbhnbdazp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.dashuyun.cn/gtpowoeswh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zycfv.cn/gtkqncbqga.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hnxiangtu.top/gtpbeqdljv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gaohongyu789.top/gtlljfjlgu.html

[N05] 最大公约数
来源：http://hz.fzhhl.top/gtumsgywuo.html

Py:   math.gcd(a, b)
来源：http://hz.sweek.top/gtuubycuoc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sxryk.cn/gtffkcxzlz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cqqwz.cn/gtpkmqjcaj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shzxlz.cn/gtgqidwwck.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.fengsongda.top/gtitbgecrp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinqigfzy.top/gtnzbzzxyg.html

Ruby: a.gcd(b)
来源：http://hz.jqgfzy.top/gtqlvqywgj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yj20258.top/gtvikkdrki.html

[N06] 判断回文字符串
来源：http://hz.52xcode.cn/gtjdfqgsfl.html

Py:   s == s[::-1]
来源：http://hz.aibaodan.cn/gtwfpicldw.html

PHP:  $s === strrev($s);
来源：http://hz.tianlin.xyz/gtbgschbeo.html

JS:   s === [...s].reverse().join("")
来源：http://hz.iojbl.cn/gtobjagppq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.316326.xyz/gtjhttrrfx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.redwolf501.top/gttmbbcorm.html

Go:   // 双指针从两端比较
来源：http://hz.mhx1999.top/gtuwhhrrcc.html

Ruby: s == s.reverse
来源：http://hz.jinqigfzy.top/gtwgkjjtxr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.9152youxi.cn/gtxluhaxdy.html

[N07] 两数之和（返回下标）
来源：http://hz.sufxvd.cn/gtgtuqnhar.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.svipenyu.cn/gtpkjpsvmr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xingfuxueyuan.xyz/gtwfkmjfdf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhiwuduotai.top/gtdpdatoks.html

TS:   // 手写 Map<string, number>
来源：http://hz.kuanghao11.cn/gtjguelfug.html

Java: // 手写 HashMap
来源：http://hz.yongpay.top/gtanbewlcg.html

Go:   // 手写 map[int]int
来源：http://hz.zdqjudy.top/gtkxvkocua.html

Ruby: // 手写 Hash
来源：http://hz.kuanghao11.cn/gtgojwracl.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gogol.net.cn/gtzwbgppio.html

[N08] 生成全排列
来源：http://hz.316326.xyz/gtvgdykiur.html

Py:   itertools.permutations(arr)
来源：http://hz.xinyue.icu/gtipsrbsgy.html

PHP:  // 手写递归交换
来源：http://hz.hfpthk.cn/gtdnbkhkqb.html

JS:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtjvkwuqou.html

TS:   // 手写回溯递归
来源：http://hz.pycfn.com/gtnvvkglet.html

Java: // 手写回溯递归
来源：http://hz.jqgfzy.top/gtdcgpwihj.html

Go:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtbytihffz.html

Ruby: arr.permutation.to_a
来源：http://hz.pycfn.com/gtcfmbqnqh.html

C#:   // 手写回溯递归
来源：http://hz.jyoumei.cn/gtmnryoljw.html

[N09] 栈与队列
来源：http://hz.hongshengwenyu.top/gtjmijrmgg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ehwqpu.com/gtxsosxinl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.smart0.xyz/gtxqrlomvn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jqgfzy.top/gtwnexaayy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.chenlongwang.top/gtcmotrwex.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shzxlz.cn/gtomlrqbca.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.meibo888.top/gtohpvsbqx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yanxiufei.cn/gtenhryisa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cashguo.top/gtfkogyhes.html

[N10] 链表节点定义
来源：http://hz.sweek.top/gtgnkwdcpm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yongpay.top/gtnztmyhbr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.iojbl.cn/gtsvdmrcru.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jinqigufen.top/gtjqxknqcn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yj20258888.top/gthdbcrlnp.html

Java: class Node { int v; Node next; }
来源：http://hz.cashguo.top/gtaygixkhn.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ppjwa.cn/gttvivcaul.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sysykeji.top/gtfdrbswze.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jiagoushi.top/gtgidqwcvb.html

[N11] 二叉树中序遍历
来源：http://hz.yj20258.top/gtkickebwa.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.fzhhl.top/gtcdveueio.html

PHP:  // 手写递归函数
来源：http://hz.smart0.xyz/gtakejvppq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.svipenyu.cn/gtdkakjsnd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.wangdashe.top/gtuiajprsl.html

Java: // 手写递归
来源：http://hz.chenjidiqi.icu/gtvirrkheo.html

Go:   // 手写递归
来源：http://hz.sweek.top/gtkpzbswhn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhixingplan.top/gtrvayehpy.html

C#:   // 手写递归
来源：http://hz.redwolf501.top/gtbnqjcqnv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yonumen.top/gtctuolexw.html


<!-- 参考信息 -->