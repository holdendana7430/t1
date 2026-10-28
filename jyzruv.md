代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shangyingyoupin.top/gtrqcsskdg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.wangshuangyany.cn/gtcoadltbc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.9152youxi.cn/gtfqtcfaka.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xuanzx.com/gthuqfkopu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hammf.cn/gtmpkbdhzw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.feifeiyinyue.top/gtdqqysrzo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ybcxt.top/gtyfhgzvvs.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.svipenyu.cn/gtjuhuiwmg.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xziqi.cn/gtsiypbwxe.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.aizwys.cn/gtuiwfvfna.html

[K04] 读取 JSON 文件
来源：http://hz.pycfn.com/gtvymbdncf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yvedp.cn/gtrslphnyi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhaomingkeji.xyz/gtmogtdjoi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.kuanghao11.cn/gtkjorgmdi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.52xcode.cn/gtpuacaeda.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.c1oappe.top/gthutvvigy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.pycfn.com/gtabxmdowu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yongpay.top/gtalyxwaaz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ydzc1.top/gtnedojdlw.html

[K05] 深拷贝对象
来源：http://hz.jiagoushi.top/gtjduqqzhp.html

Py:   copy.deepcopy(obj)
来源：http://hz.tianlin.xyz/gtbuenofsu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhoulong.xyz/gtgzqbxqpq.html

JS:   structuredClone(obj)
来源：http://hz.svipenyu.cn/gtvnanosvf.html

TS:   structuredClone(obj)
来源：http://hz.fzhhl.top/gtgcglvsya.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gotoacloud.top/gtaoasfslo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yongpay.top/gtkqihaahj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.bjfxy.top/gtwqiyqhuq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yuxming.cn/gtxcaqtcmq.html

[K06] 解析 URL 查询串
来源：http://hz.hnxiangtu.top/gtdffhrhcf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinyuanbaomall.cn/gthsqmvbko.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shuidangran.top/gttijbbfci.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xingfuxueyuan.xyz/gtvsmnyjnz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.redwolf501.top/gtbxaudsaf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.redwolf501.top/gtedfeordw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hnxiangtu.top/gtdeovzxpx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shuidangran.top/gtpdervyju.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhoulong.xyz/gthveskklf.html

[K07] 进制转换
来源：http://hz.cheryme.top/gtxrxzptpw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhengqikj.top/gtkdcmmklc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cucudq.cn/gtqtjwjdxz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.316326.xyz/gtvvkdufzy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.vqdsnc.cn/gtnecgbujk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gtzktomnoy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hfpthk.cn/gtbfqynzoh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.daxiang520.top/gtrfocvlcw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nwbrower.top/gtepcjgcey.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.quarkkingdee.top/gtkcpovovu.html

Py:   pickle.dumps(obj)
来源：http://hz.meibo888.top/gtytkmkqwc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhoulong.xyz/gtfvcsaitp.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.daria6918.cn/gtaygguohj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.guowangkeji.top/gtqyprkwuf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.birdmap.top/gtlqpkfjfn.html

Go:   encoding/gob
来源：http://hz.zycfv.cn/gtvuusnxxh.html

Ruby: Marshal.dump(obj)
来源：http://hz.mhx1999.top/gtliagwzqz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sufxvd.cn/gtxojyiubl.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gthsdfpefq.html

L. 网络请求
来源：http://hz.yongpay.top/gtupnebkom.html

================================================================================
来源：http://hz.snrcjt.cn/gtyhhqyskt.html

[L01] 发送 GET 请求
来源：http://hz.yj20258.top/gtcxvspgwq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.meibo888.top/gtjqmbsjgz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.kuanghao11.cn/gtwfpypicf.html

JS:   await fetch(url)
来源：http://hz.svipenyu.cn/gtofekcldy.html

TS:   await fetch(url)
来源：http://hz.cashguo.top/gtpqiffcxt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.birdmap.top/gttkeweahh.html

Go:   resp, err := http.Get(url)
来源：http://hz.xuetiantiany.cn/gtmjpwpces.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.pengpengdd.cyou/gtjkxflvzr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhixingplan.top/gtjjhkwjmf.html

[L02] 发送 POST JSON
来源：http://hz.ydzc1.top/gtfnpuvqsl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hywenlv.cn/gtcsrogqrv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fengsongda.top/gtrgnyptxd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cdnleiting.top/gtdldewyef.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ydjk.org.cn/gtwkioafvh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.c1oappe.top/gtkivlurcd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ppjwa.cn/gtckmcnbxi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.havefunace.top/gtdfkyuepk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ivvv.top/gtaphtdlkc.html

[L03] 设置自定义请求头
来源：http://hz.yonumen.top/gtsllciwuu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.pycfn.com/gtxgtenpib.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.svipenyu.cn/gtzocrwdaz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xinyue.icu/gtngotvtxw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hywenlv.cn/gtddrdxgsz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yj202588.top/gtoyblfora.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhijiandao.cn/gttjamksdu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cheryme.top/gtwsnhxuzd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.dashuyun.cn/gtgcfzghje.html

[L04] 设置超时
来源：http://hz.shanyushiyangkeji.top/gtlquiuxsl.html

Py:   requests.get(url, timeout=5)
来源：http://hz.svipenyu.cn/gtkqskdzql.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nwbrower.top/gtxvssvzwn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sufxvd.cn/gtdmjhvhhq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.bjfxy.top/gthyzaftfw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.snrcjt.cn/gtqefbvcii.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.tianlin.xyz/gtifhkyorg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jianghu66.top/gtkqllkish.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hnqzz.top/gtrkddjrts.html

[L05] 上传文件（multipart）
来源：http://hz.aizwys.cn/gtwtojrjjn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jqgfzy.top/gtzlrmuppu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.fzhhl.top/gtolksazbz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenjidiqi.icu/gtxfxxoqwp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhoulong.xyz/gthnyakpfv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xuetiantiany.cn/gtvbdaejie.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.316326.xyz/gtzhkjkhjj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.daxiang520.top/gtggpjphlv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.fengsongda.top/gtwbznhiyh.html

[L06] 解析响应为 JSON
来源：http://hz.aibaodan.cn/gtstpgwkus.html

Py:   resp.json()
来源：http://hz.iojbl.cn/gtkwvzdsnv.html

PHP:  json_decode($body, true);
来源：http://hz.yj202588.top/gtexlgpkef.html

JS:   await resp.json()
来源：http://hz.ppjwa.cn/gtiwjuzdox.html

TS:   await resp.json()
来源：http://hz.jinghuilouyu.cn/gtjmypotmm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.fzhhl.top/gtcvytngrd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yuxming.cn/gtmvbldyni.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ppjwa.cn/gtfawgmxvt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yuanzhike.top/gtoirfgmmn.html

[L07] 处理 HTTP 状态码
来源：http://hz.haohaochexian.top/gtpboeuwbk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shanyushiyangkeji.top/gtzyffkfdf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jianghu66.top/gtapgcinrv.html

JS:   resp.ok;  resp.status
来源：http://hz.sysykeji.top/gtyxnootzg.html

TS:   resp.ok;  resp.status
来源：http://hz.tian-w.cn/gtxnnrcakl.html

Java: resp.statusCode()
来源：http://hz.zhongyouzk.top/gtrbhkumnz.html

Go:   resp.StatusCode
来源：http://hz.jinyuanbaomall.cn/gtqxmzcmtn.html

Ruby: resp.code.to_i
来源：http://hz.quarkkingdee.top/gtuklxsfqt.html

C#:   (int)resp.StatusCode
来源：http://hz.yuanzhike.top/gtmgjofbfp.html

[L08] 并发请求多个地址
来源：http://hz.sxryk.cn/gtyszboxje.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.sufxvd.cn/gtldessnqe.html

PHP:  curl_multi_init() 系列
来源：http://hz.yuxming.cn/gtmspjkemv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dashuyun.cn/gtpziavvlx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtspjkwfin.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.guannengcc.top/gtjleyjxaf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shangyingyoupin.top/gtwgocteer.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shuidangran.top/gtoowjalbw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hysaishi.cn/gtmbstisrk.html

================================================================================
来源：http://hz.shzxlz.cn/gtkuyttxwh.html

M. 命令行 / 进程 / 环境
来源：http://hz.yuanzhike.top/gtyktkrpfm.html

================================================================================
来源：http://hz.zhoulong.xyz/gtkqfgmebf.html

[M01] 读取命令行参数
来源：http://hz.hnxiangtu.top/gtkjzwoafr.html

Py:   sys.argv[1:]
来源：http://hz.yangfankeji.com/gtupjedioo.html

PHP:  $argv;  $argc;
来源：http://hz.sysykeji.top/gtwkymvyat.html

JS:   process.argv.slice(2)
来源：http://hz.aibaodan.cn/gtbfqlrfcv.html

TS:   process.argv.slice(2)
来源：http://hz.cashguo.top/gtsraaircr.html

Java: args 数组（main 方法参数）
来源：http://hz.jlsjyb.cn/gtpylcwnso.html

Go:   os.Args[1:]
来源：http://hz.yonumen.top/gtgiekaobk.html

Ruby: ARGV
来源：http://hz.jianghu66.top/gtbtyvpcvi.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yj20258888.top/gtullcccbs.html

[M02] 读取环境变量
来源：http://hz.sufxvd.cn/gtqthugttc.html

Py:   os.environ.get("HOME")
来源：http://hz.hywenlv.cn/gtexymtyvt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hnqzz.top/gtsaflteju.html

JS:   process.env.HOME
来源：http://hz.gotoacloud.top/gtcexguutt.html

TS:   process.env.HOME
来源：http://hz.dashuyun.cn/gtidqenuxw.html

Java: System.getenv("HOME")
来源：http://hz.shanyushiyangkeji.top/gtljzildql.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.wangshuangyany.cn/gtdpcfcmmq.html

Ruby: ENV["HOME"]
来源：http://hz.zhengqikj.top/gtlshlqttq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hfpthk.cn/gtzairnokf.html

[M03] 执行外部命令
来源：http://hz.shuidangran.top/gtjwjdtjzt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yvedp.cn/gtorzfxbdz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xinyue.icu/gtrmezbizz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenlongwang.top/gtfeelbhmn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.dianchejie.cn/gtyitbutsm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.chenlongwang.top/gtqaroilsu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.guowangkeji.top/gtpliweepo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.daria6918.cn/gtueqjqwwz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.pengpengdd.cyou/gtwacwmtti.html

[M04] 获取当前工作目录
来源：http://hz.dianchejie.cn/gtecbhbzhf.html

Py:   os.getcwd()
来源：http://hz.snrcjt.cn/gttcjfgitu.html

PHP:  getcwd();
来源：http://hz.jqgfzy.top/gtglztqkze.html

JS:   process.cwd()
来源：http://hz.meibo888.top/gtfmccysjk.html

TS:   process.cwd()
来源：http://hz.sweek.top/gtuzjrdctp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hammf.cn/gtriccmcgh.html

Go:   os.Getwd()
来源：http://hz.yvedp.cn/gtfzetlsro.html

Ruby: Dir.pwd
来源：http://hz.xingfuxueyuan.xyz/gtplvqwcmr.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.9152youxi.cn/gtofccuipc.html

[M05] 设置退出码
来源：http://hz.gogol.net.cn/gtzetpssoc.html

Py:   sys.exit(1)
来源：http://hz.yangfankeji.com/gtkmmovlnz.html

PHP:  exit(1);
来源：http://hz.yonumen.top/gtgrfvgmxb.html

JS:   process.exit(1)
来源：http://hz.zhoulong.xyz/gtozhpjoae.html

TS:   process.exit(1)
来源：http://hz.zhijiandao.cn/gtoksooawo.html

Java: System.exit(1)
来源：http://hz.52xcode.cn/gteboyhvon.html

Go:   os.Exit(1)
来源：http://hz.pycfn.com/gtycjdqgmg.html

Ruby: exit 1
来源：http://hz.gaohongyu789.top/gtbcxodaud.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nwbrower.top/gtbxygrugv.html

[M06] 向标准错误输出
来源：http://hz.cheryme.top/gtwvaxjsbc.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hammf.cn/gtydfkwonz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ppjwa.cn/gthtytkwtd.html

JS:   console.error("err")
来源：http://hz.kuanghao11.cn/gtfmxygime.html

TS:   console.error("err")
来源：http://hz.hysaishi.cn/gtwtajwlas.html

Java: System.err.println("err")
来源：http://hz.chenjidiqi.icu/gtsnukpbtc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.nanxuanxn.top/gtwjvbjjlf.html

Ruby: warn "err"
来源：http://hz.hnqzz.top/gthfhgxqug.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yongpay.top/gtwqmfjtoq.html

[M07] 判断是否为主入口
来源：http://hz.yj20258.top/gtrubzpdue.html

Py:   if __name__ == "__main__":
来源：http://hz.cucudq.cn/gtcgeyfgfp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ehwqpu.com/gtjhebqxlh.html

JS:   require.main === module
来源：http://hz.xziqi.cn/gtecfqkjtl.html

TS:   require.main === module
来源：http://hz.yongpay.top/gttxpmjjoi.html

Java: public static void main(String[] args)
来源：http://hz.andypj.xyz/gtgamwcalp.html

Go:   func main()
来源：http://hz.xinyue.icu/gthqimtflm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.daria6918.cn/gtjznmjsqx.html

C#:   static void Main(string[] args)
来源：http://hz.svipenyu.cn/gtypncyqlo.html

[M08] 获取系统与运行时信息
来源：http://hz.daria6918.cn/gtwuqycfqd.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yj20258888.top/gtdivhhgxm.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhixingplan.top/gtszicnnxg.html

JS:   process.platform;  process.version
来源：http://hz.pycfn.com/gtjrgbljko.html

TS:   process.platform;  process.version
来源：http://hz.xuanzx.com/gtxfnkloon.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinyuanbaomall.cn/gtwiogvawb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gotoacloud.top/gtyxktqblh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jyoumei.cn/gtszhpuzrz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ppjwa.cn/gtmdklznvs.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtsgkdgdiq.html

N. 数据结构与算法
来源：http://hz.zhongyouzk.top/gtwfgshmfa.html

================================================================================
来源：http://hz.hammf.cn/gtodoeexrp.html

[N01] 二分查找（有序数组）
来源：http://hz.fengsongda.top/gtfbwicfmi.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ydjk.org.cn/gtbeemuxtk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.aibaodan.cn/gtssjkrbes.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenzaomai.com/gtdpviikxo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yuxming.cn/gtatvhcffk.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cheryme.top/gtsgtgrvaz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.smart0.xyz/gtubipopmj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xinyue.icu/gtujahjigf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.guowangkeji.top/gtlibdhcvd.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hammf.cn/gtfuhfkzvn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.nwbrower.top/gtjluvzqcu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ybcxt.top/gtbpkclzvf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhongyouzk.top/gtuqpxuyeb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.feifeiyinyue.top/gtsghbfijh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.redwolf501.top/gtbmnicqiv.html

Go:   slices.Sort(arr)
来源：http://hz.pengpengdd.cyou/gtxfragcri.html

Ruby: arr.sort
来源：http://hz.wangshuangyany.cn/gtgcmtlgik.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yuxming.cn/gtjzweulog.html

[N03] 快速排序（分治示例）
来源：http://hz.vqdsnc.cn/gtmcmdlfrm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhongyouzk.top/gtfvkazyzp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.meibo888.top/gtjwslkxjl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aizwys.cn/gtcgipkbhq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.andypj.xyz/gtbiyexion.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.pycfn.com/gtzluxlgaj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jyoumei.cn/gtzcybgoqc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yvedp.cn/gtukvkkgsd.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xuanzx.com/gtnxigyvov.html

[N04] 斐波那契数列
来源：http://hz.shanyushiyangtech.top/gtjwwmhzaw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinyuanbaomall.cn/gtuoejbxam.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jlsjyb.cn/gtcfjmvyvn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ppjwa.cn/gtdbfwzufq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.redwolf501.top/gtypmwasqh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jianghu66.top/gtxagaxloy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.tian-w.cn/gtcniuihwq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cucudq.cn/gteamgbgwg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhijiandao.cn/gtwtnvdeap.html

[N05] 最大公约数
来源：http://hz.dashuyun.cn/gtvvmvlbeh.html

Py:   math.gcd(a, b)
来源：http://hz.gaohongyu789.top/gtztsymqui.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.pengpengdd.cyou/gtkmosycmn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aizwys.cn/gtmmeeqvee.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xuetiantiany.cn/gtrdxpjvxc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cheryme.top/gttvgmngyg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hongshengwenyu.top/gtwgvptqfq.html

Ruby: a.gcd(b)
来源：http://hz.jinyuanbaomall.cn/gtyrlpegcf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.svipenyu.cn/gtmtxwnili.html

[N06] 判断回文字符串
来源：http://hz.havefunace.top/gtvmfhuiat.html

Py:   s == s[::-1]
来源：http://hz.yuanzhike.top/gtaugbtgpl.html

PHP:  $s === strrev($s);
来源：http://hz.haohaochexian.top/gtukxkwdml.html

JS:   s === [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtemvlbpjh.html

TS:   s === [...s].reverse().join("")
来源：http://hz.mhx1999.top/gttzhejyzz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.tanke756.top/gtoomwhisy.html

Go:   // 双指针从两端比较
来源：http://hz.cqqwz.cn/gtzgcibuof.html

Ruby: s == s.reverse
来源：http://hz.chenjidiqi.icu/gtopeoyysb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.pycfn.com/gtbsnlwsae.html

[N07] 两数之和（返回下标）
来源：http://hz.hnqzz.top/gtiyorrpzv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.316326.xyz/gtmbgudssq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ydjk.org.cn/gtnvbsbtzf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinqigufen.top/gtxdsiossy.html

TS:   // 手写 Map<string, number>
来源：http://hz.jlsjyb.cn/gtleuoyggl.html

Java: // 手写 HashMap
来源：http://hz.chenlongwang.top/gticaujbnh.html

Go:   // 手写 map[int]int
来源：http://hz.tanke756.top/gtcaflqibw.html

Ruby: // 手写 Hash
来源：http://hz.daria6918.cn/gtnbixbnbq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xingfuxueyuan.xyz/gtfxezmcuz.html

[N08] 生成全排列
来源：http://hz.ybcxt.top/gtpqzlvpbz.html

Py:   itertools.permutations(arr)
来源：http://hz.ybcxt.top/gtcxlkbqoo.html

PHP:  // 手写递归交换
来源：http://hz.iojbl.cn/gtnxagzdso.html

JS:   // 手写回溯递归
来源：http://hz.yj20258.top/gtougmatfo.html

TS:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtosdvqhwa.html

Java: // 手写回溯递归
来源：http://hz.52xcode.cn/gtpsqmgkgo.html

Go:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtltiuwtfe.html

Ruby: arr.permutation.to_a
来源：http://hz.snrcjt.cn/gticjuwomz.html

C#:   // 手写回溯递归
来源：http://hz.cashguo.top/gtotzpoaqe.html

[N09] 栈与队列
来源：http://hz.havefunace.top/gtmoonnqde.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.daria6918.cn/gtxuslgfgv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.birdmap.top/gtxakdtemt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yvedp.cn/gtujzxyifi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.andypj.xyz/gtgdvvxdiw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinqigfzy.top/gtverjvgij.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.snrcjt.cn/gtowuxspro.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shanyushiyangtech.top/gtpnvkiyru.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.dashuyun.cn/gtzntjcoyn.html

[N10] 链表节点定义
来源：http://hz.vqdsnc.cn/gtmljsahkp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ywan-chungtsiang.top/gtxpcghltq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.0kj1m.cn/gttxeyfsla.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xinyue.icu/gtsmebsunx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yongpay.top/gtjevwmoyi.html

Java: class Node { int v; Node next; }
来源：http://hz.tian-w.cn/gttmqscbgg.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.pycfn.com/gtolymorjc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhengqikj.top/gtqycljfhj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yj202588.top/gtyryaiukh.html

[N11] 二叉树中序遍历
来源：http://hz.shanyushiyangkeji.top/gtptzaxsqk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xuetiantiany.cn/gthyczpvqe.html


<!-- 参考信息 -->