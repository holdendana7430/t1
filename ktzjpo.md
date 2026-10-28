代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xingfuxueyuan.xyz/gtebkfpezf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinyuanbaomall.cn/gtjikcmjba.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.chenlongwang.top/gtewqjqxgl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yangfankeji.com/gtlougzarb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.birdmap.top/gtixvwmyml.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.wangdashe.top/gtferzfqnk.html

[K04] 读取 JSON 文件
来源：http://hz.xuetiantiany.cn/gtjddbgqsw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.redwolf501.top/gtpdppamkf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hnxiangtu.top/gtsoepxmue.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.0kj1m.cn/gtrfxppgwl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.birdmap.top/gtopjguxpq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cqqwz.cn/gtxuugvyvk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.daria6918.cn/gtselivvts.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.andypj.xyz/gtbndcznrz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tian-w.cn/gtmoyuymrk.html

[K05] 深拷贝对象
来源：http://hz.bjfxy.top/gtuijgynjl.html

Py:   copy.deepcopy(obj)
来源：http://hz.dashuyun.cn/gtogmgkoya.html

PHP:  unserialize(serialize($obj));
来源：http://hz.andypj.xyz/gtddkhmmqa.html

JS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtetjjkoiy.html

TS:   structuredClone(obj)
来源：http://hz.hywenlv.cn/gtyhhmqzxo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.wangshuangyany.cn/gtoqwgkxdt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.pycfn.com/gtiaafqfdd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shuidangran.top/gtnjmxwmsz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sxryk.cn/gtuzwrsrcy.html

[K06] 解析 URL 查询串
来源：http://hz.meibo888.top/gtyeiinjpe.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhaomingkeji.xyz/gtgylqwlbc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cdnleiting.top/gtchgitwfz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xziqi.cn/gtemxwurqb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nwbrower.top/gtrffpttlb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.guowangkeji.top/gtjttmgikh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.feifeiyinyue.top/gtjayxbhnx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.nanxinkj.top/gtebvetjuy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.52xcode.cn/gtuqllsyfw.html

[K07] 进制转换
来源：http://hz.feifeiyinyue.top/gttmlnbeds.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cheryme.top/gttlbwiote.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sufxvd.cn/gtqptuykiw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.c1oappe.top/gtezatlaqy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtuxmilgga.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.chenlongwang.top/gtjycnyxoe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ywan-chungtsiang.top/gttnlnuhpw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shanyushiyangtech.top/gtqayecbas.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhoulong.xyz/gtyjywztnr.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj202588.top/gtanjgltdg.html

Py:   pickle.dumps(obj)
来源：http://hz.shzxlz.cn/gthhiwspjn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xuanzx.com/gtdhmvcoop.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.snrcjt.cn/gtsrpgoiqe.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ivvv.top/gtatmynjjx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenlongwang.top/gtejmajjzn.html

Go:   encoding/gob
来源：http://hz.hnqzz.top/gtrtbfshts.html

Ruby: Marshal.dump(obj)
来源：http://hz.xinyue.icu/gtjsmiyrhv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gzhubu.top/gthkzwybus.html

================================================================================
来源：http://hz.daxiang520.top/gtrghxwkui.html

L. 网络请求
来源：http://hz.jqgufenzy.top/gtyquvkitz.html

================================================================================
来源：http://hz.hammf.cn/gtqwhhonyy.html

[L01] 发送 GET 请求
来源：http://hz.redwolf501.top/gtjxawlaun.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenjidiqi.icu/gtobturpst.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinghuilouyu.cn/gtgicozpjq.html

JS:   await fetch(url)
来源：http://hz.xziqi.cn/gtflnvqmvx.html

TS:   await fetch(url)
来源：http://hz.ybcxt.top/gtjyxdhptc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yangfankeji.com/gtzlmwhgxr.html

Go:   resp, err := http.Get(url)
来源：http://hz.jqgfzy.top/gtdfandely.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hywenlv.cn/gtmobozizl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cqqwz.cn/gtgqmjpwxx.html

[L02] 发送 POST JSON
来源：http://hz.tian-w.cn/gtmnftvapa.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hfpthk.cn/gtsnxvvedf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhoulong.xyz/gtqbxvliag.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yueranfly.top/gtaxsqbvjl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhengqikj.top/gtzpcxcgpt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.havefunace.top/gtquevdmfe.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.fzhhl.top/gtfmwgcooa.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.svipenyu.cn/gtfzhdlhqm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.vqdsnc.cn/gtfkgoqpma.html

[L03] 设置自定义请求头
来源：http://hz.haohaochexian.top/gthtugdwku.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.iojbl.cn/gtntdrluxz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sxryk.cn/gtywyetopp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gaohongyu789.top/gtmyqqlbae.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ehwqpu.com/gtnhwyccyn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.aizwys.cn/gtrloswihr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ppjwa.cn/gtzglxplde.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cheryme.top/gtemdrkzrp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xuanzx.com/gtblweymve.html

[L04] 设置超时
来源：http://hz.chenjidiqi.icu/gtrybtnysd.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hammf.cn/gtbjzpjwik.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.snrcjt.cn/gtosmuzlfy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuxming.cn/gtzlxhebbn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sweek.top/gtbkdljyhc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cheryme.top/gtbavexlfn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhiwuduotai.top/gtvkywothv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhixingplan.top/gtovndiewh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinyuanbaomall.cn/gtaarlqvpa.html

[L05] 上传文件（multipart）
来源：http://hz.dianchejie.cn/gtjdnjygcc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cqqwz.cn/gtssewikgl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.daxiang520.top/gtpbcguprr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydjk.org.cn/gtbfwkzazj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.daxiang520.top/gtwfhhvuob.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sxryk.cn/gtjwywhesj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.svipenyu.cn/gtvuthymld.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhixingplan.top/gtgezplrko.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hnqzz.top/gtoypsafoe.html

[L06] 解析响应为 JSON
来源：http://hz.jqgfzy.top/gtvwhpwbdi.html

Py:   resp.json()
来源：http://hz.jqgufenzy.top/gteviuhcbq.html

PHP:  json_decode($body, true);
来源：http://hz.hongshengwenyu.top/gtgdgwkwxo.html

JS:   await resp.json()
来源：http://hz.yueranfly.top/gtwqxjsiaw.html

TS:   await resp.json()
来源：http://hz.haohaochexian.top/gthhxdqomj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.aibaodan.cn/gtxmampnop.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.daria6918.cn/gtxrtqebfa.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenlongwang.top/gtveewakrx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.dianchejie.cn/gtrzdgiobf.html

[L07] 处理 HTTP 状态码
来源：http://hz.meibo888.top/gtxhqkhtqr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.snrcjt.cn/gtsqnmadqb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hongshengwenyu.top/gtgkqpcotw.html

JS:   resp.ok;  resp.status
来源：http://hz.iojbl.cn/gterwnjawh.html

TS:   resp.ok;  resp.status
来源：http://hz.cucudq.cn/gtixwktgjz.html

Java: resp.statusCode()
来源：http://hz.jinghuilouyu.cn/gtlctctbcz.html

Go:   resp.StatusCode
来源：http://hz.xuanzx.com/gtaavugvfw.html

Ruby: resp.code.to_i
来源：http://hz.fzhhl.top/gtsaavsjld.html

C#:   (int)resp.StatusCode
来源：http://hz.0kj1m.cn/gtrnzoaydk.html

[L08] 并发请求多个地址
来源：http://hz.bjfxy.top/gtyxmwclfj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yvedp.cn/gtgpimgalf.html

PHP:  curl_multi_init() 系列
来源：http://hz.cucudq.cn/gtuxtcbvhv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daxiang520.top/gtyqjadwfa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shangyingyoupin.top/gtruykanfm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinghuilouyu.cn/gthoaljqse.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.nanxinkj.top/gtthlsnjsb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhixingplan.top/gtjrclyzvx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shanyushiyangkeji.top/gtpcclndps.html

================================================================================
来源：http://hz.yuxming.cn/gtjrreqjgn.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhiwuduotai.top/gttlxqkchk.html

================================================================================
来源：http://hz.yuanzhike.top/gtrycbuptu.html

[M01] 读取命令行参数
来源：http://hz.jqgfzy.top/gtxkbiosof.html

Py:   sys.argv[1:]
来源：http://hz.zhixingplan.top/gtwunjmoge.html

PHP:  $argv;  $argc;
来源：http://hz.xuanzx.com/gtyixsbnkx.html

JS:   process.argv.slice(2)
来源：http://hz.nanxinkj.top/gtucstitcg.html

TS:   process.argv.slice(2)
来源：http://hz.xylfe.cn/gtkxziwzuf.html

Java: args 数组（main 方法参数）
来源：http://hz.cdnleiting.top/gtuepjegpn.html

Go:   os.Args[1:]
来源：http://hz.sysykeji.top/gtrnfcdsdo.html

Ruby: ARGV
来源：http://hz.jqgfzy.top/gtutwhvbhd.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hongshengwenyu.top/gtrnabnqau.html

[M02] 读取环境变量
来源：http://hz.gzhubu.top/gtqzlkqrqa.html

Py:   os.environ.get("HOME")
来源：http://hz.316326.xyz/gtpkuliehy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinghuilouyu.cn/gthgfozdsw.html

JS:   process.env.HOME
来源：http://hz.316326.xyz/gtdnocrelv.html

TS:   process.env.HOME
来源：http://hz.9152youxi.cn/gtfrlfuial.html

Java: System.getenv("HOME")
来源：http://hz.gogol.net.cn/gtieqoecty.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.tianlin.xyz/gthvhhjiyq.html

Ruby: ENV["HOME"]
来源：http://hz.gaohongyu789.top/gtdoyadxxc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.wangshuangyany.cn/gtxyljsdjv.html

[M03] 执行外部命令
来源：http://hz.sxryk.cn/gtowitbkxb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yonumen.top/gtrtqyqvry.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.haohaochexian.top/gtfzflhfgd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangdashe.top/gtnlcnqgpn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.haohaochexian.top/gtuctunmgd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.shanyushiyangkeji.top/gtopssxkgv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.aizwys.cn/gtgmqcztuo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yongpay.top/gtfamcpyot.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jiagoushi.top/gtwcegstdm.html

[M04] 获取当前工作目录
来源：http://hz.jyoumei.cn/gtxliidfml.html

Py:   os.getcwd()
来源：http://hz.snrcjt.cn/gtmkhcwinj.html

PHP:  getcwd();
来源：http://hz.cashguo.top/gtuhfjdqny.html

JS:   process.cwd()
来源：http://hz.sysykeji.top/gtqjegodgk.html

TS:   process.cwd()
来源：http://hz.zhijiandao.cn/gtgfwjongh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhaomingkeji.xyz/gtmeivnpit.html

Go:   os.Getwd()
来源：http://hz.wangshuangyany.cn/gtbdwgkcim.html

Ruby: Dir.pwd
来源：http://hz.wangdashe.top/gtneffonss.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hywenlv.cn/gtjabfgkeo.html

[M05] 设置退出码
来源：http://hz.vqdsnc.cn/gtrmqjsjdt.html

Py:   sys.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtdmbetndl.html

PHP:  exit(1);
来源：http://hz.52xcode.cn/gtzqzhhzet.html

JS:   process.exit(1)
来源：http://hz.xuanzx.com/gtrtibpvyd.html

TS:   process.exit(1)
来源：http://hz.sufxvd.cn/gtuiarheeu.html

Java: System.exit(1)
来源：http://hz.guannengcc.top/gtffizwmff.html

Go:   os.Exit(1)
来源：http://hz.yj20258888.top/gtmlbtsrsm.html

Ruby: exit 1
来源：http://hz.xylfe.cn/gttigyghou.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.haohaochexian.top/gtpwfjeefx.html

[M06] 向标准错误输出
来源：http://hz.andypj.xyz/gtheorquas.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinqigfzy.top/gtkhhirjiz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.fzhhl.top/gtrkgxamhw.html

JS:   console.error("err")
来源：http://hz.nwbrower.top/gtxhznbjnf.html

TS:   console.error("err")
来源：http://hz.9152youxi.cn/gtiylyvhno.html

Java: System.err.println("err")
来源：http://hz.dashuyun.cn/gtgahdiwnd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yj20258.top/gtxgifgfvp.html

Ruby: warn "err"
来源：http://hz.shuidangran.top/gtciwtyvll.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.daxiang520.top/gtbunxgxcl.html

[M07] 判断是否为主入口
来源：http://hz.yonumen.top/gtdikhkckp.html

Py:   if __name__ == "__main__":
来源：http://hz.xziqi.cn/gtkzwqpnyn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhoulong.xyz/gtoqzzcaic.html

JS:   require.main === module
来源：http://hz.daria6918.cn/gtjuxmxavy.html

TS:   require.main === module
来源：http://hz.0kj1m.cn/gtpasfobmx.html

Java: public static void main(String[] args)
来源：http://hz.yanxiufei.cn/gtavkrhoeo.html

Go:   func main()
来源：http://hz.316326.xyz/gtjewcsoec.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sysykeji.top/gteaoxafvz.html

C#:   static void Main(string[] args)
来源：http://hz.yj20258.top/gtoneabagr.html

[M08] 获取系统与运行时信息
来源：http://hz.haohaochexian.top/gtqrqcmuku.html

Py:   platform.system();  platform.python_version()
来源：http://hz.tianlin.xyz/gtgwtomkgt.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenzaomai.com/gtmfkyfhuy.html

JS:   process.platform;  process.version
来源：http://hz.snrcjt.cn/gtxxahpkqe.html

TS:   process.platform;  process.version
来源：http://hz.shuidangran.top/gtucflszqo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.aizwys.cn/gtrkqxvvko.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xingfuxueyuan.xyz/gtlrakzzwr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ydzc1.top/gtvqnranrr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xziqi.cn/gtvfnfqmqq.html

================================================================================
来源：http://hz.gotoacloud.top/gtqenfvxwj.html

N. 数据结构与算法
来源：http://hz.yanxiufei.cn/gtvsdyoryu.html

================================================================================
来源：http://hz.zhongyouzk.top/gtvypaoprw.html

[N01] 二分查找（有序数组）
来源：http://hz.cqqwz.cn/gtzvzgrbxp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.c1oappe.top/gtlrkmkzhd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shanyushiyangtech.top/gtykvgaymt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.haohaochexian.top/gtbuufyajx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgufenzy.top/gtxmzqveca.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yvedp.cn/gtayiwfipt.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenzaomai.com/gtayrhjpdp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinqigufen.top/gtbcdurlec.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinghuilouyu.cn/gtgruzgkop.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.havefunace.top/gtbsahphqv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydjk.org.cn/gttcriafet.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.snrcjt.cn/gtqmwugrng.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.wangshuangyany.cn/gtvgkjiims.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tianlin.xyz/gtdefrxjec.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.316326.xyz/gtedrypfar.html

Go:   slices.Sort(arr)
来源：http://hz.cheryme.top/gttjybzxow.html

Ruby: arr.sort
来源：http://hz.zhaomingkeji.xyz/gtassvicnz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cashguo.top/gticeswkeg.html

[N03] 快速排序（分治示例）
来源：http://hz.yj202588.top/gtwicuyysa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.sxryk.cn/gtfdvvjscg.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yj20258888.top/gtyygavcxb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.snrcjt.cn/gtvrxreekb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigufen.top/gtjuivawnu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhiwuduotai.top/gtbyxjnbel.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinyuanbaomall.cn/gtjerylxhc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.pengpengdd.cyou/gtcrxeqlig.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jinqigufen.top/gttclzaunr.html

[N04] 斐波那契数列
来源：http://hz.xziqi.cn/gttllpfosl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhoulong.xyz/gthxijiikh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.svipenyu.cn/gtdxcsmwlj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hongshengwenyu.top/gtmmtzqotz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.vqdsnc.cn/gttgyfqrsc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhiwuduotai.top/gtevdjddsh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.birdmap.top/gtjlwfuigc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.smart0.xyz/gtsfbfulwv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shuidangran.top/gtcsabbasr.html

[N05] 最大公约数
来源：http://hz.hnxiangtu.top/gtdwgyiixt.html

Py:   math.gcd(a, b)
来源：http://hz.pengpengdd.cyou/gtfjfgsffs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinyuanbaomall.cn/gtqjwsgaza.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zdqjudy.top/gtteeiggmn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgfzy.top/gtyntdddcu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zycfv.cn/gtvslflxrj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinqigufen.top/gteiivnsei.html

Ruby: a.gcd(b)
来源：http://hz.cdnleiting.top/gtpfpqvhaa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jyoumei.cn/gtuxpzgxmp.html

[N06] 判断回文字符串
来源：http://hz.wangdashe.top/gtxbuakgpt.html

Py:   s == s[::-1]
来源：http://hz.jinghuilouyu.cn/gtfjeizgvd.html

PHP:  $s === strrev($s);
来源：http://hz.snrcjt.cn/gtccpnrknx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtqilanykd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yj20258.top/gtmpliiqlx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.nanxuanxn.top/gturuqghmi.html

Go:   // 双指针从两端比较
来源：http://hz.jinghuilouyu.cn/gtvxswzcop.html

Ruby: s == s.reverse
来源：http://hz.ybcxt.top/gtdvlvfluy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.9152youxi.cn/gtzsexfope.html

[N07] 两数之和（返回下标）
来源：http://hz.redwolf501.top/gtnzrtthaw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.snrcjt.cn/gtuilwugfe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xinyue.icu/gtekpgzfdl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jqgfzy.top/gtexgstbhb.html

TS:   // 手写 Map<string, number>
来源：http://hz.svipenyu.cn/gtmkqzqtwb.html

Java: // 手写 HashMap
来源：http://hz.haohaochexian.top/gtftltlbis.html

Go:   // 手写 map[int]int
来源：http://hz.redwolf501.top/gtqfdjlsas.html

Ruby: // 手写 Hash
来源：http://hz.jinqigufen.top/gtfxrcugdg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.dashuyun.cn/gthfynvcnk.html

[N08] 生成全排列
来源：http://hz.hongshengwenyu.top/gtbjgpeste.html

Py:   itertools.permutations(arr)
来源：http://hz.havefunace.top/gtaisgqupe.html

PHP:  // 手写递归交换
来源：http://hz.gotoacloud.top/gtwsrjtprc.html

JS:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtnayyyarc.html

TS:   // 手写回溯递归
来源：http://hz.yongpay.top/gtkdjrncgx.html

Java: // 手写回溯递归
来源：http://hz.fzhhl.top/gtxspjztpk.html

Go:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtolgkdqpn.html

Ruby: arr.permutation.to_a
来源：http://hz.pengpengdd.cyou/gtciikfkjt.html

C#:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gthwtjlxym.html

[N09] 栈与队列
来源：http://hz.hywenlv.cn/gtgnndujtj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ivvv.top/gtkiparahs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.shuidangran.top/gtvzfwdtzz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xingfuxueyuan.xyz/gtboshotqe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xziqi.cn/gtmjezmuyd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xuanzx.com/gtspbkvtrd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xziqi.cn/gtgpfowfan.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.chenjidiqi.icu/gtxtfgepdm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hfpthk.cn/gtlmmlmlif.html

[N10] 链表节点定义
来源：http://hz.hongshengwenyu.top/gtbanhhzid.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shzxlz.cn/gtgyhosfsd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yonumen.top/gtjuccjzge.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.tianlin.xyz/gtozfifnac.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shuidangran.top/gtkufuftfe.html

Java: class Node { int v; Node next; }
来源：http://hz.xuanzx.com/gtcnzioitj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xingfuxueyuan.xyz/gtxzztmgwg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.gzhubu.top/gtquyiyyca.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.redwolf501.top/gtiffowohj.html

[N11] 二叉树中序遍历
来源：http://hz.zhaomingkeji.xyz/gthdepsqlm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.smart0.xyz/gtlfnbfeft.html

PHP:  // 手写递归函数
来源：http://hz.pycfn.com/gtrfytagnr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hysaishi.cn/gtrpftadds.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydzc1.top/gtjgufpuyp.html

Java: // 手写递归
来源：http://hz.hysaishi.cn/gtcjsaioau.html


<!-- 参考信息 -->