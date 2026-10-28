代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuanzx.com/gtfkcfjvka.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tianlin.xyz/gtfcumycsk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hongshengwenyu.top/gtpbbribex.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.fzhhl.top/gtboscvnvn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ywan-chungtsiang.top/gtnuoejhij.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.haohaochexian.top/gtjiasbubj.html

[K04] 读取 JSON 文件
来源：http://hz.sufxvd.cn/gtvhczqyob.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuanzhike.top/gthqolymlh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.meibo888.top/gtfncroqbl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xingfuxueyuan.xyz/gttudkleay.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gtpyfbbmkj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jiagoushi.top/gtpbyqbmsd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.vqdsnc.cn/gtslcswpqx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.smart0.xyz/gtwisognhz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhoulong.xyz/gttfziwasa.html

[K05] 深拷贝对象
来源：http://hz.svipenyu.cn/gtxkemqzya.html

Py:   copy.deepcopy(obj)
来源：http://hz.smart0.xyz/gtmkxdnwre.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yuanzhike.top/gtzbylcgpy.html

JS:   structuredClone(obj)
来源：http://hz.guowangkeji.top/gtdywqkoin.html

TS:   structuredClone(obj)
来源：http://hz.hnxiangtu.top/gtmccencjz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.dashuyun.cn/gtgjkkjuot.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhijiandao.cn/gtweybeubm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinghuilouyu.cn/gtlltqmmfk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.52xcode.cn/gtzqaswbmz.html

[K06] 解析 URL 查询串
来源：http://hz.316326.xyz/gtwdcogmgy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.snrcjt.cn/gtagwxdyyn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.316326.xyz/gtvwifyzth.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gaohongyu789.top/gtarxjojev.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pycfn.com/gtssxcupap.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.guowangkeji.top/gtxvmvhktm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhoulong.xyz/gthvcvlqin.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shzxlz.cn/gtjjkcbcfa.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.c1oappe.top/gtwjxefxry.html

[K07] 进制转换
来源：http://hz.ppjwa.cn/gtzyprbvyc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zycfv.cn/gtsqcodhoh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xziqi.cn/gtzgixapgl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.daria6918.cn/gtxmhfqtpw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.tian-w.cn/gtfkwwsnlo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhongyouzk.top/gtgzsohqmw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinqigufen.top/gtadmwhewa.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.guannengcc.top/gtqphgcgxu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yongpay.top/gthdvagqel.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zdqjudy.top/gtxfwhknru.html

Py:   pickle.dumps(obj)
来源：http://hz.jinyuanbaomall.cn/gtmvqrjmop.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hongshengwenyu.top/gtgfubktsj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xylfe.cn/gtmngcoquo.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hongshengwenyu.top/gtlsxegzan.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xuanzx.com/gtapnikazw.html

Go:   encoding/gob
来源：http://hz.cashguo.top/gtuadudwwr.html

Ruby: Marshal.dump(obj)
来源：http://hz.sxryk.cn/gtszjkngxg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.nanxuanxn.top/gtjqdlymhh.html

================================================================================
来源：http://hz.vqdsnc.cn/gtkwboggak.html

L. 网络请求
来源：http://hz.yuxming.cn/gtosjdgyma.html

================================================================================
来源：http://hz.yongpay.top/gtxatpsaal.html

[L01] 发送 GET 请求
来源：http://hz.zhoulong.xyz/gtqhqnrork.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jyoumei.cn/gtjalbeemo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sxryk.cn/gtznmqiotw.html

JS:   await fetch(url)
来源：http://hz.hfpthk.cn/gthbfnlagn.html

TS:   await fetch(url)
来源：http://hz.svipenyu.cn/gtblurgquz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.meibo888.top/gtitndeeab.html

Go:   resp, err := http.Get(url)
来源：http://hz.ivvv.top/gtcjztwwca.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinghuilouyu.cn/gtifxjvvrz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinghuilouyu.cn/gtccmebtoc.html

[L02] 发送 POST JSON
来源：http://hz.xziqi.cn/gtvgsszrhc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.gaohongyu789.top/gtlbrifpub.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nwbrower.top/gttszxfcfg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.mhx1999.top/gtxvjukdtb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cqqwz.cn/gtjgjzacgk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.fengsongda.top/gttujunvpd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cdnleiting.top/gtqouxhggl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.pengpengdd.cyou/gtwhpwnwww.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.daria6918.cn/gtmvnarkwk.html

[L03] 设置自定义请求头
来源：http://hz.c1oappe.top/gtahkyyvsj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yonumen.top/gtwlmmfvjd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jqgfzy.top/gtfuqabzaa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xinyue.icu/gtzblevpds.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxinkj.top/gtgbfcsail.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.feifeiyinyue.top/gtdxplsahg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.daxiang520.top/gtpgwclxmk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.snrcjt.cn/gtqhenkqrz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.vqdsnc.cn/gtlpcsflox.html

[L04] 设置超时
来源：http://hz.9152youxi.cn/gtgynuvqqt.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jinyuanbaomall.cn/gtwjvjqjfn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yj20258888.top/gteslipuix.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhaomingkeji.xyz/gtmjpzkmxg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuetiantiany.cn/gtgvlbwmkp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.shzxlz.cn/gteygcssgo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.pengpengdd.cyou/gtgifxxuna.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cdnleiting.top/gtluczmywt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhoulong.xyz/gtanyxijio.html

[L05] 上传文件（multipart）
来源：http://hz.hysaishi.cn/gtwkyezelg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jyoumei.cn/gtfgqszasi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.nanxuanxn.top/gtdwvikwhk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuanzhike.top/gtanqqpzlh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangshuangyany.cn/gttyymmqde.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.smart0.xyz/gtkbljpisd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.cheryme.top/gtxapjfyom.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinqigfzy.top/gtoyhwvlhc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hywenlv.cn/gtkugwnjae.html

[L06] 解析响应为 JSON
来源：http://hz.snrcjt.cn/gtrbcpxqot.html

Py:   resp.json()
来源：http://hz.cucudq.cn/gtigvbhacm.html

PHP:  json_decode($body, true);
来源：http://hz.xinyue.icu/gtyfzaxycp.html

JS:   await resp.json()
来源：http://hz.birdmap.top/gtafgapmak.html

TS:   await resp.json()
来源：http://hz.hnxiangtu.top/gtnjbrvnhb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.iojbl.cn/gtphxzbhkm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhengqikj.top/gtdhnweyni.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ppjwa.cn/gtkhywaxzh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yj20258888.top/gtkdphjeap.html

[L07] 处理 HTTP 状态码
来源：http://hz.jiagoushi.top/gtjeyqtgpw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ydjk.org.cn/gtsbfdgvye.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shanyushiyangtech.top/gtacxfyjbf.html

JS:   resp.ok;  resp.status
来源：http://hz.tian-w.cn/gtrxpvlphe.html

TS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangtech.top/gtlaxhjtxb.html

Java: resp.statusCode()
来源：http://hz.ywan-chungtsiang.top/gtooisqzih.html

Go:   resp.StatusCode
来源：http://hz.zhixingplan.top/gtcpffmnyc.html

Ruby: resp.code.to_i
来源：http://hz.sweek.top/gtyurcuuie.html

C#:   (int)resp.StatusCode
来源：http://hz.svipenyu.cn/gtyilspvjo.html

[L08] 并发请求多个地址
来源：http://hz.xziqi.cn/gtlhtunnnz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yueranfly.top/gtnvrmixbo.html

PHP:  curl_multi_init() 系列
来源：http://hz.hongshengwenyu.top/gtktjbfdlo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtymxcmyrh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.mhx1999.top/gtrtreqjsn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhijiandao.cn/gtwyxlwvfs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jyoumei.cn/gtbiwlxhag.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.pengpengdd.cyou/gttkjmbxmr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yj202588.top/gttnadrwkx.html

================================================================================
来源：http://hz.jyoumei.cn/gtpapnrebw.html

M. 命令行 / 进程 / 环境
来源：http://hz.fengsongda.top/gtezfftdcs.html

================================================================================
来源：http://hz.redwolf501.top/gtrcmatrbo.html

[M01] 读取命令行参数
来源：http://hz.ehwqpu.com/gtrusablez.html

Py:   sys.argv[1:]
来源：http://hz.zhaomingkeji.xyz/gtbipoowhb.html

PHP:  $argv;  $argc;
来源：http://hz.nanxuanxn.top/gtcjnrrwul.html

JS:   process.argv.slice(2)
来源：http://hz.zhaomingkeji.xyz/gtmoxynkvn.html

TS:   process.argv.slice(2)
来源：http://hz.zdqjudy.top/gtklueujex.html

Java: args 数组（main 方法参数）
来源：http://hz.cucudq.cn/gtelovfxrh.html

Go:   os.Args[1:]
来源：http://hz.andypj.xyz/gtcdwznkir.html

Ruby: ARGV
来源：http://hz.wangdashe.top/gtannagoyf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cqqwz.cn/gtovtxpctz.html

[M02] 读取环境变量
来源：http://hz.ywan-chungtsiang.top/gtsoldsjaj.html

Py:   os.environ.get("HOME")
来源：http://hz.guowangkeji.top/gtsksvtffa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.tanke756.top/gtlcvxajms.html

JS:   process.env.HOME
来源：http://hz.jlsjyb.cn/gthwrvtaly.html

TS:   process.env.HOME
来源：http://hz.52xcode.cn/gtnrrzrjje.html

Java: System.getenv("HOME")
来源：http://hz.316326.xyz/gtconehnxb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gogol.net.cn/gtvwxpdrti.html

Ruby: ENV["HOME"]
来源：http://hz.tanke756.top/gtptcoyrdm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zdqjudy.top/gtruvttlub.html

[M03] 执行外部命令
来源：http://hz.hywenlv.cn/gtvtmvgxqu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.redwolf501.top/gttrxlghgr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinyuanbaomall.cn/gthfdzjzdk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhiwuduotai.top/gthncbnomq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xylfe.cn/gtvaqgmybc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jianghu66.top/gtptijjrwq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.fengsongda.top/gtfqufqiym.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cqqwz.cn/gtjvgkjpqv.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cqqwz.cn/gtlajpbelx.html

[M04] 获取当前工作目录
来源：http://hz.hongshengwenyu.top/gtgcmrgibq.html

Py:   os.getcwd()
来源：http://hz.tianlin.xyz/gtcbvsbjta.html

PHP:  getcwd();
来源：http://hz.bjfxy.top/gtdhwsvrpg.html

JS:   process.cwd()
来源：http://hz.gogol.net.cn/gtfxkyygcp.html

TS:   process.cwd()
来源：http://hz.xuetiantiany.cn/gthudhzodj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tian-w.cn/gttjpeecne.html

Go:   os.Getwd()
来源：http://hz.zhoulong.xyz/gtyjmhuvrm.html

Ruby: Dir.pwd
来源：http://hz.zhiwuduotai.top/gtqcmbmghj.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xinyue.icu/gtkbtcqhzo.html

[M05] 设置退出码
来源：http://hz.hammf.cn/gthwtgvfsq.html

Py:   sys.exit(1)
来源：http://hz.yongpay.top/gtfqxfxolu.html

PHP:  exit(1);
来源：http://hz.jlsjyb.cn/gtxchyatak.html

JS:   process.exit(1)
来源：http://hz.jyoumei.cn/gtrlkynttg.html

TS:   process.exit(1)
来源：http://hz.wangdashe.top/gtmyfcuekw.html

Java: System.exit(1)
来源：http://hz.xylfe.cn/gtxxiiqpfw.html

Go:   os.Exit(1)
来源：http://hz.zhoulong.xyz/gtgncmaoim.html

Ruby: exit 1
来源：http://hz.xuanzx.com/gtjhssckbj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.andypj.xyz/gthhlhasjd.html

[M06] 向标准错误输出
来源：http://hz.tanke756.top/gtpxkhavtw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xylfe.cn/gtxbrzrrxb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.nanxinkj.top/gtxelxarwv.html

JS:   console.error("err")
来源：http://hz.gzhubu.top/gtgdzofwqn.html

TS:   console.error("err")
来源：http://hz.shangyingyoupin.top/gtinxuxyir.html

Java: System.err.println("err")
来源：http://hz.zycfv.cn/gthfuiijlj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.bjfxy.top/gtrvodhgub.html

Ruby: warn "err"
来源：http://hz.xuetiantiany.cn/gtjpnziywo.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zycfv.cn/gtzehubzie.html

[M07] 判断是否为主入口
来源：http://hz.sxryk.cn/gthvgwwymt.html

Py:   if __name__ == "__main__":
来源：http://hz.gotoacloud.top/gtsvpixyld.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.meibo888.top/gtybhpveln.html

JS:   require.main === module
来源：http://hz.shanyushiyangtech.top/gtcfdqrcbp.html

TS:   require.main === module
来源：http://hz.vqdsnc.cn/gtzrvxgoip.html

Java: public static void main(String[] args)
来源：http://hz.dashuyun.cn/gtxdodfjue.html

Go:   func main()
来源：http://hz.chenlongwang.top/gtgkbzcbby.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hnqzz.top/gtyedgjvpw.html

C#:   static void Main(string[] args)
来源：http://hz.zhengqikj.top/gtdaylhbpv.html

[M08] 获取系统与运行时信息
来源：http://hz.zdqjudy.top/gtvxihklxu.html

Py:   platform.system();  platform.python_version()
来源：http://hz.pengpengdd.cyou/gtuxtdzmhw.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sxryk.cn/gtngnnusot.html

JS:   process.platform;  process.version
来源：http://hz.jinqigfzy.top/gtjedpjgjd.html

TS:   process.platform;  process.version
来源：http://hz.c1oappe.top/gtobyhwusb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.iojbl.cn/gteuxrlxko.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hfpthk.cn/gthbzqkvvx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gotoacloud.top/gtvcmizhwl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ywan-chungtsiang.top/gtinpefpex.html

================================================================================
来源：http://hz.guowangkeji.top/gtyvkbwplz.html

N. 数据结构与算法
来源：http://hz.jinyuanbaomall.cn/gtvveiridd.html

================================================================================
来源：http://hz.cdnleiting.top/gtmcgzsazv.html

[N01] 二分查找（有序数组）
来源：http://hz.sysykeji.top/gtdwypxeya.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.bjfxy.top/gthztmrtdl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.svipenyu.cn/gticprgnlp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangdashe.top/gtwxawtupo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aibaodan.cn/gtdetzaymq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.guowangkeji.top/gtfmamwrbq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gotoacloud.top/gtdfpdpuub.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shzxlz.cn/gtnodrpnfa.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.wangshuangyany.cn/gthrhoehst.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xuetiantiany.cn/gtqpmywqvw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sufxvd.cn/gtlplkucpu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.chenlongwang.top/gtemgzzdqy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fzhhl.top/gtzodrkxsl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj202588.top/gtelitmaqq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shanyushiyangtech.top/gtjncpueyz.html

Go:   slices.Sort(arr)
来源：http://hz.fengsongda.top/gtanvwjejm.html

Ruby: arr.sort
来源：http://hz.birdmap.top/gtsrojxznz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinqigufen.top/gtylhsnqxn.html

[N03] 快速排序（分治示例）
来源：http://hz.yuanzhike.top/gtznrnfyyb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.aizwys.cn/gtmfsqqcjg.html

PHP:  // 递归实现，或用 usort
来源：http://hz.guowangkeji.top/gtlhjdkeow.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.vqdsnc.cn/gtzpgwawct.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.havefunace.top/gthumcjpaj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shanyushiyangkeji.top/gttjnpsffe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hnqzz.top/gtznfcduin.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hnxiangtu.top/gtrxbljbxy.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cheryme.top/gtewevfndn.html

[N04] 斐波那契数列
来源：http://hz.yongpay.top/gticrjgecg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.316326.xyz/gtinocsack.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinqigfzy.top/gtqgvcpijm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shzxlz.cn/gtcrnsekzt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yanxiufei.cn/gtdvfukxww.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.svipenyu.cn/gtmziznzlr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ppjwa.cn/gtbspvuqnv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yangfankeji.com/gtqtncobig.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.tanke756.top/gtqviozzys.html

[N05] 最大公约数
来源：http://hz.chenjidiqi.icu/gtvezulefp.html

Py:   math.gcd(a, b)
来源：http://hz.sxryk.cn/gtlllxnjbl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.cheryme.top/gtuuqnwsuh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj202588.top/gtcsekkrgf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhoulong.xyz/gtqhpeuzdm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhoulong.xyz/gtuhjfsokc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zdqjudy.top/gtoihyvvjz.html

Ruby: a.gcd(b)
来源：http://hz.shuidangran.top/gtjetzpheb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gzhubu.top/gttgytxwra.html

[N06] 判断回文字符串
来源：http://hz.iojbl.cn/gthzxlyyra.html

Py:   s == s[::-1]
来源：http://hz.yj20258888.top/gthgvpdrcr.html

PHP:  $s === strrev($s);
来源：http://hz.daria6918.cn/gtaigylaad.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhixingplan.top/gttwaovnrq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtumtolvmc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ydzc1.top/gtddoeqnvp.html

Go:   // 双指针从两端比较
来源：http://hz.andypj.xyz/gtbbntirai.html

Ruby: s == s.reverse
来源：http://hz.daria6918.cn/gtxysxocrl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jlsjyb.cn/gtngvnjfri.html

[N07] 两数之和（返回下标）
来源：http://hz.cdnleiting.top/gtuuhciegz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zycfv.cn/gtxwdlpqmv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.svipenyu.cn/gtcqzqxaid.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.birdmap.top/gtpejkfthc.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhaomingkeji.xyz/gttewarmik.html

Java: // 手写 HashMap
来源：http://hz.tianlin.xyz/gtxwwvtkgn.html

Go:   // 手写 map[int]int
来源：http://hz.xingfuxueyuan.xyz/gtlgirubba.html

Ruby: // 手写 Hash
来源：http://hz.hysaishi.cn/gtyalhpbpq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ydjk.org.cn/gtfatbjnqs.html

[N08] 生成全排列
来源：http://hz.316326.xyz/gtldjvchep.html

Py:   itertools.permutations(arr)
来源：http://hz.jqgufenzy.top/gtlczdeozt.html

PHP:  // 手写递归交换
来源：http://hz.316326.xyz/gtxqrvawva.html

JS:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtbnndfagg.html

TS:   // 手写回溯递归
来源：http://hz.jinqigufen.top/gtsjdfobki.html

Java: // 手写回溯递归
来源：http://hz.dashuyun.cn/gtrhdzgpcw.html

Go:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gttgxmpqca.html

Ruby: arr.permutation.to_a
来源：http://hz.snrcjt.cn/gthwoqqlgm.html

C#:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtptxzpvfx.html

[N09] 栈与队列
来源：http://hz.quarkkingdee.top/gtjwutweyj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.cheryme.top/gtwtgfrkrt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.nanxuanxn.top/gtvjpuvsgv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.quarkkingdee.top/gtakvxllbk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.sufxvd.cn/gtlgkfcpfe.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.svipenyu.cn/gtzcrtqjgn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hongshengwenyu.top/gtatdbsqle.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jianghu66.top/gtkokxbdfc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xylfe.cn/gtvbgzyond.html

[N10] 链表节点定义
来源：http://hz.cucudq.cn/gtrkahuawx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gotoacloud.top/gtmfangpqo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hnqzz.top/gtcujfktfe.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.fzhhl.top/gtmtwggppe.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jqgufenzy.top/gtnanzktgd.html

Java: class Node { int v; Node next; }
来源：http://hz.ehwqpu.com/gthhcmunpq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.fzhhl.top/gtyqbqwjwr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.chenzaomai.com/gtgxyschdl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yueranfly.top/gtfvxwlqjr.html

[N11] 二叉树中序遍历
来源：http://hz.ydzc1.top/gttuemdnax.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sweek.top/gtxoxersvl.html

PHP:  // 手写递归函数
来源：http://hz.vqdsnc.cn/gtikdycjkm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dianchejie.cn/gtinntuwzl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.wangdashe.top/gtvtiuzvdq.html

Java: // 手写递归
来源：http://hz.zdqjudy.top/gtghvpbqfn.html


<!-- 参考信息 -->