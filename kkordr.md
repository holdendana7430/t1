代发 wailian999

TS:   JSON.parse(s)
来源：http://hz.meibo888.top/gtujvdrgci.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jlsjyb.cn/gtclojiwhc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhengqikj.top/gtbolpbtuq.html

Ruby: JSON.parse(s)
来源：http://hz.mhx1999.top/gtxpmczrsk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cheryme.top/gtszqpgtbl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yueranfly.top/gtpzqqfsvm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ybcxt.top/gtmmnlsxks.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hnqzz.top/gtzolzaogu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangkeji.top/gtmftfxxha.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.andypj.xyz/gtfyhhewsb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.guowangkeji.top/gtnciftein.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.wangdashe.top/gtoajncuoc.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shanyushiyangkeji.top/gtyexdmnug.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhongyouzk.top/gtcrloptfq.html

[K04] 读取 JSON 文件
来源：http://hz.yueranfly.top/gtzzajapfj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenjidiqi.icu/gtlhqbrrcp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cucudq.cn/gtgzmzjrtr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yanxiufei.cn/gtjyccrdes.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinghuilouyu.cn/gtponadgtl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhaomingkeji.xyz/gtibhuqjoh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.snrcjt.cn/gtntojbcmw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jqgufenzy.top/gtwgeipngj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yangfankeji.com/gtwkvtsdru.html

[K05] 深拷贝对象
来源：http://hz.hysaishi.cn/gtqrxwxnrj.html

Py:   copy.deepcopy(obj)
来源：http://hz.aibaodan.cn/gtlzfjmqsp.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenlongwang.top/gtnhljnifp.html

JS:   structuredClone(obj)
来源：http://hz.yj20258.top/gtsdzwzouz.html

TS:   structuredClone(obj)
来源：http://hz.c1oappe.top/gtssidalfv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinqigufen.top/gtsnovklkv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.kuanghao11.cn/gtstycdzfm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yj20258888.top/gtsuaelcwb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj20258.top/gtyxxosepp.html

[K06] 解析 URL 查询串
来源：http://hz.wangdashe.top/gttbhborae.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.pycfn.com/gtxpmdgdzh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinghuilouyu.cn/gtrwckogko.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgfzy.top/gtsbqoorfl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yangfankeji.com/gtomsqfbdp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.fengsongda.top/gtmlgmgbrj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj20258.top/gteclzazwy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.nwbrower.top/gtaavdwpzv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.pycfn.com/gtgtcfoyzh.html

[K07] 进制转换
来源：http://hz.zhiwuduotai.top/gtjywjgocv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shuidangran.top/gtywrkyfvy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.havefunace.top/gtqodpzrcw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ybcxt.top/gtjvaiquwn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtrqjsncnv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.dianchejie.cn/gtwssjwlzw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.316326.xyz/gtsxexjiki.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yueranfly.top/gtczssgbvb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ydzc1.top/gtslieuwzy.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.svipenyu.cn/gtdjvovgey.html

Py:   pickle.dumps(obj)
来源：http://hz.cdnleiting.top/gtejnoocsh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.daria6918.cn/gtucseclvb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jlsjyb.cn/gtfocawwtw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.bjfxy.top/gtpantbxtl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenlongwang.top/gtxdpuhixf.html

Go:   encoding/gob
来源：http://hz.ivvv.top/gtqbttflzz.html

Ruby: Marshal.dump(obj)
来源：http://hz.shzxlz.cn/gtmotoswln.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jqgufenzy.top/gtvmxuyvfb.html

================================================================================
来源：http://hz.nanxinkj.top/gtgvjnvlik.html

L. 网络请求
来源：http://hz.cheryme.top/gttmhpmurf.html

================================================================================
来源：http://hz.jinqigufen.top/gttzifnquy.html

[L01] 发送 GET 请求
来源：http://hz.ywan-chungtsiang.top/gtcyrgwzdn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yonumen.top/gtihjcajyr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhongyouzk.top/gtcbiuqtzz.html

JS:   await fetch(url)
来源：http://hz.yanxiufei.cn/gtiddmqomx.html

TS:   await fetch(url)
来源：http://hz.hysaishi.cn/gtywikpour.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.haohaochexian.top/gtnnchrdbx.html

Go:   resp, err := http.Get(url)
来源：http://hz.aibaodan.cn/gtfudibgxp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cashguo.top/gtmtfvvkpu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jianghu66.top/gtfvlirfde.html

[L02] 发送 POST JSON
来源：http://hz.hfpthk.cn/gtejanmmnv.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shzxlz.cn/gtveymvpmu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.52xcode.cn/gtdqppmijn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258888.top/gtbnpdfyrl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ppjwa.cn/gterrvflad.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhiwuduotai.top/gtneubiakh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yuanzhike.top/gtkpuvswrd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nanxuanxn.top/gtbfnrcxpf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ehwqpu.com/gtqjoxnmea.html

[L03] 设置自定义请求头
来源：http://hz.chenlongwang.top/gtdejvyxlj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zdqjudy.top/gttekjuzod.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ydjk.org.cn/gtshjgzoji.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangshuangyany.cn/gtbemogyox.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.feifeiyinyue.top/gtyupojyhz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yuanzhike.top/gtcxnilrhy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yuanzhike.top/gtrrgqugoz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj202588.top/gtptuckvwr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.meibo888.top/gtxfixdggv.html

[L04] 设置超时
来源：http://hz.tianlin.xyz/gtrwqgwjnt.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hnqzz.top/gtoyfmmxov.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ehwqpu.com/gttxfqdxxb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gzhubu.top/gtmubeemgz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hongshengwenyu.top/gthfiqbyhw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinyuanbaomall.cn/gttbhvmpsl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yuanzhike.top/gtdelhgdij.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hnqzz.top/gtwdhhchxi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shangyingyoupin.top/gtyxlilheu.html

[L05] 上传文件（multipart）
来源：http://hz.haohaochexian.top/gtzzyqfxvy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.fengsongda.top/gtljlupzjr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhengqikj.top/gtpwgiuodu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.c1oappe.top/gtyhscvsau.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jyoumei.cn/gtotpgbfyh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cheryme.top/gtzaosrcku.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.tianlin.xyz/gtzespoahq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yongpay.top/gtpbqimeif.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.316326.xyz/gtyqrixifu.html

[L06] 解析响应为 JSON
来源：http://hz.nanxinkj.top/gtyxtvirtq.html

Py:   resp.json()
来源：http://hz.daxiang520.top/gtlkwchbkb.html

PHP:  json_decode($body, true);
来源：http://hz.shuidangran.top/gtwlgunuwe.html

JS:   await resp.json()
来源：http://hz.birdmap.top/gtsfdrptdq.html

TS:   await resp.json()
来源：http://hz.pengpengdd.cyou/gtjnprmprz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinyuanbaomall.cn/gttsejahnp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shangyingyoupin.top/gtuomxgivv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.meibo888.top/gtvafwiwxe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shanyushiyangkeji.top/gtdjncrgpi.html

[L07] 处理 HTTP 状态码
来源：http://hz.vqdsnc.cn/gtbtkbqdjo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sysykeji.top/gtauoygfew.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ydzc1.top/gtqsjnrcvd.html

JS:   resp.ok;  resp.status
来源：http://hz.snrcjt.cn/gtcrqntict.html

TS:   resp.ok;  resp.status
来源：http://hz.gotoacloud.top/gtgxcazgml.html

Java: resp.statusCode()
来源：http://hz.kuanghao11.cn/gtniqlglsk.html

Go:   resp.StatusCode
来源：http://hz.cdnleiting.top/gtdepqkhjk.html

Ruby: resp.code.to_i
来源：http://hz.smart0.xyz/gtlijowukg.html

C#:   (int)resp.StatusCode
来源：http://hz.svipenyu.cn/gtqrhryujb.html

[L08] 并发请求多个地址
来源：http://hz.snrcjt.cn/gtbrgjacwx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.aibaodan.cn/gtkfmkxvjg.html

PHP:  curl_multi_init() 系列
来源：http://hz.ywan-chungtsiang.top/gthntqqyqs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtlvmjdhwz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xinyue.icu/gtknfgtzju.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ivvv.top/gtbullpldn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hnqzz.top/gtvrxzxxpp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hongshengwenyu.top/gtunygioji.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ivvv.top/gtateqjrbp.html

================================================================================
来源：http://hz.yj20258.top/gtdddbloyb.html

M. 命令行 / 进程 / 环境
来源：http://hz.zdqjudy.top/gtfyucjxkl.html

================================================================================
来源：http://hz.nanxinkj.top/gtepobajkm.html

[M01] 读取命令行参数
来源：http://hz.316326.xyz/gtljaoqbnw.html

Py:   sys.argv[1:]
来源：http://hz.zycfv.cn/gtyvsnobwi.html

PHP:  $argv;  $argc;
来源：http://hz.c1oappe.top/gtthmjdrnh.html

JS:   process.argv.slice(2)
来源：http://hz.cqqwz.cn/gtulikvhzz.html

TS:   process.argv.slice(2)
来源：http://hz.ydjk.org.cn/gtqboknypj.html

Java: args 数组（main 方法参数）
来源：http://hz.zhaomingkeji.xyz/gtkqthjnfb.html

Go:   os.Args[1:]
来源：http://hz.kuanghao11.cn/gtpaztrvxx.html

Ruby: ARGV
来源：http://hz.cqqwz.cn/gtubafuptu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yuxming.cn/gtyuycvfsr.html

[M02] 读取环境变量
来源：http://hz.smart0.xyz/gtuxrkbdxa.html

Py:   os.environ.get("HOME")
来源：http://hz.haohaochexian.top/gtomdyogzh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ybcxt.top/gtunsaacbc.html

JS:   process.env.HOME
来源：http://hz.jqgufenzy.top/gtxwpevtyx.html

TS:   process.env.HOME
来源：http://hz.hammf.cn/gtyybiwpfd.html

Java: System.getenv("HOME")
来源：http://hz.tianlin.xyz/gtaurtrcvw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yuxming.cn/gtbczohsop.html

Ruby: ENV["HOME"]
来源：http://hz.yuanzhike.top/gtjtgqzjrm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hammf.cn/gtvxaxubto.html

[M03] 执行外部命令
来源：http://hz.zhiwuduotai.top/gtvrxopfkg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jyoumei.cn/gttezqywkl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yj20258888.top/gtybqkxfag.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jyoumei.cn/gtxbkvsjbo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhengqikj.top/gtztieavmk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj202588.top/gtiegjjknj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.snrcjt.cn/gtwhjkazpf.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.pengpengdd.cyou/gttuccdmaz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.mhx1999.top/gtbgrkfygi.html

[M04] 获取当前工作目录
来源：http://hz.xziqi.cn/gtryiaybro.html

Py:   os.getcwd()
来源：http://hz.sufxvd.cn/gtrglpumgf.html

PHP:  getcwd();
来源：http://hz.ydzc1.top/gttmrwynub.html

JS:   process.cwd()
来源：http://hz.yj20258.top/gtufyadbae.html

TS:   process.cwd()
来源：http://hz.vqdsnc.cn/gtdejaszqf.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xuetiantiany.cn/gtedulwyzz.html

Go:   os.Getwd()
来源：http://hz.zdqjudy.top/gtjoyeilaz.html

Ruby: Dir.pwd
来源：http://hz.ybcxt.top/gtgevzmxem.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhoulong.xyz/gttzdgexiq.html

[M05] 设置退出码
来源：http://hz.hammf.cn/gtclprgpyf.html

Py:   sys.exit(1)
来源：http://hz.cheryme.top/gtbvjdcqgj.html

PHP:  exit(1);
来源：http://hz.tanke756.top/gtzxgehibw.html

JS:   process.exit(1)
来源：http://hz.aizwys.cn/gtrzwlzzqi.html

TS:   process.exit(1)
来源：http://hz.nwbrower.top/gtdbjuhoxx.html

Java: System.exit(1)
来源：http://hz.hfpthk.cn/gtpypfgfep.html

Go:   os.Exit(1)
来源：http://hz.sysykeji.top/gtxmqnnsli.html

Ruby: exit 1
来源：http://hz.xziqi.cn/gtqtrirwlq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yonumen.top/gtyuycgzjf.html

[M06] 向标准错误输出
来源：http://hz.gotoacloud.top/gtiggfhxpp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.meibo888.top/gtpukraqds.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gaohongyu789.top/gtdyvpffae.html

JS:   console.error("err")
来源：http://hz.shanyushiyangtech.top/gtziczging.html

TS:   console.error("err")
来源：http://hz.tian-w.cn/gtciwbktzc.html

Java: System.err.println("err")
来源：http://hz.tianlin.xyz/gtodphtqdl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xuetiantiany.cn/gtwmktnkvd.html

Ruby: warn "err"
来源：http://hz.hysaishi.cn/gtiysortsp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yanxiufei.cn/gtofsacjgd.html

[M07] 判断是否为主入口
来源：http://hz.cashguo.top/gtgititufe.html

Py:   if __name__ == "__main__":
来源：http://hz.cucudq.cn/gtdndnvgfg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ywan-chungtsiang.top/gtlcykdmeh.html

JS:   require.main === module
来源：http://hz.316326.xyz/gtougnhseb.html

TS:   require.main === module
来源：http://hz.birdmap.top/gtlntvggdz.html

Java: public static void main(String[] args)
来源：http://hz.guowangkeji.top/gtxctpuzko.html

Go:   func main()
来源：http://hz.gogol.net.cn/gtnwihyjdx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.nwbrower.top/gtuqqhewah.html

C#:   static void Main(string[] args)
来源：http://hz.tanke756.top/gtlxpruzhd.html

[M08] 获取系统与运行时信息
来源：http://hz.yj20258888.top/gtwokqvqln.html

Py:   platform.system();  platform.python_version()
来源：http://hz.c1oappe.top/gteuocqmdw.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yj20258.top/gthjgavxot.html

JS:   process.platform;  process.version
来源：http://hz.hnqzz.top/gtthyxylkt.html

TS:   process.platform;  process.version
来源：http://hz.chenzaomai.com/gtmwwsouaz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cdnleiting.top/gtzalmpjmp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.fzhhl.top/gtciaglgkk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xuetiantiany.cn/gtgznntmql.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ydjk.org.cn/gtzocwovgz.html

================================================================================
来源：http://hz.jqgfzy.top/gtaoskujie.html

N. 数据结构与算法
来源：http://hz.tanke756.top/gtqxwuloha.html

================================================================================
来源：http://hz.shzxlz.cn/gtxcuhlskn.html

[N01] 二分查找（有序数组）
来源：http://hz.zhixingplan.top/gtxqtladhj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.snrcjt.cn/gtjbmtvtxt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sweek.top/gtficfnuou.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhixingplan.top/gtlsqnslzj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zycfv.cn/gtkzounofh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ydzc1.top/gtqlgwupsj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yuxming.cn/gtchmaoreh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hnqzz.top/gtdzmwekdq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.meibo888.top/gttrbvdxnx.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.nwbrower.top/gtdzntyyct.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.birdmap.top/gtwbgmvppz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.redwolf501.top/gtjtluvgxg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yongpay.top/gtuiqbwyva.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtscynzfvg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yj202588.top/gttfllfaku.html

Go:   slices.Sort(arr)
来源：http://hz.fengsongda.top/gtplcuqkyg.html

Ruby: arr.sort
来源：http://hz.daxiang520.top/gtctosphwa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.pycfn.com/gtxwqgwhqm.html

[N03] 快速排序（分治示例）
来源：http://hz.gzhubu.top/gtziootjic.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.tian-w.cn/gtpzrnayts.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yj20258888.top/gtwtnmeiva.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aizwys.cn/gtykzdpsru.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.316326.xyz/gtgegrrogq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yuxming.cn/gtybyebzvj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shanyushiyangkeji.top/gtfchuipzy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.nanxuanxn.top/gtfehhzxhe.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tian-w.cn/gtkyntyifm.html

[N04] 斐波那契数列
来源：http://hz.vqdsnc.cn/gtssigyius.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xylfe.cn/gtgnmeqwva.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cashguo.top/gtehklkzkw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.svipenyu.cn/gtugadepfc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cdnleiting.top/gtfbjxzjaf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.0kj1m.cn/gtqainqfdf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.svipenyu.cn/gtoonkbbbb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinyuanbaomall.cn/gtuyarsuxw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sxryk.cn/gtlhljzabn.html

[N05] 最大公约数
来源：http://hz.jinyuanbaomall.cn/gtxtbhlkzh.html

Py:   math.gcd(a, b)
来源：http://hz.kuanghao11.cn/gtprixklpx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yj20258.top/gtvnqhqapl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangdashe.top/gtfezrzutv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhijiandao.cn/gtvjkrkloe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xingfuxueyuan.xyz/gtdblukyol.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.wangshuangyany.cn/gtciigmpim.html

Ruby: a.gcd(b)
来源：http://hz.gogol.net.cn/gtecpgybvl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinqigufen.top/gtwnulaxmq.html

[N06] 判断回文字符串
来源：http://hz.aibaodan.cn/gtmeesegka.html

Py:   s == s[::-1]
来源：http://hz.andypj.xyz/gttsxihjbp.html

PHP:  $s === strrev($s);
来源：http://hz.zhongyouzk.top/gtgazxmtiu.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jinqigufen.top/gtaegdmlxw.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shuidangran.top/gtaesbdeug.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinghuilouyu.cn/gtfxwwudbm.html

Go:   // 双指针从两端比较
来源：http://hz.jianghu66.top/gtfzlisuao.html

Ruby: s == s.reverse
来源：http://hz.nwbrower.top/gteroqukia.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cdnleiting.top/gtprtozmfr.html

[N07] 两数之和（返回下标）
来源：http://hz.yonumen.top/gttcmixzfd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nwbrower.top/gtdbniyllp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yonumen.top/gtujbgmbco.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.guowangkeji.top/gtltqoqsxx.html

TS:   // 手写 Map<string, number>
来源：http://hz.daxiang520.top/gtuhsysyje.html

Java: // 手写 HashMap
来源：http://hz.jqgfzy.top/gtlijmiinv.html

Go:   // 手写 map[int]int
来源：http://hz.52xcode.cn/gtdkxxzzsh.html

Ruby: // 手写 Hash
来源：http://hz.yuanzhike.top/gtqcwtyndd.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.feifeiyinyue.top/gtwwdzfhdy.html

[N08] 生成全排列
来源：http://hz.mhx1999.top/gtgmyhfwqb.html

Py:   itertools.permutations(arr)
来源：http://hz.pengpengdd.cyou/gtqnowryix.html

PHP:  // 手写递归交换
来源：http://hz.jqgfzy.top/gthruukvgt.html

JS:   // 手写回溯递归
来源：http://hz.yonumen.top/gtmybohuec.html

TS:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gtvyzchvwb.html

Java: // 手写回溯递归
来源：http://hz.zhongyouzk.top/gtoeaieobq.html

Go:   // 手写回溯递归
来源：http://hz.guowangkeji.top/gtalgvprji.html

Ruby: arr.permutation.to_a
来源：http://hz.zhijiandao.cn/gtamufdwij.html

C#:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtvjxgkzbi.html

[N09] 栈与队列
来源：http://hz.ydjk.org.cn/gttnwefnbe.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.c1oappe.top/gtgjlfbtzy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinqigufen.top/gtfakufsiy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.wangdashe.top/gtkirnsigu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ydzc1.top/gtsjcpulld.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yangfankeji.com/gtxzwvjxax.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.chenlongwang.top/gtauuxzduy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.tianlin.xyz/gtkqkmxqnr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jlsjyb.cn/gtswxhmtly.html

[N10] 链表节点定义
来源：http://hz.hysaishi.cn/gtcuufnxjn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hysaishi.cn/gticwxfisv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gogol.net.cn/gtomybhvmr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhongyouzk.top/gtrscgkzdr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cheryme.top/gthuzjafnv.html

Java: class Node { int v; Node next; }
来源：http://hz.nanxuanxn.top/gtstvzjdsd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.bjfxy.top/gtmdsxktog.html


<!-- 参考信息 -->