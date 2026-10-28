代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://hz.9152youxi.cn/gtrsvdhuyd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yuanzhike.top/gtynouljdr.html

[K04] 读取 JSON 文件
来源：http://hz.hongshengwenyu.top/gtijkzyqkv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hywenlv.cn/gtfsrezimi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hammf.cn/gtnsaumqpw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenjidiqi.icu/gtijecpnyi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhixingplan.top/gttqqxdpsg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.0kj1m.cn/gtjfaaqkjk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hfpthk.cn/gtnldphlfr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.pengpengdd.cyou/gtowftvzbv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.chenjidiqi.icu/gtzzmrcept.html

[K05] 深拷贝对象
来源：http://hz.jyoumei.cn/gtcaxeolto.html

Py:   copy.deepcopy(obj)
来源：http://hz.tanke756.top/gtnvrltiev.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xingfuxueyuan.xyz/gtkdxuqyoo.html

JS:   structuredClone(obj)
来源：http://hz.cucudq.cn/gtmjnypqia.html

TS:   structuredClone(obj)
来源：http://hz.havefunace.top/gtitzlomfv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.0kj1m.cn/gtazxmdshj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sufxvd.cn/gtesboamvf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.0kj1m.cn/gttkurqyia.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhiwuduotai.top/gtyqulztcq.html

[K06] 解析 URL 查询串
来源：http://hz.zdqjudy.top/gtczhlbewz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinqigfzy.top/gtucjtcbnk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shzxlz.cn/gtdgurenuc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtnqeopbjq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xylfe.cn/gtmoafxqyh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ppjwa.cn/gthpoangqz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj20258888.top/gtyntnuack.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xziqi.cn/gtwkisxtde.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtbbqgfwpk.html

[K07] 进制转换
来源：http://hz.guannengcc.top/gtidngvwel.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ehwqpu.com/gtcwuqcuzr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tanke756.top/gtrmdbhaoy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gtnhkttter.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cdnleiting.top/gtsirciheg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.chenlongwang.top/gttfbvqzlb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hysaishi.cn/gtkyplymec.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.daxiang520.top/gtldxmzxck.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xuanzx.com/gtgkmzmsmd.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinghuilouyu.cn/gtdecxaepo.html

Py:   pickle.dumps(obj)
来源：http://hz.dashuyun.cn/gtmtjevocy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shanyushiyangkeji.top/gtzoywngcs.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.nanxinkj.top/gttogbwejx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.sysykeji.top/gtpszkwagr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.c1oappe.top/gtwqxwwrsc.html

Go:   encoding/gob
来源：http://hz.kuanghao11.cn/gtogsarwtk.html

Ruby: Marshal.dump(obj)
来源：http://hz.tianlin.xyz/gtcprwvdhp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.fengsongda.top/gtzgxqtgwn.html

================================================================================
来源：http://hz.zhixingplan.top/gtzzppzxrq.html

L. 网络请求
来源：http://hz.xuanzx.com/gtydtznfyg.html

================================================================================
来源：http://hz.quarkkingdee.top/gtmiftltwi.html

[L01] 发送 GET 请求
来源：http://hz.cqqwz.cn/gtljymjylx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cdnleiting.top/gtbdaynrhc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hongshengwenyu.top/gthsqsgbdg.html

JS:   await fetch(url)
来源：http://hz.zhengqikj.top/gtbuvtsrqo.html

TS:   await fetch(url)
来源：http://hz.chenjidiqi.icu/gttetsjkmn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhijiandao.cn/gtxrrtvita.html

Go:   resp, err := http.Get(url)
来源：http://hz.shangyingyoupin.top/gteefygbqa.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.dianchejie.cn/gtnpihyiyr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj202588.top/gtcikucgqt.html

[L02] 发送 POST JSON
来源：http://hz.gogol.net.cn/gtoksrnoru.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.smart0.xyz/gthjbqobvk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhongyouzk.top/gtpepgfapa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yueranfly.top/gtleyanafh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hywenlv.cn/gtbqfhwlsr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yanxiufei.cn/gtybxhjhtj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sxryk.cn/gtkbqrgrew.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.tanke756.top/gtriqweqos.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.snrcjt.cn/gtstezbjkn.html

[L03] 设置自定义请求头
来源：http://hz.jiagoushi.top/gtadpseisk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.c1oappe.top/gteipxqfue.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.dashuyun.cn/gtjjozjicl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dianchejie.cn/gtaszrdreb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenlongwang.top/gtwwylmpob.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.daria6918.cn/gtuhpxihwp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinqigufen.top/gtklvwnnnw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.0kj1m.cn/gtjdbbimzp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.havefunace.top/gtddmwqicg.html

[L04] 设置超时
来源：http://hz.c1oappe.top/gtrxjkocbw.html

Py:   requests.get(url, timeout=5)
来源：http://hz.quarkkingdee.top/gtbyfbsmzx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.birdmap.top/gtofagknvs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnxiangtu.top/gtfokfxfxa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigufen.top/gtssnfsvfl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhoulong.xyz/gtqogwuwek.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xingfuxueyuan.xyz/gtuseeecun.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ybcxt.top/gtlcxwieny.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.pengpengdd.cyou/gthfrtcuib.html

[L05] 上传文件（multipart）
来源：http://hz.jinyuanbaomall.cn/gttuznhasj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.iojbl.cn/gtpjyhdwba.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.vqdsnc.cn/gtbpoiaifn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zdqjudy.top/gtmakithos.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuanzhike.top/gtbaemyfwq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yuanzhike.top/gtklkfeqxh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhengqikj.top/gtckxwnrly.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.haohaochexian.top/gtlcvkphlg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxinkj.top/gthakuleha.html

[L06] 解析响应为 JSON
来源：http://hz.hfpthk.cn/gtrstpzxey.html

Py:   resp.json()
来源：http://hz.zhoulong.xyz/gtzshteoem.html

PHP:  json_decode($body, true);
来源：http://hz.hnqzz.top/gtvyrqdnvb.html

JS:   await resp.json()
来源：http://hz.hywenlv.cn/gtmouwemgq.html

TS:   await resp.json()
来源：http://hz.hnqzz.top/gtygmquwom.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinqigufen.top/gtdwquhrhi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yongpay.top/gtfxmhcjsh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.vqdsnc.cn/gtwzxklnvz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cashguo.top/gtbxaeajql.html

[L07] 处理 HTTP 状态码
来源：http://hz.shanyushiyangtech.top/gtvxyoeuqs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhijiandao.cn/gtpjvfujaz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cucudq.cn/gtyopdmpxc.html

JS:   resp.ok;  resp.status
来源：http://hz.yongpay.top/gtyhfukhdt.html

TS:   resp.ok;  resp.status
来源：http://hz.yangfankeji.com/gtatnfdnkq.html

Java: resp.statusCode()
来源：http://hz.chenjidiqi.icu/gtvxwtdqkt.html

Go:   resp.StatusCode
来源：http://hz.yj20258.top/gtyjqvscua.html

Ruby: resp.code.to_i
来源：http://hz.zhixingplan.top/gttjbcniok.html

C#:   (int)resp.StatusCode
来源：http://hz.nwbrower.top/gtjmhgnexu.html

[L08] 并发请求多个地址
来源：http://hz.316326.xyz/gtcmlciboe.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhiwuduotai.top/gtonkgiyzm.html

PHP:  curl_multi_init() 系列
来源：http://hz.aibaodan.cn/gtyhkzlegv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shuidangran.top/gtqqbncctz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhongyouzk.top/gtwqzxwrll.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hongshengwenyu.top/gtkdxxngxy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ydjk.org.cn/gtxcocmgrs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.fengsongda.top/gtaughbgsb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinqigfzy.top/gtykkgphvw.html

================================================================================
来源：http://hz.shuidangran.top/gtevorgrtf.html

M. 命令行 / 进程 / 环境
来源：http://hz.shanyushiyangtech.top/gtdehubllg.html

================================================================================
来源：http://hz.hywenlv.cn/gtfofcmdgp.html

[M01] 读取命令行参数
来源：http://hz.hongshengwenyu.top/gtwlanowsz.html

Py:   sys.argv[1:]
来源：http://hz.yuanzhike.top/gtrmolwwic.html

PHP:  $argv;  $argc;
来源：http://hz.meibo888.top/gtwymgkgud.html

JS:   process.argv.slice(2)
来源：http://hz.ywan-chungtsiang.top/gtxcvsqdkn.html

TS:   process.argv.slice(2)
来源：http://hz.ivvv.top/gtsssytjtr.html

Java: args 数组（main 方法参数）
来源：http://hz.shanyushiyangtech.top/gtsajvsyru.html

Go:   os.Args[1:]
来源：http://hz.shangyingyoupin.top/gtdfogrnbd.html

Ruby: ARGV
来源：http://hz.jinqigfzy.top/gtnqckxyml.html

C#:   args 数组（Main 方法参数）
来源：http://hz.bjfxy.top/gtcvqhvzlk.html

[M02] 读取环境变量
来源：http://hz.jyoumei.cn/gtxpsfeipc.html

Py:   os.environ.get("HOME")
来源：http://hz.ydjk.org.cn/gtsietvwmw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.bjfxy.top/gtqzvplbrw.html

JS:   process.env.HOME
来源：http://hz.cashguo.top/gtbzdqwvhg.html

TS:   process.env.HOME
来源：http://hz.shangyingyoupin.top/gtelyiwezd.html

Java: System.getenv("HOME")
来源：http://hz.nwbrower.top/gtprfxokxj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhijiandao.cn/gttvrkgaxj.html

Ruby: ENV["HOME"]
来源：http://hz.yangfankeji.com/gtrcujlzjr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhixingplan.top/gtwksbjqvh.html

[M03] 执行外部命令
来源：http://hz.jiagoushi.top/gtfjwlaplm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.bjfxy.top/gtqazfqjqy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.pycfn.com/gtiwqbszdb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.meibo888.top/gtzxuizvss.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hammf.cn/gtgsddwiwb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zycfv.cn/gturauipqg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.snrcjt.cn/gtsvrkwkss.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.feifeiyinyue.top/gtwyskaorh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.dianchejie.cn/gtutcrngdg.html

[M04] 获取当前工作目录
来源：http://hz.hammf.cn/gtwczuymwl.html

Py:   os.getcwd()
来源：http://hz.yonumen.top/gtcebbnumo.html

PHP:  getcwd();
来源：http://hz.cheryme.top/gttoijwhsc.html

JS:   process.cwd()
来源：http://hz.yuanzhike.top/gthpokvzvs.html

TS:   process.cwd()
来源：http://hz.zhiwuduotai.top/gtokghhzmt.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yonumen.top/gtqvooxkho.html

Go:   os.Getwd()
来源：http://hz.ywan-chungtsiang.top/gtjxirdlmb.html

Ruby: Dir.pwd
来源：http://hz.yongpay.top/gtxbhtbtno.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.9152youxi.cn/gtnlmmjink.html

[M05] 设置退出码
来源：http://hz.jinqigfzy.top/gtapoatsjg.html

Py:   sys.exit(1)
来源：http://hz.cashguo.top/gtigjbxweb.html

PHP:  exit(1);
来源：http://hz.jianghu66.top/gtxohyphxp.html

JS:   process.exit(1)
来源：http://hz.dianchejie.cn/gtblzlicoh.html

TS:   process.exit(1)
来源：http://hz.nanxinkj.top/gtanlaxljb.html

Java: System.exit(1)
来源：http://hz.havefunace.top/gtmyneehan.html

Go:   os.Exit(1)
来源：http://hz.shanyushiyangkeji.top/gtbcpzlbrz.html

Ruby: exit 1
来源：http://hz.chenjidiqi.icu/gtzzgqpopk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj202588.top/gttovmytrw.html

[M06] 向标准错误输出
来源：http://hz.0kj1m.cn/gtohnjdofs.html

Py:   print("err", file=sys.stderr)
来源：http://hz.chenlongwang.top/gtgfujhrbp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ivvv.top/gtsxkexyta.html

JS:   console.error("err")
来源：http://hz.52xcode.cn/gtmcqdfgop.html

TS:   console.error("err")
来源：http://hz.dianchejie.cn/gtukmzfpdy.html

Java: System.err.println("err")
来源：http://hz.fzhhl.top/gtowncnpty.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hfpthk.cn/gtruvvjlni.html

Ruby: warn "err"
来源：http://hz.feifeiyinyue.top/gtxojounfp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhiwuduotai.top/gtwzgcifip.html

[M07] 判断是否为主入口
来源：http://hz.meibo888.top/gtopsrebil.html

Py:   if __name__ == "__main__":
来源：http://hz.gogol.net.cn/gtifnwczde.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinqigufen.top/gtvcxtiflo.html

JS:   require.main === module
来源：http://hz.shanyushiyangkeji.top/gtcsgyjknb.html

TS:   require.main === module
来源：http://hz.haohaochexian.top/gtugyhzywy.html

Java: public static void main(String[] args)
来源：http://hz.hongshengwenyu.top/gtazfiawtm.html

Go:   func main()
来源：http://hz.c1oappe.top/gtintiacid.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sxryk.cn/gtzoahqxpc.html

C#:   static void Main(string[] args)
来源：http://hz.yangfankeji.com/gtaeaikrmo.html

[M08] 获取系统与运行时信息
来源：http://hz.mhx1999.top/gthikdugei.html

Py:   platform.system();  platform.python_version()
来源：http://hz.wangshuangyany.cn/gtskmvdced.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zdqjudy.top/gtahqspvbm.html

JS:   process.platform;  process.version
来源：http://hz.gzhubu.top/gtyybkstbu.html

TS:   process.platform;  process.version
来源：http://hz.shzxlz.cn/gtgspokvot.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tianlin.xyz/gtpoiefmgm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhaomingkeji.xyz/gtbuunbbav.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yuanzhike.top/gtawixizgs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hammf.cn/gttaknbtng.html

================================================================================
来源：http://hz.iojbl.cn/gttmtkxdra.html

N. 数据结构与算法
来源：http://hz.ybcxt.top/gtnsjgwfcf.html

================================================================================
来源：http://hz.guowangkeji.top/gthfpjlobg.html

[N01] 二分查找（有序数组）
来源：http://hz.nanxinkj.top/gtjecyytjh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.fzhhl.top/gtfhlgjavs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yuxming.cn/gtdshgnvak.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhengqikj.top/gtjcnfszsx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gzhubu.top/gtunueowcw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.nwbrower.top/gtsphwyddt.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jianghu66.top/gtsymdaomc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhiwuduotai.top/gtwdmwzfma.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jiagoushi.top/gttryefgoa.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yonumen.top/gtklmvmasb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.svipenyu.cn/gtaefaxwfv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shanyushiyangtech.top/gtremfxecj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tanke756.top/gtygyhqrms.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fengsongda.top/gtyqgzlcyj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hnqzz.top/gtheysxnlm.html

Go:   slices.Sort(arr)
来源：http://hz.nanxuanxn.top/gtyhupgozi.html

Ruby: arr.sort
来源：http://hz.ywan-chungtsiang.top/gtxoxjzfue.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shanyushiyangkeji.top/gtjfgxxjre.html

[N03] 快速排序（分治示例）
来源：http://hz.pycfn.com/gtumofdtvz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.iojbl.cn/gthjiolzgw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.andypj.xyz/gtbxeqxntw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cashguo.top/gtmwwvfigl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.snrcjt.cn/gtywylfmsp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj20258888.top/gtudnhtvsd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhoulong.xyz/gtohnjdslu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jiagoushi.top/gtquxkflmk.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhiwuduotai.top/gtaeggegyi.html

[N04] 斐波那契数列
来源：http://hz.aizwys.cn/gtsqgwqjjm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangtech.top/gtrosnrbwt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jqgufenzy.top/gtzsuaiknv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ppjwa.cn/gthnzorrll.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dashuyun.cn/gtyskerfom.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.fengsongda.top/gtuhtkywbj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shuidangran.top/gtjvudvyrj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hnxiangtu.top/gtxshpvenr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xinyue.icu/gtrapbcvay.html

[N05] 最大公约数
来源：http://hz.daxiang520.top/gtjceebpau.html

Py:   math.gcd(a, b)
来源：http://hz.cashguo.top/gtgvqjlyrs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xuetiantiany.cn/gtudysdtix.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhijiandao.cn/gtnwspefhd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ppjwa.cn/gtbkzocqro.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.iojbl.cn/gtsqyutclu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.aizwys.cn/gttyxmzeft.html

Ruby: a.gcd(b)
来源：http://hz.zycfv.cn/gtyibnvktx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hywenlv.cn/gtgesrislo.html

[N06] 判断回文字符串
来源：http://hz.yuxming.cn/gtegwlvdvw.html

Py:   s == s[::-1]
来源：http://hz.cdnleiting.top/gtarnngtnb.html

PHP:  $s === strrev($s);
来源：http://hz.kuanghao11.cn/gtjmuhqliy.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cashguo.top/gteklozdbo.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gaohongyu789.top/gtiytcoibw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.316326.xyz/gtvvhffeul.html

Go:   // 双指针从两端比较
来源：http://hz.tanke756.top/gtjlkptkvz.html

Ruby: s == s.reverse
来源：http://hz.dianchejie.cn/gtxkoktvmk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ywan-chungtsiang.top/gttuaoirka.html

[N07] 两数之和（返回下标）
来源：http://hz.sxryk.cn/gtiqzlpifp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.kuanghao11.cn/gteuojdmrc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.smart0.xyz/gtcybhsqqn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shanyushiyangtech.top/gtmnbapbdn.html

TS:   // 手写 Map<string, number>
来源：http://hz.mhx1999.top/gtxqgkabws.html

Java: // 手写 HashMap
来源：http://hz.shzxlz.cn/gtioqmgipy.html

Go:   // 手写 map[int]int
来源：http://hz.jqgufenzy.top/gtjovupeqz.html

Ruby: // 手写 Hash
来源：http://hz.ydzc1.top/gtvchqjmgs.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yanxiufei.cn/gtmymchdwf.html

[N08] 生成全排列
来源：http://hz.dashuyun.cn/gtzhwrstlq.html

Py:   itertools.permutations(arr)
来源：http://hz.shanyushiyangkeji.top/gtwckumwfm.html

PHP:  // 手写递归交换
来源：http://hz.quarkkingdee.top/gtooxfmjzs.html

JS:   // 手写回溯递归
来源：http://hz.jiagoushi.top/gtgxrulkoi.html

TS:   // 手写回溯递归
来源：http://hz.cqqwz.cn/gtbxszjqry.html

Java: // 手写回溯递归
来源：http://hz.fengsongda.top/gtbwduukha.html

Go:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtqhibwnfc.html

Ruby: arr.permutation.to_a
来源：http://hz.xylfe.cn/gtwgrlcqkh.html

C#:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtdxkfkald.html

[N09] 栈与队列
来源：http://hz.quarkkingdee.top/gtlhsunfxj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hammf.cn/gtmtspcqyw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.wangshuangyany.cn/gtusmgyqkb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.nanxinkj.top/gtsrdnepry.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.aizwys.cn/gtxtjhyitz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jqgfzy.top/gtihqgonqq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xingfuxueyuan.xyz/gtotpwtqlj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.chenlongwang.top/gtovbrjbsh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.fzhhl.top/gtneccjhld.html

[N10] 链表节点定义
来源：http://hz.jinqigfzy.top/gtkexxpeah.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xingfuxueyuan.xyz/gtmnxucytv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.dashuyun.cn/gtvsttskgk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.chenzaomai.com/gtfdvugfzc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ywan-chungtsiang.top/gttdzozndm.html

Java: class Node { int v; Node next; }
来源：http://hz.cashguo.top/gtvydmalvl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.redwolf501.top/gtfiiqyvcf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.bjfxy.top/gtdwmgehgg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ywan-chungtsiang.top/gtaooixelc.html

[N11] 二叉树中序遍历
来源：http://hz.xingfuxueyuan.xyz/gtyvzvxvgw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhengqikj.top/gtkbnwieey.html

PHP:  // 手写递归函数
来源：http://hz.c1oappe.top/gtdqwitedv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yongpay.top/gtzcbrojtq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.feifeiyinyue.top/gtcxqoxbmv.html

Java: // 手写递归
来源：http://hz.zhengqikj.top/gtozxvslxy.html

Go:   // 手写递归
来源：http://hz.daria6918.cn/gtbqjqxdtc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.316326.xyz/gtemqysbhw.html

C#:   // 手写递归
来源：http://hz.gotoacloud.top/gtsqagbjzt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhoulong.xyz/gtnbzfiewc.html


<!-- 参考信息 -->