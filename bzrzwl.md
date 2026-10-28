代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gogol.net.cn/gttadzuqfb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tianlin.xyz/gtrnrrslbp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.aizwys.cn/gtumkjhsqz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sweek.top/gtkyqxnmfj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jlsjyb.cn/gtxlxkvkcp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.9152youxi.cn/gtxvkvehcd.html

[K04] 读取 JSON 文件
来源：http://hz.shzxlz.cn/gtwwvjwvoh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.52xcode.cn/gtsylgwrbn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ivvv.top/gtcpytbohr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinghuilouyu.cn/gtwmlqmetz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.meibo888.top/gtvjgssrkt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.9152youxi.cn/gtbqxfieez.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zycfv.cn/gttsaulbwq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhoulong.xyz/gtdfibmihs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.iojbl.cn/gtvyepjmyt.html

[K05] 深拷贝对象
来源：http://hz.zhoulong.xyz/gtsxfrgwdu.html

Py:   copy.deepcopy(obj)
来源：http://hz.yonumen.top/gtotoyaxyk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ppjwa.cn/gtvnxehhnz.html

JS:   structuredClone(obj)
来源：http://hz.yj20258888.top/gtfpxyfond.html

TS:   structuredClone(obj)
来源：http://hz.hnqzz.top/gtpuekghhv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yueranfly.top/gtinnbgbhc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.tian-w.cn/gtmmwsexfr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.snrcjt.cn/gtffhhgfbj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinyuanbaomall.cn/gtsallqhcs.html

[K06] 解析 URL 查询串
来源：http://hz.sufxvd.cn/gtawukgzjx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sufxvd.cn/gtqzjiilau.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yuxming.cn/gtfqmbgrbd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinyuanbaomall.cn/gtukwmjedg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangshuangyany.cn/gtuybadtxx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.birdmap.top/gtrzsmlodl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinqigufen.top/gtsohwwrbl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zdqjudy.top/gtgqdihoro.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ywan-chungtsiang.top/gtpwvrbohx.html

[K07] 进制转换
来源：http://hz.iojbl.cn/gtsuuruhaz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.aizwys.cn/gtajannaro.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.kuanghao11.cn/gtqgoytuci.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sweek.top/gtziynckts.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zdqjudy.top/gtmdcynasw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.wangdashe.top/gthpmuyazj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.fengsongda.top/gtkzuwvjrn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.wangshuangyany.cn/gtbahcjyxp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sxryk.cn/gtdnltmzrs.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.chenlongwang.top/gtoztisfdc.html

Py:   pickle.dumps(obj)
来源：http://hz.hongshengwenyu.top/gtskhjtszk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.andypj.xyz/gtcjpizaug.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.pycfn.com/gtnqufasnw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhixingplan.top/gtvfdtgjix.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenjidiqi.icu/gtxtmrvbcg.html

Go:   encoding/gob
来源：http://hz.sysykeji.top/gtmiajipfk.html

Ruby: Marshal.dump(obj)
来源：http://hz.hnxiangtu.top/gtflrlsspx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ydjk.org.cn/gtupqttzmw.html

================================================================================
来源：http://hz.jyoumei.cn/gtialwnykr.html

L. 网络请求
来源：http://hz.haohaochexian.top/gtypjvmcrc.html

================================================================================
来源：http://hz.vqdsnc.cn/gtxzdcucfj.html

[L01] 发送 GET 请求
来源：http://hz.ivvv.top/gtytnokowj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hywenlv.cn/gtkrbqsfqf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cdnleiting.top/gtjmutotvw.html

JS:   await fetch(url)
来源：http://hz.hongshengwenyu.top/gtiwnchtpx.html

TS:   await fetch(url)
来源：http://hz.chenjidiqi.icu/gtucscbilm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xziqi.cn/gtkyvmrzvg.html

Go:   resp, err := http.Get(url)
来源：http://hz.hywenlv.cn/gtarjszaun.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.andypj.xyz/gtcgzefzle.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jlsjyb.cn/gtycdjiakm.html

[L02] 发送 POST JSON
来源：http://hz.tian-w.cn/gtvaiwvpoe.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ppjwa.cn/gtnqqywgqw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.shuidangran.top/gtqwxssuuk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gaohongyu789.top/gtqghvmyuv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ivvv.top/gtwadokmal.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.guowangkeji.top/gtilxhlhrb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hongshengwenyu.top/gteqlkjoir.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yanxiufei.cn/gtsxhwgnnt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xuanzx.com/gtcxlwoopk.html

[L03] 设置自定义请求头
来源：http://hz.feifeiyinyue.top/gtssvyqjrt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cashguo.top/gtgqmqrbdm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.tianlin.xyz/gtbpsjvdpw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuxming.cn/gtelelkzot.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guowangkeji.top/gtuotmczmg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.vqdsnc.cn/gtepzcopca.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.havefunace.top/gtcwunbira.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.0kj1m.cn/gtpvzvocmz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhoulong.xyz/gtvgrlzyca.html

[L04] 设置超时
来源：http://hz.cucudq.cn/gtxcrpnjwk.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jinghuilouyu.cn/gtvrvjgajk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.pengpengdd.cyou/gtftkjlwjs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gotoacloud.top/gteesbajim.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aizwys.cn/gtaluskdwj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.meibo888.top/gtflwizpph.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ydzc1.top/gtsxvlzthw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jlsjyb.cn/gtiysluwco.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cdnleiting.top/gtgjwevvih.html

[L05] 上传文件（multipart）
来源：http://hz.shzxlz.cn/gtwbpgigrz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinqigufen.top/gtwhryzfda.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.andypj.xyz/gtctfotffn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cqqwz.cn/gtfyaadlrh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yonumen.top/gtzvarnmif.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.nanxuanxn.top/gtywwyqsnn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.pengpengdd.cyou/gtrljdbsan.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.redwolf501.top/gtvvzuqiqx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hfpthk.cn/gtdzlrccyu.html

[L06] 解析响应为 JSON
来源：http://hz.jinyuanbaomall.cn/gtaesyquee.html

Py:   resp.json()
来源：http://hz.jianghu66.top/gtkmsvircu.html

PHP:  json_decode($body, true);
来源：http://hz.jlsjyb.cn/gtwgvowhpi.html

JS:   await resp.json()
来源：http://hz.shzxlz.cn/gtxgqxxhtr.html

TS:   await resp.json()
来源：http://hz.cdnleiting.top/gtsrtzvmca.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gogol.net.cn/gtpgristmn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gzhubu.top/gtcmaosnil.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xingfuxueyuan.xyz/gtpbsojhbk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ydzc1.top/gtaefqgefs.html

[L07] 处理 HTTP 状态码
来源：http://hz.xuetiantiany.cn/gtyrliypge.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yj20258888.top/gtjijlqxfi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cqqwz.cn/gtptmmuvsx.html

JS:   resp.ok;  resp.status
来源：http://hz.jinghuilouyu.cn/gtwrcraovb.html

TS:   resp.ok;  resp.status
来源：http://hz.0kj1m.cn/gtfpqkfcne.html

Java: resp.statusCode()
来源：http://hz.zhongyouzk.top/gtlxzuvlic.html

Go:   resp.StatusCode
来源：http://hz.ydjk.org.cn/gtplhviakb.html

Ruby: resp.code.to_i
来源：http://hz.tian-w.cn/gtqqgdakoc.html

C#:   (int)resp.StatusCode
来源：http://hz.havefunace.top/gtcrmpbzpl.html

[L08] 并发请求多个地址
来源：http://hz.xuanzx.com/gtqshlcptl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gaohongyu789.top/gtntvqybsf.html

PHP:  curl_multi_init() 系列
来源：http://hz.yongpay.top/gtnnyjomli.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hysaishi.cn/gtjozxqmcd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xylfe.cn/gtbtjassrm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hysaishi.cn/gtzbvscpyp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinghuilouyu.cn/gtgsotdspb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhongyouzk.top/gthghrcjwk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinghuilouyu.cn/gtsqimihzj.html

================================================================================
来源：http://hz.yj202588.top/gtxghzqljc.html

M. 命令行 / 进程 / 环境
来源：http://hz.tian-w.cn/gtuznvlbnk.html

================================================================================
来源：http://hz.shuidangran.top/gtlrgbqwux.html

[M01] 读取命令行参数
来源：http://hz.jianghu66.top/gtvsfigfiu.html

Py:   sys.argv[1:]
来源：http://hz.guowangkeji.top/gtxkvkgxwb.html

PHP:  $argv;  $argc;
来源：http://hz.aizwys.cn/gthuqswiyp.html

JS:   process.argv.slice(2)
来源：http://hz.gotoacloud.top/gtzxekbvdf.html

TS:   process.argv.slice(2)
来源：http://hz.snrcjt.cn/gtlzdvghwd.html

Java: args 数组（main 方法参数）
来源：http://hz.shangyingyoupin.top/gtzdnucnyc.html

Go:   os.Args[1:]
来源：http://hz.jiagoushi.top/gtzimzmltw.html

Ruby: ARGV
来源：http://hz.zhengqikj.top/gtsfzjkvgi.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ydzc1.top/gtiwudtscz.html

[M02] 读取环境变量
来源：http://hz.kuanghao11.cn/gtyrtyszog.html

Py:   os.environ.get("HOME")
来源：http://hz.sxryk.cn/gtnqjeoihj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.dashuyun.cn/gtseztmaol.html

JS:   process.env.HOME
来源：http://hz.nanxinkj.top/gtwlcpxsxr.html

TS:   process.env.HOME
来源：http://hz.tianlin.xyz/gtivnoxahj.html

Java: System.getenv("HOME")
来源：http://hz.hnxiangtu.top/gtbpmidwch.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.kuanghao11.cn/gtkrrnvsmz.html

Ruby: ENV["HOME"]
来源：http://hz.xinyue.icu/gtdnhshwfe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shzxlz.cn/gtkzjhbhqt.html

[M03] 执行外部命令
来源：http://hz.ywan-chungtsiang.top/gtzoqxothz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.daxiang520.top/gtuxxucfal.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.daxiang520.top/gttbwcrdwx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj202588.top/gticpgdrlc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.sweek.top/gtuebythil.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hysaishi.cn/gtytshuupd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xuanzx.com/gtaxlcolnv.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.chenlongwang.top/gtawzrufnf.html

C#:   Process.Start("ls", "-l");
来源：http://hz.chenzaomai.com/gtufgotvzh.html

[M04] 获取当前工作目录
来源：http://hz.quarkkingdee.top/gtnwnjjwsv.html

Py:   os.getcwd()
来源：http://hz.yangfankeji.com/gttwmnsevl.html

PHP:  getcwd();
来源：http://hz.jqgufenzy.top/gtuxbqchit.html

JS:   process.cwd()
来源：http://hz.tianlin.xyz/gtftxoogbh.html

TS:   process.cwd()
来源：http://hz.dianchejie.cn/gtyzlpfikt.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yuxming.cn/gtbweoewvq.html

Go:   os.Getwd()
来源：http://hz.hywenlv.cn/gtccojnetk.html

Ruby: Dir.pwd
来源：http://hz.wangshuangyany.cn/gtxdzxgira.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jqgfzy.top/gtpgfmjzxm.html

[M05] 设置退出码
来源：http://hz.zhiwuduotai.top/gtprprqmjm.html

Py:   sys.exit(1)
来源：http://hz.jyoumei.cn/gtswefdyza.html

PHP:  exit(1);
来源：http://hz.yongpay.top/gtdkclgiwf.html

JS:   process.exit(1)
来源：http://hz.0kj1m.cn/gtowqibxwv.html

TS:   process.exit(1)
来源：http://hz.mhx1999.top/gtyiebxfbx.html

Java: System.exit(1)
来源：http://hz.quarkkingdee.top/gtazlrgtno.html

Go:   os.Exit(1)
来源：http://hz.iojbl.cn/gtqvkbqttj.html

Ruby: exit 1
来源：http://hz.tian-w.cn/gttmjalmha.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jyoumei.cn/gtlkpfvjug.html

[M06] 向标准错误输出
来源：http://hz.xuetiantiany.cn/gtjjuzeemr.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jiagoushi.top/gtznfbdmbu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.nwbrower.top/gtfvcwseko.html

JS:   console.error("err")
来源：http://hz.tian-w.cn/gtypilubxl.html

TS:   console.error("err")
来源：http://hz.redwolf501.top/gtuvkvvkea.html

Java: System.err.println("err")
来源：http://hz.yj202588.top/gtbhkiumhx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.pengpengdd.cyou/gtnblpawtz.html

Ruby: warn "err"
来源：http://hz.shzxlz.cn/gtyizmfvrb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hnqzz.top/gtarthcxtg.html

[M07] 判断是否为主入口
来源：http://hz.guannengcc.top/gtwwrohcss.html

Py:   if __name__ == "__main__":
来源：http://hz.svipenyu.cn/gtaipozots.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xinyue.icu/gtngzvhxsf.html

JS:   require.main === module
来源：http://hz.nanxinkj.top/gtcvudhwvu.html

TS:   require.main === module
来源：http://hz.sweek.top/gtjuiekqhf.html

Java: public static void main(String[] args)
来源：http://hz.nwbrower.top/gtkccojxhx.html

Go:   func main()
来源：http://hz.redwolf501.top/gtztczfein.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinqigfzy.top/gtqnshsznw.html

C#:   static void Main(string[] args)
来源：http://hz.cqqwz.cn/gtznnqgncd.html

[M08] 获取系统与运行时信息
来源：http://hz.daria6918.cn/gttgafmkus.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hongshengwenyu.top/gttawrbxpv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhoulong.xyz/gtvzxzbkhg.html

JS:   process.platform;  process.version
来源：http://hz.hysaishi.cn/gtzuedmegd.html

TS:   process.platform;  process.version
来源：http://hz.zhongyouzk.top/gtjeoxshan.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xylfe.cn/gtzghzywgw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sxryk.cn/gttxbqlodg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.tanke756.top/gtzfosluyf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.nwbrower.top/gthidirqtj.html

================================================================================
来源：http://hz.jqgufenzy.top/gtexakmtfd.html

N. 数据结构与算法
来源：http://hz.shzxlz.cn/gtaqxdnkmq.html

================================================================================
来源：http://hz.guowangkeji.top/gtlfwhvbca.html

[N01] 二分查找（有序数组）
来源：http://hz.cashguo.top/gttjnqrebm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhongyouzk.top/gtvawdrxnv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ivvv.top/gtcaqccpwm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gaohongyu789.top/gtqcazhhxv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxinkj.top/gtggoqlfsv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.nanxuanxn.top/gtgpqmmmaa.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ehwqpu.com/gttkcoozjy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.daxiang520.top/gtsdgchpbr.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.iojbl.cn/gttygryxpw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.iojbl.cn/gtdhmqbljb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigufen.top/gtscpdifce.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yuxming.cn/gtaiolgkos.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.snrcjt.cn/gteklxpseu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cheryme.top/gtkzjrwtdo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yanxiufei.cn/gtbvhnsxut.html

Go:   slices.Sort(arr)
来源：http://hz.gotoacloud.top/gthqwlixxt.html

Ruby: arr.sort
来源：http://hz.jqgfzy.top/gtdwaxkjvc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jqgufenzy.top/gtlykhlgwk.html

[N03] 快速排序（分治示例）
来源：http://hz.zhixingplan.top/gtqyqiuocy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.chenlongwang.top/gtqmjjhhny.html

PHP:  // 递归实现，或用 usort
来源：http://hz.dianchejie.cn/gtjvmmqfik.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydjk.org.cn/gtoyjmbyip.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.quarkkingdee.top/gtgonvlhxl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.nanxinkj.top/gtsropwiln.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xylfe.cn/gtvstxetbk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.316326.xyz/gtrjsukfmo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jqgfzy.top/gtqxmmqjye.html

[N04] 斐波那契数列
来源：http://hz.xziqi.cn/gtwklgugbj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ydjk.org.cn/gtetcvhkgc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.52xcode.cn/gtjexvsqdg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sysykeji.top/gtkdwyswlf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jianghu66.top/gtsujcyset.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.meibo888.top/gtrvzadoxh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.tanke756.top/gtpugefspb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.9152youxi.cn/gtzvzzmpos.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xylfe.cn/gtocoieeea.html

[N05] 最大公约数
来源：http://hz.zhongyouzk.top/gtjuterfge.html

Py:   math.gcd(a, b)
来源：http://hz.shuidangran.top/gtrtzrhwlu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.redwolf501.top/gtejdmdoej.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gotoacloud.top/gtiuagfgiy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.snrcjt.cn/gtoojgwoab.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenlongwang.top/gttqjrntsb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shanyushiyangtech.top/gtajxtlkea.html

Ruby: a.gcd(b)
来源：http://hz.316326.xyz/gtsvwprwai.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.andypj.xyz/gtszsztwtq.html

[N06] 判断回文字符串
来源：http://hz.zhixingplan.top/gtzqwjggkl.html

Py:   s == s[::-1]
来源：http://hz.daxiang520.top/gtiyrrbgve.html

PHP:  $s === strrev($s);
来源：http://hz.birdmap.top/gtafpbgorb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.wangshuangyany.cn/gtxmnhpkxq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yvedp.cn/gtsaijiopp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.nanxinkj.top/gtdqhchatw.html

Go:   // 双指针从两端比较
来源：http://hz.hammf.cn/gtzuuatctz.html

Ruby: s == s.reverse
来源：http://hz.shuidangran.top/gtfuppmbuy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.52xcode.cn/gtecqrpbtw.html

[N07] 两数之和（返回下标）
来源：http://hz.wangdashe.top/gtmogyptqq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jqgfzy.top/gtnxaksubl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cucudq.cn/gtwoethlyh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.vqdsnc.cn/gtachazhog.html

TS:   // 手写 Map<string, number>
来源：http://hz.shanyushiyangtech.top/gttzjlmlik.html

Java: // 手写 HashMap
来源：http://hz.guowangkeji.top/gtyorlqleb.html

Go:   // 手写 map[int]int
来源：http://hz.daria6918.cn/gtaxkqyfqw.html

Ruby: // 手写 Hash
来源：http://hz.nanxinkj.top/gthxlrwgzz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xinyue.icu/gtrlvxmysc.html

[N08] 生成全排列
来源：http://hz.yonumen.top/gtssokuhzq.html

Py:   itertools.permutations(arr)
来源：http://hz.nanxuanxn.top/gttcxjupvm.html

PHP:  // 手写递归交换
来源：http://hz.zycfv.cn/gtmpcsphic.html

JS:   // 手写回溯递归
来源：http://hz.sysykeji.top/gtnkqvjyxy.html

TS:   // 手写回溯递归
来源：http://hz.yuanzhike.top/gtoiimbuvn.html

Java: // 手写回溯递归
来源：http://hz.aizwys.cn/gtrvdqsbnj.html

Go:   // 手写回溯递归
来源：http://hz.xziqi.cn/gtfuoujjqu.html

Ruby: arr.permutation.to_a
来源：http://hz.havefunace.top/gtjdhwellw.html

C#:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gthdibnise.html

[N09] 栈与队列
来源：http://hz.shanyushiyangtech.top/gtqeufygzu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.tanke756.top/gtgzkwkcpg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.feifeiyinyue.top/gtnnxlohax.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.smart0.xyz/gtspuostbk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cdnleiting.top/gtjazxsssk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xingfuxueyuan.xyz/gtvsjlhiem.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ybcxt.top/gticclcxde.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.wangshuangyany.cn/gtdvfoycip.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ivvv.top/gtepawihlj.html

[N10] 链表节点定义
来源：http://hz.daxiang520.top/gtxqdbuyaj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.0kj1m.cn/gtysttmzzo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.daxiang520.top/gtovhuiuah.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.shanyushiyangkeji.top/gtsainnbey.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yongpay.top/gtttoegomb.html

Java: class Node { int v; Node next; }
来源：http://hz.cdnleiting.top/gtukjvajtu.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.birdmap.top/gtffgnfcyg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.nwbrower.top/gtzrxzszhw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ywan-chungtsiang.top/gtlwylemzg.html

[N11] 二叉树中序遍历
来源：http://hz.ydjk.org.cn/gtxttgiitk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xuanzx.com/gttwrwhumb.html

PHP:  // 手写递归函数
来源：http://hz.dashuyun.cn/gtbuhjtzjn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxuanxn.top/gtvdxffart.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.0kj1m.cn/gtjlntifrx.html

Java: // 手写递归
来源：http://hz.shuidangran.top/gthodkebsa.html


<!-- 参考信息 -->