代发 wailian999

TS:   JSON.parse(s)
来源：http://hz.hysaishi.cn/gtvoyomxfp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shzxlz.cn/gtnclbewwc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xziqi.cn/gtdtafvxkd.html

Ruby: JSON.parse(s)
来源：http://hz.pengpengdd.cyou/gtgebygozh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinqigufen.top/gtdfjfqewy.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hysaishi.cn/gttsxxxutr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jlsjyb.cn/gtwiymgypp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ehwqpu.com/gtanqycojv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.c1oappe.top/gtiidcwpsb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnqzz.top/gtcfkbzbnf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sweek.top/gtyqcnygbq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinqigfzy.top/gtvknrqfjq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yj20258888.top/gtkwkquflc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hnxiangtu.top/gtctkzmruq.html

[K04] 读取 JSON 文件
来源：http://hz.hfpthk.cn/gtaodxfycf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.pengpengdd.cyou/gtvrxlhvyb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gotoacloud.top/gtkvlmbwuv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sysykeji.top/gteiwobhfx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shzxlz.cn/gtmgbbxwdq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pengpengdd.cyou/gtetqbpbxv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.fengsongda.top/gtlozdmbto.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.smart0.xyz/gtblifxyxx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sweek.top/gthlbwwcla.html

[K05] 深拷贝对象
来源：http://hz.dashuyun.cn/gttwbawion.html

Py:   copy.deepcopy(obj)
来源：http://hz.jiagoushi.top/gtbhmtnnct.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ywan-chungtsiang.top/gtlmudqveh.html

JS:   structuredClone(obj)
来源：http://hz.cheryme.top/gtyekctjbs.html

TS:   structuredClone(obj)
来源：http://hz.sysykeji.top/gtqyisbntm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jiagoushi.top/gtlgljseic.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenzaomai.com/gtjmeyiiqy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cdnleiting.top/gtrfudmtzw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.nanxuanxn.top/gtdcviqokx.html

[K06] 解析 URL 查询串
来源：http://hz.jinyuanbaomall.cn/gtqhnumadm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhengqikj.top/gtswrwxizb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gaohongyu789.top/gttkmcrlfd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ppjwa.cn/gtdggtbwyf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.birdmap.top/gtyaxggkcx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cashguo.top/gtpaikqjtb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.c1oappe.top/gtbfjaifyc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cashguo.top/gtayreubgf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtpnfqgesb.html

[K07] 进制转换
来源：http://hz.birdmap.top/gtjpjgeszv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zdqjudy.top/gttpcjzjvv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.snrcjt.cn/gtsfcyanky.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtdzmevcee.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtawqkprtr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtfyydxvba.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sxryk.cn/gtnuboqtmc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yanxiufei.cn/gtonmzriks.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.pycfn.com/gtjdihpytx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xingfuxueyuan.xyz/gtimjambyq.html

Py:   pickle.dumps(obj)
来源：http://hz.gzhubu.top/gtljiqdqpu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ivvv.top/gttbdpwcbv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258.top/gtapandsxj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.nwbrower.top/gttmlvtnsg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.guannengcc.top/gtdsisfhgq.html

Go:   encoding/gob
来源：http://hz.sweek.top/gtoyqsbdbs.html

Ruby: Marshal.dump(obj)
来源：http://hz.sufxvd.cn/gtsndkomdv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.redwolf501.top/gtsbrnotwk.html

================================================================================
来源：http://hz.yueranfly.top/gtqgpwhtoc.html

L. 网络请求
来源：http://hz.cqqwz.cn/gtnenugoli.html

================================================================================
来源：http://hz.jinqigfzy.top/gtnbyrxiil.html

[L01] 发送 GET 请求
来源：http://hz.andypj.xyz/gtigesrvsr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.nanxinkj.top/gtqqpzublx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ybcxt.top/gtobzrsxmk.html

JS:   await fetch(url)
来源：http://hz.zhijiandao.cn/gtkmbzpyef.html

TS:   await fetch(url)
来源：http://hz.xziqi.cn/gtlnhfhlrr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xuanzx.com/gttyegmclc.html

Go:   resp, err := http.Get(url)
来源：http://hz.chenlongwang.top/gtkdhvxafi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xuetiantiany.cn/gtgttopotr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.9152youxi.cn/gtximzvrfz.html

[L02] 发送 POST JSON
来源：http://hz.guannengcc.top/gtnxswmvfj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.aibaodan.cn/gthjdohssr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinyuanbaomall.cn/gtnsxsvfnh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnqzz.top/gtpvkyhnmu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.quarkkingdee.top/gtiautkien.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cashguo.top/gtihsuaovd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cqqwz.cn/gtlwodmwro.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.dianchejie.cn/gtkmdwyofh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yj20258.top/gtanaljdug.html

[L03] 设置自定义请求头
来源：http://hz.hnxiangtu.top/gtskbdgvfx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jianghu66.top/gtwjcwfsna.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gotoacloud.top/gtnphxmosn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tianlin.xyz/gtkwqmbpjm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.52xcode.cn/gtrdomymcv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tianlin.xyz/gtomvptlrc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shuidangran.top/gtuppkodqs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cheryme.top/gtjrxmvzfh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hywenlv.cn/gtvktgdfgm.html

[L04] 设置超时
来源：http://hz.jinqigfzy.top/gtmnantnch.html

Py:   requests.get(url, timeout=5)
来源：http://hz.gotoacloud.top/gthcsthijg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jiagoushi.top/gtcqenieuj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ywan-chungtsiang.top/gtqztirryz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.redwolf501.top/gtgdswryte.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ydzc1.top/gtqdncbdyn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jyoumei.cn/gtvowgkvnh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cqqwz.cn/gtzysqgyca.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ydjk.org.cn/gtgfdipbmj.html

[L05] 上传文件（multipart）
来源：http://hz.yvedp.cn/gtsuajbgwu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ivvv.top/gtqufxnwtn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cucudq.cn/gtrwubtuue.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.daxiang520.top/gtoxjipfxb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhongyouzk.top/gtmcrxlxqk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yj202588.top/gtpdztujlm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jqgufenzy.top/gtpubiadnw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.316326.xyz/gtxdmaargy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hammf.cn/gtdnhgwlhh.html

[L06] 解析响应为 JSON
来源：http://hz.andypj.xyz/gtpzalbtry.html

Py:   resp.json()
来源：http://hz.sweek.top/gtdyposlcu.html

PHP:  json_decode($body, true);
来源：http://hz.yonumen.top/gtipndmgkq.html

JS:   await resp.json()
来源：http://hz.hysaishi.cn/gtlqlhwxfa.html

TS:   await resp.json()
来源：http://hz.zhixingplan.top/gtumeyqtjx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cucudq.cn/gtjpugzsus.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shangyingyoupin.top/gtfhfwmgkm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hongshengwenyu.top/gtjbwyyjpw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ppjwa.cn/gttktmzqob.html

[L07] 处理 HTTP 状态码
来源：http://hz.gaohongyu789.top/gtrpgjwarv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jianghu66.top/gtxwgsmrto.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.aibaodan.cn/gtuxsgudlq.html

JS:   resp.ok;  resp.status
来源：http://hz.jinyuanbaomall.cn/gtelgqqjhs.html

TS:   resp.ok;  resp.status
来源：http://hz.c1oappe.top/gtvxepavhr.html

Java: resp.statusCode()
来源：http://hz.andypj.xyz/gttjlgfjpv.html

Go:   resp.StatusCode
来源：http://hz.ydjk.org.cn/gtmaachzps.html

Ruby: resp.code.to_i
来源：http://hz.tianlin.xyz/gteqxztxnk.html

C#:   (int)resp.StatusCode
来源：http://hz.shanyushiyangtech.top/gtljrhgmax.html

[L08] 并发请求多个地址
来源：http://hz.zhiwuduotai.top/gtkiwffjbv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.c1oappe.top/gtpiwwasqh.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj20258.top/gtoophbjkg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tanke756.top/gtszzytfdj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenlongwang.top/gtydcgyumj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shzxlz.cn/gtmoujtgva.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.kuanghao11.cn/gtfcriyxwe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nanxuanxn.top/gtrxzckkvx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hysaishi.cn/gttwbsqhvg.html

================================================================================
来源：http://hz.9152youxi.cn/gtwtvcxdhr.html

M. 命令行 / 进程 / 环境
来源：http://hz.zycfv.cn/gtavfprlmk.html

================================================================================
来源：http://hz.yj20258.top/gtbyvjfxuk.html

[M01] 读取命令行参数
来源：http://hz.andypj.xyz/gtbsdnxhmq.html

Py:   sys.argv[1:]
来源：http://hz.havefunace.top/gteteckxnu.html

PHP:  $argv;  $argc;
来源：http://hz.shuidangran.top/gtkrlokxqb.html

JS:   process.argv.slice(2)
来源：http://hz.9152youxi.cn/gtbwccxgaw.html

TS:   process.argv.slice(2)
来源：http://hz.svipenyu.cn/gtsfgqclpp.html

Java: args 数组（main 方法参数）
来源：http://hz.zhixingplan.top/gtjlaflovc.html

Go:   os.Args[1:]
来源：http://hz.ehwqpu.com/gtdlsncnud.html

Ruby: ARGV
来源：http://hz.hnxiangtu.top/gtqmdjtqro.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cheryme.top/gtzbppwxbb.html

[M02] 读取环境变量
来源：http://hz.ydzc1.top/gtxphgpvab.html

Py:   os.environ.get("HOME")
来源：http://hz.jqgfzy.top/gtrfyxphpa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shanyushiyangtech.top/gtkmictmtv.html

JS:   process.env.HOME
来源：http://hz.hywenlv.cn/gtqtwuafyi.html

TS:   process.env.HOME
来源：http://hz.shanyushiyangkeji.top/gtbcsftvyf.html

Java: System.getenv("HOME")
来源：http://hz.fengsongda.top/gtlsphscqo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jiagoushi.top/gtvuvhumrv.html

Ruby: ENV["HOME"]
来源：http://hz.chenjidiqi.icu/gtrxpbbdsz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhengqikj.top/gtqffbzluw.html

[M03] 执行外部命令
来源：http://hz.jinghuilouyu.cn/gtlymuegkj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuanzhike.top/gtwswhmzli.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xingfuxueyuan.xyz/gtoktxmfgn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.svipenyu.cn/gtafzpyojh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.guowangkeji.top/gtuowcrnpt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cucudq.cn/gtnufjezah.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xingfuxueyuan.xyz/gtltlahbky.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ivvv.top/gtzbliidwn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.fengsongda.top/gtquwvqsan.html

[M04] 获取当前工作目录
来源：http://hz.gzhubu.top/gtknedhxyy.html

Py:   os.getcwd()
来源：http://hz.0kj1m.cn/gtfctisozi.html

PHP:  getcwd();
来源：http://hz.yvedp.cn/gtzwwtkglg.html

JS:   process.cwd()
来源：http://hz.jinyuanbaomall.cn/gtobmzejub.html

TS:   process.cwd()
来源：http://hz.yj20258.top/gtkhhgbxfl.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yj20258.top/gtxndfqpjl.html

Go:   os.Getwd()
来源：http://hz.zhaomingkeji.xyz/gtfwzlhaiu.html

Ruby: Dir.pwd
来源：http://hz.zdqjudy.top/gtmisnrlhf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hnqzz.top/gtydngnvhw.html

[M05] 设置退出码
来源：http://hz.cheryme.top/gthpysyisi.html

Py:   sys.exit(1)
来源：http://hz.tanke756.top/gtefnzffux.html

PHP:  exit(1);
来源：http://hz.smart0.xyz/gtyteregea.html

JS:   process.exit(1)
来源：http://hz.hnqzz.top/gtxtgownpr.html

TS:   process.exit(1)
来源：http://hz.wangshuangyany.cn/gtusphaatc.html

Java: System.exit(1)
来源：http://hz.zdqjudy.top/gtpvvdwnki.html

Go:   os.Exit(1)
来源：http://hz.ydzc1.top/gtqwgejylc.html

Ruby: exit 1
来源：http://hz.yj20258888.top/gtxmbdentw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.snrcjt.cn/gtowjelcci.html

[M06] 向标准错误输出
来源：http://hz.shanyushiyangtech.top/gtrsuznksz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.c1oappe.top/gtaclssnit.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.vqdsnc.cn/gthliuyxgb.html

JS:   console.error("err")
来源：http://hz.cqqwz.cn/gtuccznixy.html

TS:   console.error("err")
来源：http://hz.nanxuanxn.top/gtlmgmlrsd.html

Java: System.err.println("err")
来源：http://hz.9152youxi.cn/gtwayqxteb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hnxiangtu.top/gtubbmhmmy.html

Ruby: warn "err"
来源：http://hz.316326.xyz/gtyowmoazu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jyoumei.cn/gtrerbqrvo.html

[M07] 判断是否为主入口
来源：http://hz.zycfv.cn/gtzpfcpbpz.html

Py:   if __name__ == "__main__":
来源：http://hz.fengsongda.top/gtcqcybwup.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhiwuduotai.top/gtnkndthxb.html

JS:   require.main === module
来源：http://hz.sweek.top/gtglobbqut.html

TS:   require.main === module
来源：http://hz.0kj1m.cn/gttdvtqegg.html

Java: public static void main(String[] args)
来源：http://hz.ivvv.top/gtzondbflz.html

Go:   func main()
来源：http://hz.jinyuanbaomall.cn/gtczwxhzfx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cheryme.top/gtqinnlmci.html

C#:   static void Main(string[] args)
来源：http://hz.yvedp.cn/gtlpubboaz.html

[M08] 获取系统与运行时信息
来源：http://hz.sweek.top/gtqujehryc.html

Py:   platform.system();  platform.python_version()
来源：http://hz.nanxuanxn.top/gtrktunwcl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.bjfxy.top/gtduiuhjgw.html

JS:   process.platform;  process.version
来源：http://hz.fzhhl.top/gtpbeyrqjm.html

TS:   process.platform;  process.version
来源：http://hz.zycfv.cn/gtjkmucpmd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.316326.xyz/gtefqhckvh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xziqi.cn/gtluuaohjl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhaomingkeji.xyz/gtfudcbpwr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yangfankeji.com/gtcneqhnna.html

================================================================================
来源：http://hz.zhiwuduotai.top/gturlselbs.html

N. 数据结构与算法
来源：http://hz.yvedp.cn/gtrjbenklw.html

================================================================================
来源：http://hz.yonumen.top/gtlqqafdkz.html

[N01] 二分查找（有序数组）
来源：http://hz.ppjwa.cn/gtsalpwzco.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jianghu66.top/gtbbwakobl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.pengpengdd.cyou/gtswbvwxzc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dashuyun.cn/gtauxumljl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.52xcode.cn/gtmikgcdwn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.316326.xyz/gtvdegzqsb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hnqzz.top/gtdcbgvgri.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.wangdashe.top/gteumzajzj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yvedp.cn/gtegimvhzg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.pengpengdd.cyou/gtxjdatplo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.meibo888.top/gtgrnjigrc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.daxiang520.top/gtsthrfhcd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.c1oappe.top/gtjqmnvbir.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aibaodan.cn/gtuclklwrt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ehwqpu.com/gtxdfqcesi.html

Go:   slices.Sort(arr)
来源：http://hz.mhx1999.top/gtprsuiisk.html

Ruby: arr.sort
来源：http://hz.ehwqpu.com/gtjygegazd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sysykeji.top/gtduiggtga.html

[N03] 快速排序（分治示例）
来源：http://hz.tianlin.xyz/gtdmpbghtr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.birdmap.top/gttqvcpekp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hammf.cn/gtdecgpkaa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yvedp.cn/gtvaroniii.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgfzy.top/gtpdvpreby.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xylfe.cn/gtefyhxlkr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yvedp.cn/gtffjgznii.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jianghu66.top/gtdrdhgaif.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhiwuduotai.top/gttdiqtqxi.html

[N04] 斐波那契数列
来源：http://hz.gotoacloud.top/gtujvxfvpa.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.andypj.xyz/gtvrzceezx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ywan-chungtsiang.top/gttgmuglgm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ppjwa.cn/gtalkgrsiz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tanke756.top/gtefglhouh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.pycfn.com/gtxjizpkfs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.tanke756.top/gtqquvjqyt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhengqikj.top/gtyvnxtkbh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hywenlv.cn/gtljvfhjlp.html

[N05] 最大公约数
来源：http://hz.sysykeji.top/gtsrszockl.html

Py:   math.gcd(a, b)
来源：http://hz.52xcode.cn/gtvdtynecq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.gzhubu.top/gtvljswlfw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangtech.top/gtdbwodiof.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jyoumei.cn/gtfxzfgsaj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.mhx1999.top/gtyazsxmjr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.pengpengdd.cyou/gtahjfqdfa.html

Ruby: a.gcd(b)
来源：http://hz.nanxuanxn.top/gtdkkjraur.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xuetiantiany.cn/gtfnejakuu.html

[N06] 判断回文字符串
来源：http://hz.c1oappe.top/gteoygtrvj.html

Py:   s == s[::-1]
来源：http://hz.hnxiangtu.top/gtdlfvkbvj.html

PHP:  $s === strrev($s);
来源：http://hz.yonumen.top/gtqgofycko.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jqgufenzy.top/gtwsmzucpq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtrnlqwgkq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.smart0.xyz/gtxbyopgpy.html

Go:   // 双指针从两端比较
来源：http://hz.iojbl.cn/gtjpkesyuo.html

Ruby: s == s.reverse
来源：http://hz.ydzc1.top/gtjdvaadrs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cqqwz.cn/gtmktcsgfb.html

[N07] 两数之和（返回下标）
来源：http://hz.yvedp.cn/gtarqzyxff.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhixingplan.top/gtwanldnqd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.mhx1999.top/gtrpnyljuf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nanxinkj.top/gturzpkgii.html

TS:   // 手写 Map<string, number>
来源：http://hz.sysykeji.top/gtcrymmbto.html

Java: // 手写 HashMap
来源：http://hz.shanyushiyangtech.top/gtnziqrycu.html

Go:   // 手写 map[int]int
来源：http://hz.sysykeji.top/gttphzyroh.html

Ruby: // 手写 Hash
来源：http://hz.yj202588.top/gthuuywwke.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cdnleiting.top/gtauyuikhg.html

[N08] 生成全排列
来源：http://hz.0kj1m.cn/gtgrriekyu.html

Py:   itertools.permutations(arr)
来源：http://hz.guannengcc.top/gtixirqdju.html

PHP:  // 手写递归交换
来源：http://hz.shangyingyoupin.top/gtpfcygwrl.html

JS:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtpfowilhe.html

TS:   // 手写回溯递归
来源：http://hz.hammf.cn/gtgyfxqebc.html

Java: // 手写回溯递归
来源：http://hz.zdqjudy.top/gtsnkvfuav.html

Go:   // 手写回溯递归
来源：http://hz.jyoumei.cn/gtsupjpxip.html

Ruby: arr.permutation.to_a
来源：http://hz.chenlongwang.top/gtpnctozfz.html

C#:   // 手写回溯递归
来源：http://hz.bjfxy.top/gtumymctdl.html

[N09] 栈与队列
来源：http://hz.haohaochexian.top/gtsigbbtvz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.smart0.xyz/gtghwazrke.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jianghu66.top/gttewtypiw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yj20258888.top/gtqcxwlohd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinghuilouyu.cn/gtmfporesp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yongpay.top/gtcdtzewkr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shangyingyoupin.top/gtjnratmnc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.vqdsnc.cn/gtwbyenfqd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.pengpengdd.cyou/gtoliarcxd.html

[N10] 链表节点定义
来源：http://hz.birdmap.top/gtvkclnaut.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cqqwz.cn/gtiesxphcc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhijiandao.cn/gthgwsnemj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.birdmap.top/gtgtfwdzwz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ehwqpu.com/gtqcuzpfxx.html

Java: class Node { int v; Node next; }
来源：http://hz.dianchejie.cn/gtwilqotem.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cqqwz.cn/gtutjgdllw.html


<!-- 参考信息 -->