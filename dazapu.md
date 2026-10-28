代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.birdmap.top/gtqpljybbu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sxryk.cn/gttyuzrqah.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.vqdsnc.cn/gtezgyptuf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cdnleiting.top/gtaoadhzrt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangshuangyany.cn/gthogxvhji.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigufen.top/gtmzpwziyr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yonumen.top/gtztbftsig.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.smart0.xyz/gtjhvpyile.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.guowangkeji.top/gtgoypinmz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.bjfxy.top/gttruxdvuy.html

[K04] 读取 JSON 文件
来源：http://hz.shanyushiyangtech.top/gtzlbntfwp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.feifeiyinyue.top/gtfisunzfk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.aibaodan.cn/gtqclyqdga.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yuanzhike.top/gtzfbcmhpg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guowangkeji.top/gtpqqrrmyl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ppjwa.cn/gtwndlkrbo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinyuanbaomall.cn/gtufeqhzwr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jqgufenzy.top/gtgaxgfmrh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jiagoushi.top/gtwyqpqbcs.html

[K05] 深拷贝对象
来源：http://hz.dashuyun.cn/gtdjfwaxlh.html

Py:   copy.deepcopy(obj)
来源：http://hz.ehwqpu.com/gthzgasquz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinqigfzy.top/gtlbcbbwte.html

JS:   structuredClone(obj)
来源：http://hz.jinqigufen.top/gtknjtvnmd.html

TS:   structuredClone(obj)
来源：http://hz.shuidangran.top/gtmuqblycb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ywan-chungtsiang.top/gtdujmregm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.dashuyun.cn/gtcpxkgkxg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cheryme.top/gtbtycxonr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gaohongyu789.top/gtrvqehckd.html

[K06] 解析 URL 查询串
来源：http://hz.quarkkingdee.top/gtkwjkqcrv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xuanzx.com/gteehhsgeh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.havefunace.top/gtiqysfbpe.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zycfv.cn/gtyhzlnqas.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jiagoushi.top/gttomqzarp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.tanke756.top/gtwhiwsuww.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jlsjyb.cn/gtjrdczaye.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yj202588.top/gtumtanmwl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ppjwa.cn/gtikuxwxyk.html

[K07] 进制转换
来源：http://hz.pengpengdd.cyou/gtpkyhmvaj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.daxiang520.top/gtaondtgld.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xinyue.icu/gtximcynhi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gtkihpkuil.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenjidiqi.icu/gtrwiilvcg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hnqzz.top/gtmhtphsdr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yuxming.cn/gtsfejigri.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yonumen.top/gtifmeqbxz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.c1oappe.top/gtetmkvlxy.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hongshengwenyu.top/gtmasgwizn.html

Py:   pickle.dumps(obj)
来源：http://hz.hnqzz.top/gtgvdtnkda.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xuetiantiany.cn/gtovgrbfde.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.daxiang520.top/gtewmhrjuc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.meibo888.top/gtqqavanzy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xinyue.icu/gttnvtcqwz.html

Go:   encoding/gob
来源：http://hz.cucudq.cn/gtraiijxos.html

Ruby: Marshal.dump(obj)
来源：http://hz.shuidangran.top/gtxxudwdxf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xinyue.icu/gtclxkcnly.html

================================================================================
来源：http://hz.guannengcc.top/gtuaddpmot.html

L. 网络请求
来源：http://hz.chenlongwang.top/gtjgmaxkrr.html

================================================================================
来源：http://hz.tian-w.cn/gtxipqdloz.html

[L01] 发送 GET 请求
来源：http://hz.sxryk.cn/gthikqzzie.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.wangshuangyany.cn/gteaykauqe.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.guowangkeji.top/gtyhvasokv.html

JS:   await fetch(url)
来源：http://hz.xuetiantiany.cn/gtddzjiatw.html

TS:   await fetch(url)
来源：http://hz.hfpthk.cn/gtzwhusrsv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xuanzx.com/gtuzwqpruj.html

Go:   resp, err := http.Get(url)
来源：http://hz.jianghu66.top/gtepgpnerq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.tian-w.cn/gtnvagcftj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.c1oappe.top/gtpuanytpb.html

[L02] 发送 POST JSON
来源：http://hz.jinyuanbaomall.cn/gtzsbstchl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.daria6918.cn/gtvzxumpba.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.redwolf501.top/gtqkikftyp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ydjk.org.cn/gtzqwwtfbo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hfpthk.cn/gturgfaosi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.feifeiyinyue.top/gtfqsvfcla.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nanxinkj.top/gtmpgykaaj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yongpay.top/gtvqfmgnwv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.kuanghao11.cn/gtvmksbhde.html

[L03] 设置自定义请求头
来源：http://hz.jinqigufen.top/gtwbbjihvz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.pengpengdd.cyou/gtltwgpfgd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jiagoushi.top/gtdsdfpuqm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenlongwang.top/gtainucocm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.svipenyu.cn/gtawvzbrbt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.wangdashe.top/gteshygovw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.wangshuangyany.cn/gtavkuwimy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cdnleiting.top/gtmuplkioc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.tianlin.xyz/gtndpbgsxu.html

[L04] 设置超时
来源：http://hz.yongpay.top/gtdoektlze.html

Py:   requests.get(url, timeout=5)
来源：http://hz.daria6918.cn/gtemreeifm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.meibo888.top/gtapzqvdpa.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hywenlv.cn/gtmestbgba.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fengsongda.top/gtcbbzvqdb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cheryme.top/gtmndzomhg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cheryme.top/gtjooxjhbt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cdnleiting.top/gtsozpmcdw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.smart0.xyz/gtugxfdhkp.html

[L05] 上传文件（multipart）
来源：http://hz.ydzc1.top/gtaawlgfxj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xuetiantiany.cn/gtapokgffl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.sxryk.cn/gtinthahax.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.havefunace.top/gtxsljiurd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxinkj.top/gtcbfsauqj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.daria6918.cn/gtyfmugpkp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shanyushiyangtech.top/gtngenhbxn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.snrcjt.cn/gtoyrgejav.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xuanzx.com/gtaceozaqk.html

[L06] 解析响应为 JSON
来源：http://hz.yj202588.top/gtiolqgxns.html

Py:   resp.json()
来源：http://hz.jqgufenzy.top/gtegehlmgi.html

PHP:  json_decode($body, true);
来源：http://hz.yonumen.top/gtixqtidnc.html

JS:   await resp.json()
来源：http://hz.zhijiandao.cn/gtadfnwyow.html

TS:   await resp.json()
来源：http://hz.daria6918.cn/gtbzeufjai.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cdnleiting.top/gtoxauluqa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jlsjyb.cn/gtrefidait.html

Ruby: JSON.parse(resp.body)
来源：http://hz.andypj.xyz/gtenofumbw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.guannengcc.top/gthfkwnszx.html

[L07] 处理 HTTP 状态码
来源：http://hz.hysaishi.cn/gtzxwtjltw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zycfv.cn/gtzlyyfbyu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hfpthk.cn/gtrauhkjaj.html

JS:   resp.ok;  resp.status
来源：http://hz.sufxvd.cn/gthvsmsklb.html

TS:   resp.ok;  resp.status
来源：http://hz.wangdashe.top/gtfbokbzmt.html

Java: resp.statusCode()
来源：http://hz.0kj1m.cn/gtskhunizf.html

Go:   resp.StatusCode
来源：http://hz.jqgufenzy.top/gtfouebjtb.html

Ruby: resp.code.to_i
来源：http://hz.52xcode.cn/gtenasncbv.html

C#:   (int)resp.StatusCode
来源：http://hz.redwolf501.top/gtfxlvptts.html

[L08] 并发请求多个地址
来源：http://hz.cqqwz.cn/gtszmvgwly.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.c1oappe.top/gtqmcnlnlg.html

PHP:  curl_multi_init() 系列
来源：http://hz.aizwys.cn/gtstnihwie.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangdashe.top/gthpxufnxk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hnxiangtu.top/gtikvwbfbu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.chenlongwang.top/gtvbngxgpa.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhixingplan.top/gtvzzulgni.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xylfe.cn/gtozxsdxon.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yj20258888.top/gtferwwgio.html

================================================================================
来源：http://hz.ivvv.top/gtqtuqutkw.html

M. 命令行 / 进程 / 环境
来源：http://hz.xinyue.icu/gtlhfrmnjm.html

================================================================================
来源：http://hz.nanxuanxn.top/gtueahlppq.html

[M01] 读取命令行参数
来源：http://hz.chenjidiqi.icu/gttdgdndcg.html

Py:   sys.argv[1:]
来源：http://hz.gzhubu.top/gtrfnjjzgh.html

PHP:  $argv;  $argc;
来源：http://hz.gaohongyu789.top/gtnlmqvknv.html

JS:   process.argv.slice(2)
来源：http://hz.0kj1m.cn/gtvwxdukqz.html

TS:   process.argv.slice(2)
来源：http://hz.hfpthk.cn/gtyqnbttyz.html

Java: args 数组（main 方法参数）
来源：http://hz.nanxinkj.top/gtfvlodmsf.html

Go:   os.Args[1:]
来源：http://hz.cdnleiting.top/gtjxdloyfz.html

Ruby: ARGV
来源：http://hz.chenlongwang.top/gtpunhmmik.html

C#:   args 数组（Main 方法参数）
来源：http://hz.birdmap.top/gtpnkfjdhj.html

[M02] 读取环境变量
来源：http://hz.cheryme.top/gtugsadgdq.html

Py:   os.environ.get("HOME")
来源：http://hz.yueranfly.top/gtdfvnkkow.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hnqzz.top/gtwckskeja.html

JS:   process.env.HOME
来源：http://hz.jinghuilouyu.cn/gtvvknrgtk.html

TS:   process.env.HOME
来源：http://hz.yuanzhike.top/gtejugdbtk.html

Java: System.getenv("HOME")
来源：http://hz.redwolf501.top/gtbwgrainf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.guannengcc.top/gtyfjbazsb.html

Ruby: ENV["HOME"]
来源：http://hz.jinghuilouyu.cn/gtkgladgoy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yvedp.cn/gtbfbmaonz.html

[M03] 执行外部命令
来源：http://hz.birdmap.top/gthvvebppp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xylfe.cn/gtxbsoaqdi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cdnleiting.top/gtdgnzzpyj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangtech.top/gtxywlrovy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yangfankeji.com/gtmjoejseu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yanxiufei.cn/gtlaovltav.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jlsjyb.cn/gtfpzmwgnh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sufxvd.cn/gtkozymraa.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jqgufenzy.top/gtupjuzliy.html

[M04] 获取当前工作目录
来源：http://hz.meibo888.top/gtiuoxhbix.html

Py:   os.getcwd()
来源：http://hz.hongshengwenyu.top/gtysjkdqxx.html

PHP:  getcwd();
来源：http://hz.nwbrower.top/gtachjnqoq.html

JS:   process.cwd()
来源：http://hz.jyoumei.cn/gtwohissyj.html

TS:   process.cwd()
来源：http://hz.jinghuilouyu.cn/gthvrytfrg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.feifeiyinyue.top/gtaudbkwwa.html

Go:   os.Getwd()
来源：http://hz.hongshengwenyu.top/gtmqpwazqj.html

Ruby: Dir.pwd
来源：http://hz.xinyue.icu/gtwmoikzzt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yangfankeji.com/gtixvsrcde.html

[M05] 设置退出码
来源：http://hz.ehwqpu.com/gtwfifyqnx.html

Py:   sys.exit(1)
来源：http://hz.zdqjudy.top/gtxpiaohmu.html

PHP:  exit(1);
来源：http://hz.xuetiantiany.cn/gtnlcbiqof.html

JS:   process.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gttzxeobvd.html

TS:   process.exit(1)
来源：http://hz.zycfv.cn/gtvackpkjh.html

Java: System.exit(1)
来源：http://hz.zdqjudy.top/gttltodgxs.html

Go:   os.Exit(1)
来源：http://hz.0kj1m.cn/gtpsqnuiuk.html

Ruby: exit 1
来源：http://hz.kuanghao11.cn/gtssggprpp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.tanke756.top/gtftwcmlvz.html

[M06] 向标准错误输出
来源：http://hz.chenlongwang.top/gtdfqkqhsc.html

Py:   print("err", file=sys.stderr)
来源：http://hz.dianchejie.cn/gtapazicua.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.daria6918.cn/gtixmxwqjp.html

JS:   console.error("err")
来源：http://hz.xuanzx.com/gtsxtslwqd.html

TS:   console.error("err")
来源：http://hz.quarkkingdee.top/gtaeevywdo.html

Java: System.err.println("err")
来源：http://hz.hywenlv.cn/gtkvpooxer.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sweek.top/gtmepxscap.html

Ruby: warn "err"
来源：http://hz.gzhubu.top/gtbefrylsc.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.nwbrower.top/gtwzygrjcr.html

[M07] 判断是否为主入口
来源：http://hz.haohaochexian.top/gtghrusjkw.html

Py:   if __name__ == "__main__":
来源：http://hz.hnqzz.top/gtwgipniuc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yvedp.cn/gteeudzgba.html

JS:   require.main === module
来源：http://hz.birdmap.top/gtibaazczg.html

TS:   require.main === module
来源：http://hz.ppjwa.cn/gtrnknsifj.html

Java: public static void main(String[] args)
来源：http://hz.sweek.top/gtflzcbzbb.html

Go:   func main()
来源：http://hz.yangfankeji.com/gthdcubvrc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yonumen.top/gtxgrlyoyr.html

C#:   static void Main(string[] args)
来源：http://hz.nanxinkj.top/gtxgrliqbg.html

[M08] 获取系统与运行时信息
来源：http://hz.redwolf501.top/gtvgwnvefn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.guowangkeji.top/gtzvzqsrcg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhixingplan.top/gtkirjwlmh.html

JS:   process.platform;  process.version
来源：http://hz.pycfn.com/gtlrljeynz.html

TS:   process.platform;  process.version
来源：http://hz.smart0.xyz/gtnezlmyhs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sweek.top/gtwnwjtvbn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.smart0.xyz/gtevnsstlq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yangfankeji.com/gtoutfsxxm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yuxming.cn/gtbtpbrinx.html

================================================================================
来源：http://hz.cdnleiting.top/gtgzfhqtos.html

N. 数据结构与算法
来源：http://hz.birdmap.top/gtppypagnx.html

================================================================================
来源：http://hz.gaohongyu789.top/gtbazmdcck.html

[N01] 二分查找（有序数组）
来源：http://hz.ybcxt.top/gtufwujbze.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yuxming.cn/gtocbmcxaq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gotoacloud.top/gtgzgxuhzv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yanxiufei.cn/gtazpohnay.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fzhhl.top/gtbemdziyw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.316326.xyz/gtfmwecvkw.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhongyouzk.top/gtkuqytcly.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xuetiantiany.cn/gtgiefzfel.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gtlwibiwld.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hysaishi.cn/gtkrsibpue.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xingfuxueyuan.xyz/gtvexhcbrf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nanxuanxn.top/gtjqjmwgvo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shuidangran.top/gtybasbucb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.havefunace.top/gtjahwgurr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.fzhhl.top/gtasmmbysg.html

Go:   slices.Sort(arr)
来源：http://hz.haohaochexian.top/gtsiwfhvdz.html

Ruby: arr.sort
来源：http://hz.jinghuilouyu.cn/gtvlqylyzm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.gaohongyu789.top/gtfbsunonm.html

[N03] 快速排序（分治示例）
来源：http://hz.birdmap.top/gtyxlloyut.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yj202588.top/gtpotdelpo.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xylfe.cn/gttulbsdxk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nwbrower.top/gtbzhoqidt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jyoumei.cn/gttdbbgrcy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hywenlv.cn/gtioqehktt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.aizwys.cn/gtyhhdkadf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shuidangran.top/gthxearlow.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jinyuanbaomall.cn/gtronrktrf.html

[N04] 斐波那契数列
来源：http://hz.jianghu66.top/gtwswccljk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.9152youxi.cn/gttjkshfoe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.gzhubu.top/gtlibxqnio.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aibaodan.cn/gtyyjfcbsy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhiwuduotai.top/gtajrqctec.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jyoumei.cn/gtdxilpsxu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gzhubu.top/gtlnliaeqb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.smart0.xyz/gtfhtsxnqa.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenzaomai.com/gtmkbpxozz.html

[N05] 最大公约数
来源：http://hz.gogol.net.cn/gtlnevnmzw.html

Py:   math.gcd(a, b)
来源：http://hz.redwolf501.top/gtjqmadkzp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yongpay.top/gtygdutynp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.9152youxi.cn/gtovidpxpz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.birdmap.top/gtrugacssj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sufxvd.cn/gthcbhwizh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hnqzz.top/gtidbzplrw.html

Ruby: a.gcd(b)
来源：http://hz.hfpthk.cn/gtyoyrqwvo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ehwqpu.com/gtnynsrzmp.html

[N06] 判断回文字符串
来源：http://hz.fzhhl.top/gtnfgjrnez.html

Py:   s == s[::-1]
来源：http://hz.hammf.cn/gttugxsixp.html

PHP:  $s === strrev($s);
来源：http://hz.shuidangran.top/gtrboajdmg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.kuanghao11.cn/gtsomyfpki.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhiwuduotai.top/gtmeaqdjou.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yj202588.top/gtakkdqcuh.html

Go:   // 双指针从两端比较
来源：http://hz.tianlin.xyz/gtacaezuxx.html

Ruby: s == s.reverse
来源：http://hz.shangyingyoupin.top/gtufmsxanc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hywenlv.cn/gtxbwmniql.html

[N07] 两数之和（返回下标）
来源：http://hz.guannengcc.top/gtfzkgcacd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ydzc1.top/gtpbaisevv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.52xcode.cn/gtihxzdbwc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xuetiantiany.cn/gtocuhwsaj.html

TS:   // 手写 Map<string, number>
来源：http://hz.snrcjt.cn/gtcvwbmznf.html

Java: // 手写 HashMap
来源：http://hz.nwbrower.top/gtwtababqo.html

Go:   // 手写 map[int]int
来源：http://hz.zhiwuduotai.top/gtwemxbvkn.html

Ruby: // 手写 Hash
来源：http://hz.zhijiandao.cn/gtmkcjfaxy.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.dianchejie.cn/gtmzozzsxm.html

[N08] 生成全排列
来源：http://hz.fengsongda.top/gtdmggbtaa.html

Py:   itertools.permutations(arr)
来源：http://hz.hnxiangtu.top/gtowfrygay.html

PHP:  // 手写递归交换
来源：http://hz.gzhubu.top/gtpkvjhpol.html

JS:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtlivwbnzb.html

TS:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtqmjhjplk.html

Java: // 手写回溯递归
来源：http://hz.cashguo.top/gtdscalebi.html

Go:   // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtdxdzjxam.html

Ruby: arr.permutation.to_a
来源：http://hz.feifeiyinyue.top/gtlfvsvgxa.html

C#:   // 手写回溯递归
来源：http://hz.cdnleiting.top/gtrcnekkwz.html

[N09] 栈与队列
来源：http://hz.hfpthk.cn/gtlybwafrf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhongyouzk.top/gtlnuxpkay.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.aizwys.cn/gtxzhmkngu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.feifeiyinyue.top/gtfejsoqps.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.wangshuangyany.cn/gtojzgyuad.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ybcxt.top/gtejsmqlpr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.svipenyu.cn/gtkmnrdioo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yvedp.cn/gtdpplqzgd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.0kj1m.cn/gtngzjccuy.html

[N10] 链表节点定义
来源：http://hz.jqgufenzy.top/gtqzomvpak.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.dianchejie.cn/gtzbptekmk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhoulong.xyz/gtnqkmbuvb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhiwuduotai.top/gtmodtrbfl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sufxvd.cn/gtjjvusrte.html

Java: class Node { int v; Node next; }
来源：http://hz.yanxiufei.cn/gtzhgpisev.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinqigfzy.top/gtltxifbwe.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.chenjidiqi.icu/gtoxjilevx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jqgufenzy.top/gtfwefqfoq.html

[N11] 二叉树中序遍历
来源：http://hz.tianlin.xyz/gtckesgqva.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cashguo.top/gtchhelaee.html


<!-- 参考信息 -->