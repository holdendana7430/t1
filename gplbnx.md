代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.chenlongwang.top/gtqiaanwfz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guannengcc.top/gteggmqrfe.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sxryk.cn/gtziqtgjgt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hnxiangtu.top/gtulpqnrmg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.quarkkingdee.top/gtewgtyjog.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yueranfly.top/gtzjdzddxe.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hnqzz.top/gtnteaqjyb.html

[K05] 深拷贝对象
来源：http://hz.hywenlv.cn/gtznuhexmv.html

Py:   copy.deepcopy(obj)
来源：http://hz.shangyingyoupin.top/gtchencaew.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hfpthk.cn/gtsszmfmtb.html

JS:   structuredClone(obj)
来源：http://hz.jiagoushi.top/gtykmcfade.html

TS:   structuredClone(obj)
来源：http://hz.vqdsnc.cn/gtkgvfwbvb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.havefunace.top/gtekeouuxe.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shanyushiyangkeji.top/gtvhtcfilt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.svipenyu.cn/gtsbpispxl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hysaishi.cn/gtmzyzzhej.html

[K06] 解析 URL 查询串
来源：http://hz.hywenlv.cn/gtqgwrzwpv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.mhx1999.top/gtrshkdxmu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xingfuxueyuan.xyz/gtqmzsgfed.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhaomingkeji.xyz/gtvlorvyig.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xinyue.icu/gtobupknaa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.316326.xyz/gttdpviziu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zdqjudy.top/gtxtbymgfy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yangfankeji.com/gtbsqbnizr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhaomingkeji.xyz/gtbkwiiazu.html

[K07] 进制转换
来源：http://hz.meibo888.top/gtgkkwsbay.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtpfowzymn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj20258.top/gtcwadvyar.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtmrxlndcu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cqqwz.cn/gthpqxrjsd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.haohaochexian.top/gtnctfxnbd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hysaishi.cn/gtfyrsgini.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xuetiantiany.cn/gtxznlfuhu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hywenlv.cn/gtestoqvqj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shanyushiyangkeji.top/gtklsnrpao.html

Py:   pickle.dumps(obj)
来源：http://hz.shzxlz.cn/gtxlqeysla.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.bjfxy.top/gtzfszzfre.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sxryk.cn/gtejfdfcbx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.316326.xyz/gtkehfbesb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jqgufenzy.top/gtmrhlvumt.html

Go:   encoding/gob
来源：http://hz.xuanzx.com/gtpywxbrqk.html

Ruby: Marshal.dump(obj)
来源：http://hz.tian-w.cn/gteusowxrr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj202588.top/gtokbhggos.html

================================================================================
来源：http://hz.bjfxy.top/gtbxbpoxax.html

L. 网络请求
来源：http://hz.yj202588.top/gtuiqihvam.html

================================================================================
来源：http://hz.sweek.top/gtcdabepmp.html

[L01] 发送 GET 请求
来源：http://hz.smart0.xyz/gtvrnlyagv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hywenlv.cn/gtjklzdhog.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.svipenyu.cn/gtnfdtvmda.html

JS:   await fetch(url)
来源：http://hz.daria6918.cn/gtjsguuppa.html

TS:   await fetch(url)
来源：http://hz.cucudq.cn/gtygngxlhh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yangfankeji.com/gtyukmeqyp.html

Go:   resp, err := http.Get(url)
来源：http://hz.snrcjt.cn/gtcfwgbqya.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhengqikj.top/gtbudrlrpd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hammf.cn/gtqeynfgqa.html

[L02] 发送 POST JSON
来源：http://hz.hammf.cn/gtdhdcslnd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yj202588.top/gtfaaliylr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.0kj1m.cn/gtdyucpnvs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhijiandao.cn/gtrhjadpcz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gogol.net.cn/gtquigzcty.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ydzc1.top/gtgvlbaumb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shzxlz.cn/gtuoralioz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.andypj.xyz/gtagbhcnat.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.316326.xyz/gtkmmhcwxu.html

[L03] 设置自定义请求头
来源：http://hz.zdqjudy.top/gtceirzrhv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.pengpengdd.cyou/gtljmjaxbd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.nanxinkj.top/gtvrolihyn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gaohongyu789.top/gtqioymmfq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.svipenyu.cn/gtkxyqydie.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hysaishi.cn/gtqvdvouto.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yuxming.cn/gtvwlusvjv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhengqikj.top/gtelysnynu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.feifeiyinyue.top/gtmgdgcdch.html

[L04] 设置超时
来源：http://hz.kuanghao11.cn/gtppzpiyip.html

Py:   requests.get(url, timeout=5)
来源：http://hz.52xcode.cn/gtcaqxpmiv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.snrcjt.cn/gtcitsqivk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shangyingyoupin.top/gtmlhkxbsi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuanzhike.top/gtjzgeqdts.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jyoumei.cn/gtxyefcxea.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.aibaodan.cn/gtjfhyvfhp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.nanxuanxn.top/gtsvojfysl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hammf.cn/gtotmyilfd.html

[L05] 上传文件（multipart）
来源：http://hz.tianlin.xyz/gtzupoxhkb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.birdmap.top/gtxgbtedxc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cashguo.top/gtknssbohj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sxryk.cn/gtuzyaubwy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.snrcjt.cn/gtopwlzrfe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.birdmap.top/gtxtftxsmo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.iojbl.cn/gtxsxvlyjn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jqgufenzy.top/gtugqiotlm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhiwuduotai.top/gtsiumjdoz.html

[L06] 解析响应为 JSON
来源：http://hz.zdqjudy.top/gtsmgvcrao.html

Py:   resp.json()
来源：http://hz.yuxming.cn/gtppufqaiy.html

PHP:  json_decode($body, true);
来源：http://hz.wangshuangyany.cn/gtoconlehy.html

JS:   await resp.json()
来源：http://hz.sufxvd.cn/gthicbjfrs.html

TS:   await resp.json()
来源：http://hz.sxryk.cn/gtkuiraumx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jiagoushi.top/gtmuzqwztj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhengqikj.top/gtrohcqwcl.html

Ruby: JSON.parse(resp.body)
来源：http://hz.guowangkeji.top/gtlazhrtal.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.nwbrower.top/gtlheynufp.html

[L07] 处理 HTTP 状态码
来源：http://hz.wangdashe.top/gtrasvflsr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.0kj1m.cn/gtxavdhdrk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sufxvd.cn/gtxzkdflbf.html

JS:   resp.ok;  resp.status
来源：http://hz.jlsjyb.cn/gtbaztjono.html

TS:   resp.ok;  resp.status
来源：http://hz.jqgufenzy.top/gtjkrvfxbm.html

Java: resp.statusCode()
来源：http://hz.shzxlz.cn/gtzwdqoozm.html

Go:   resp.StatusCode
来源：http://hz.chenlongwang.top/gtmzkbstxp.html

Ruby: resp.code.to_i
来源：http://hz.sweek.top/gtufmozsxs.html

C#:   (int)resp.StatusCode
来源：http://hz.jlsjyb.cn/gtdzzkdqdo.html

[L08] 并发请求多个地址
来源：http://hz.shangyingyoupin.top/gtpmpuylbl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhaomingkeji.xyz/gtvwcobfmv.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhengqikj.top/gtticaacgj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtgwwoasof.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ywan-chungtsiang.top/gtbjkscpan.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.quarkkingdee.top/gtdllmdjmc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhixingplan.top/gtosmbkvgm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yonumen.top/gtmijzvgtz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hammf.cn/gtoekwvvbf.html

================================================================================
来源：http://hz.9152youxi.cn/gtzkuztoiu.html

M. 命令行 / 进程 / 环境
来源：http://hz.vqdsnc.cn/gtxhgstxum.html

================================================================================
来源：http://hz.kuanghao11.cn/gtwzcxtzui.html

[M01] 读取命令行参数
来源：http://hz.svipenyu.cn/gtyzjaakvy.html

Py:   sys.argv[1:]
来源：http://hz.yuanzhike.top/gtlgjasbhc.html

PHP:  $argv;  $argc;
来源：http://hz.c1oappe.top/gtnthsuzad.html

JS:   process.argv.slice(2)
来源：http://hz.yj20258.top/gtmwjrqtnv.html

TS:   process.argv.slice(2)
来源：http://hz.pengpengdd.cyou/gtmjpfbyez.html

Java: args 数组（main 方法参数）
来源：http://hz.sweek.top/gtbzhdcbbu.html

Go:   os.Args[1:]
来源：http://hz.ydjk.org.cn/gtmsgkslmc.html

Ruby: ARGV
来源：http://hz.0kj1m.cn/gtogxjbxmj.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinghuilouyu.cn/gtexjohekb.html

[M02] 读取环境变量
来源：http://hz.pengpengdd.cyou/gteupgyhpf.html

Py:   os.environ.get("HOME")
来源：http://hz.ehwqpu.com/gtytvbdqqu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shanyushiyangkeji.top/gtbzufjbdl.html

JS:   process.env.HOME
来源：http://hz.hysaishi.cn/gtzspmfbsb.html

TS:   process.env.HOME
来源：http://hz.jinqigfzy.top/gtufgzlwxr.html

Java: System.getenv("HOME")
来源：http://hz.jinghuilouyu.cn/gthianizkd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ywan-chungtsiang.top/gtvpskzmug.html

Ruby: ENV["HOME"]
来源：http://hz.zhiwuduotai.top/gtyadhjhrv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.meibo888.top/gtrnlxrldz.html

[M03] 执行外部命令
来源：http://hz.shzxlz.cn/gtyovhxlqn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ehwqpu.com/gtjqbmebpy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shanyushiyangkeji.top/gtngolszri.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.nanxuanxn.top/gtmlxaifvq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jiagoushi.top/gtqggkawbm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj20258.top/gtnufeojrn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tianlin.xyz/gtxkogzxhn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhongyouzk.top/gtovpkzpvp.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gotoacloud.top/gtykeeercr.html

[M04] 获取当前工作目录
来源：http://hz.jyoumei.cn/gtrafxswuu.html

Py:   os.getcwd()
来源：http://hz.jinghuilouyu.cn/gtwihvpmax.html

PHP:  getcwd();
来源：http://hz.zhijiandao.cn/gtnpmzqsni.html

JS:   process.cwd()
来源：http://hz.meibo888.top/gtpykgacgv.html

TS:   process.cwd()
来源：http://hz.hysaishi.cn/gtswqwpzir.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ywan-chungtsiang.top/gtotrkuimf.html

Go:   os.Getwd()
来源：http://hz.chenlongwang.top/gtxlfbzepn.html

Ruby: Dir.pwd
来源：http://hz.xziqi.cn/gthehovpoq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ydzc1.top/gthrzzeloz.html

[M05] 设置退出码
来源：http://hz.kuanghao11.cn/gtssxswhmc.html

Py:   sys.exit(1)
来源：http://hz.birdmap.top/gtovnopazd.html

PHP:  exit(1);
来源：http://hz.9152youxi.cn/gtxxfdbbkh.html

JS:   process.exit(1)
来源：http://hz.ivvv.top/gtjsahftbt.html

TS:   process.exit(1)
来源：http://hz.havefunace.top/gtlesvvqjo.html

Java: System.exit(1)
来源：http://hz.hongshengwenyu.top/gtnpijcafl.html

Go:   os.Exit(1)
来源：http://hz.yj202588.top/gtwmxabdiw.html

Ruby: exit 1
来源：http://hz.daria6918.cn/gtosdhuqpn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zycfv.cn/gtngvirvnl.html

[M06] 向标准错误输出
来源：http://hz.dashuyun.cn/gtndnkwosa.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hongshengwenyu.top/gtnfbhslnw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ybcxt.top/gtunylktef.html

JS:   console.error("err")
来源：http://hz.ybcxt.top/gtynyagxge.html

TS:   console.error("err")
来源：http://hz.ybcxt.top/gtantaawtm.html

Java: System.err.println("err")
来源：http://hz.dashuyun.cn/gtbihwdkxb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.0kj1m.cn/gtljwxqgdq.html

Ruby: warn "err"
来源：http://hz.jinqigfzy.top/gttaqezvgt.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shzxlz.cn/gtvpfxqajo.html

[M07] 判断是否为主入口
来源：http://hz.yj20258888.top/gttgxtswut.html

Py:   if __name__ == "__main__":
来源：http://hz.shzxlz.cn/gtxaptmotk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cucudq.cn/gtvoidzqbf.html

JS:   require.main === module
来源：http://hz.zycfv.cn/gtiheswmwp.html

TS:   require.main === module
来源：http://hz.jlsjyb.cn/gtirzykfwa.html

Java: public static void main(String[] args)
来源：http://hz.316326.xyz/gtwarojmzz.html

Go:   func main()
来源：http://hz.jqgfzy.top/gtegexljbd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yongpay.top/gtcjrocxhq.html

C#:   static void Main(string[] args)
来源：http://hz.hysaishi.cn/gtyzdithzd.html

[M08] 获取系统与运行时信息
来源：http://hz.sysykeji.top/gtzschacwj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ppjwa.cn/gtzmqbcvsp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.redwolf501.top/gtjzrcbmdz.html

JS:   process.platform;  process.version
来源：http://hz.xylfe.cn/gthxvnitrs.html

TS:   process.platform;  process.version
来源：http://hz.gzhubu.top/gtbkiyznqz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xinyue.icu/gtorrlnvxn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hfpthk.cn/gtbbfultfe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yj202588.top/gtvtvrsawm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.fengsongda.top/gtjblcxntt.html

================================================================================
来源：http://hz.hfpthk.cn/gtftxtovrk.html

N. 数据结构与算法
来源：http://hz.gzhubu.top/gtdvogeheo.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtxfuldkgv.html

[N01] 二分查找（有序数组）
来源：http://hz.jyoumei.cn/gtiiwjjwmz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhoulong.xyz/gtnhtktezz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.meibo888.top/gtuqyftalq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.vqdsnc.cn/gtfdrvdigw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydjk.org.cn/gtlvyrjjti.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shuidangran.top/gtnuuirina.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtgauyhrhq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.wangdashe.top/gtwcapuubj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.fzhhl.top/gtmqyxyley.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yj20258.top/gtepsdbvxh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pengpengdd.cyou/gtkylmryyy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.quarkkingdee.top/gtvfmicybw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yongpay.top/gtxkoerlvb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gtsgmqkqpz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.gogol.net.cn/gtkssfuuwk.html

Go:   slices.Sort(arr)
来源：http://hz.dianchejie.cn/gtjylbblmy.html

Ruby: arr.sort
来源：http://hz.zhixingplan.top/gtheqjuatt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhoulong.xyz/gtydrtoyxv.html

[N03] 快速排序（分治示例）
来源：http://hz.jinqigufen.top/gthyzglzyr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.mhx1999.top/gtbaebzqup.html

PHP:  // 递归实现，或用 usort
来源：http://hz.mhx1999.top/gtpzlzdzfp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinyuanbaomall.cn/gtlphxenco.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.snrcjt.cn/gtdsgynvxs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cdnleiting.top/gtznijbxda.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.kuanghao11.cn/gtbqbplyiw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sxryk.cn/gtbumbjvfv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.snrcjt.cn/gtfjgrewkb.html

[N04] 斐波那契数列
来源：http://hz.yongpay.top/gtgkcvsofn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cashguo.top/gtryrjtjrl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hysaishi.cn/gtajlamvif.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhixingplan.top/gtutiohdjh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ydzc1.top/gtebenngaq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.daria6918.cn/gtjnlyiozr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xziqi.cn/gtannzrdzi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.fengsongda.top/gtokchstks.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj20258888.top/gtcxkgavne.html

[N05] 最大公约数
来源：http://hz.ivvv.top/gtjnwtogqg.html

Py:   math.gcd(a, b)
来源：http://hz.zhijiandao.cn/gtgnrduqas.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.dianchejie.cn/gtjrpmugqi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gogol.net.cn/gtbfyggxbl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gogol.net.cn/gtrjprlxpb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sxryk.cn/gtdqeezmsa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hnqzz.top/gtynfwnylu.html

Ruby: a.gcd(b)
来源：http://hz.xziqi.cn/gtreqdfuhx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yuxming.cn/gtzlligkwz.html

[N06] 判断回文字符串
来源：http://hz.0kj1m.cn/gtirwyvdwa.html

Py:   s == s[::-1]
来源：http://hz.chenzaomai.com/gtlgypzavk.html

PHP:  $s === strrev($s);
来源：http://hz.iojbl.cn/gtobyouoig.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtryctsxiz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtgcbenplq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinghuilouyu.cn/gtiezqywly.html

Go:   // 双指针从两端比较
来源：http://hz.jinqigfzy.top/gtwfoifmfo.html

Ruby: s == s.reverse
来源：http://hz.quarkkingdee.top/gtncqichmz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cashguo.top/gtrxaikqtq.html

[N07] 两数之和（返回下标）
来源：http://hz.chenlongwang.top/gtuweooeid.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gogol.net.cn/gtpqgvwssw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hammf.cn/gtezugpnvo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jiagoushi.top/gtnmhjqwvu.html

TS:   // 手写 Map<string, number>
来源：http://hz.dashuyun.cn/gtjhqlqhei.html

Java: // 手写 HashMap
来源：http://hz.aibaodan.cn/gtjdxqkqyf.html

Go:   // 手写 map[int]int
来源：http://hz.pycfn.com/gtircfxzug.html

Ruby: // 手写 Hash
来源：http://hz.zhongyouzk.top/gtismwtxae.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.tianlin.xyz/gtjohcbmsp.html

[N08] 生成全排列
来源：http://hz.ivvv.top/gtceifvodp.html

Py:   itertools.permutations(arr)
来源：http://hz.xuetiantiany.cn/gtboqnketo.html

PHP:  // 手写递归交换
来源：http://hz.aibaodan.cn/gtemlkirjl.html

JS:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtoxnermax.html

TS:   // 手写回溯递归
来源：http://hz.zycfv.cn/gtjymtnsbo.html

Java: // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtibrhzlhy.html

Go:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtjuqdzhkt.html

Ruby: arr.permutation.to_a
来源：http://hz.hnxiangtu.top/gtnszmdndl.html

C#:   // 手写回溯递归
来源：http://hz.jqgufenzy.top/gtngbuuhpz.html

[N09] 栈与队列
来源：http://hz.daria6918.cn/gtpgvbihbx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.cucudq.cn/gtzzodowls.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.c1oappe.top/gtbzopxvbo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.shanyushiyangtech.top/gtrfjiwtwh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinyuanbaomall.cn/gtewrzllrn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.52xcode.cn/gtwkqgzqhk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hammf.cn/gtzvhydxtk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xuanzx.com/gtbehfeaie.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yangfankeji.com/gtdjzwgkjy.html

[N10] 链表节点定义
来源：http://hz.gaohongyu789.top/gtnwlktkws.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shanyushiyangkeji.top/gtuddwdxzk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.haohaochexian.top/gtcutasyfk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhiwuduotai.top/gteddujsbn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ivvv.top/gtkepeuzsb.html

Java: class Node { int v; Node next; }
来源：http://hz.jinqigfzy.top/gtyqvchxxr.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gotoacloud.top/gttjtvzlqy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.gzhubu.top/gtdjjbbuqa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhixingplan.top/gtpcdnrswu.html

[N11] 二叉树中序遍历
来源：http://hz.52xcode.cn/gthftaakrn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jqgfzy.top/gttiavsdvd.html

PHP:  // 手写递归函数
来源：http://hz.ehwqpu.com/gtgildjxxe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pengpengdd.cyou/gtfrpgyqrs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hammf.cn/gtdzuqujhu.html

Java: // 手写递归
来源：http://hz.xziqi.cn/gthcuhghyu.html

Go:   // 手写递归
来源：http://hz.yanxiufei.cn/gtzhryzrzw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.gotoacloud.top/gtyvmhvkiw.html

C#:   // 手写递归
来源：http://hz.jinqigfzy.top/gtpielnlvx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.daxiang520.top/gtmubkmyli.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yueranfly.top/gtpamvcgco.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhiwuduotai.top/gtljfzilye.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.svipenyu.cn/gtlajfxsgo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhiwuduotai.top/gtryqnrpca.html


<!-- 参考信息 -->