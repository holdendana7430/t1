代发 wailian999

TS:   JSON.parse(s)
来源：http://hz.sufxvd.cn/gtdooeaiir.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.havefunace.top/gtwqgrvphm.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cqqwz.cn/gtucelewxe.html

Ruby: JSON.parse(s)
来源：http://hz.ydzc1.top/gttangwsrv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinqigufen.top/gtqicoualf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cashguo.top/gtcqmtszeq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yuxming.cn/gtusyucgjg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.iojbl.cn/gtqhqbnpzk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydjk.org.cn/gtxcbnwqsp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tian-w.cn/gtpcsalsiv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.smart0.xyz/gtiqchczri.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.dashuyun.cn/gtkolwvxeh.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.meibo888.top/gtjyjukxbx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hysaishi.cn/gtdojkacpk.html

[K04] 读取 JSON 文件
来源：http://hz.hfpthk.cn/gtxcmotdkq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.0kj1m.cn/gtnpqqzsiy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shanyushiyangkeji.top/gtyfwbhtfi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xuetiantiany.cn/gtvmniejrp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhengqikj.top/gtbqanjqjj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xingfuxueyuan.xyz/gtgsaonwfe.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jlsjyb.cn/gtoomjmoin.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.andypj.xyz/gtgufjssey.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tianlin.xyz/gtzwsslrdl.html

[K05] 深拷贝对象
来源：http://hz.hongshengwenyu.top/gtysgspahl.html

Py:   copy.deepcopy(obj)
来源：http://hz.redwolf501.top/gtaeppmurw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.vqdsnc.cn/gtzgtcqkbq.html

JS:   structuredClone(obj)
来源：http://hz.fengsongda.top/gtokgnmavv.html

TS:   structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gtbhyaifgp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.havefunace.top/gtdrmktefd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj20258888.top/gtugzqoxzo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hnxiangtu.top/gtrxjidxbr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.smart0.xyz/gtlpfkyjev.html

[K06] 解析 URL 查询串
来源：http://hz.cdnleiting.top/gttvrnbznw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yongpay.top/gtfgxkkrbk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.fengsongda.top/gtxatxlfxk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258.top/gtuudpqhjz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aizwys.cn/gtjnezhrhd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xylfe.cn/gtdemlduwd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gotoacloud.top/gttucqbfej.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.guannengcc.top/gtpvoteebo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yj202588.top/gtilbiwfzx.html

[K07] 进制转换
来源：http://hz.gaohongyu789.top/gtygnfzpus.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sweek.top/gtotuekfon.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yueranfly.top/gtjvooidyd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gtgmkmlcdx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.quarkkingdee.top/gtzuyyrxdp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gtmuyzcxvb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.0kj1m.cn/gthjazxxlb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.svipenyu.cn/gtblvptiwg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yongpay.top/gtrlpuaadd.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.c1oappe.top/gtwlhhtlay.html

Py:   pickle.dumps(obj)
来源：http://hz.guannengcc.top/gtxgsvpfce.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.svipenyu.cn/gtsikyiriw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinyuanbaomall.cn/gtxkqulkns.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.fzhhl.top/gtovscskjk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ivvv.top/gtrfjiomwv.html

Go:   encoding/gob
来源：http://hz.cheryme.top/gtotxunyae.html

Ruby: Marshal.dump(obj)
来源：http://hz.nwbrower.top/gtsclyhvdm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cucudq.cn/gtobarjwpc.html

================================================================================
来源：http://hz.xziqi.cn/gtjgepjots.html

L. 网络请求
来源：http://hz.andypj.xyz/gtjnhnszmq.html

================================================================================
来源：http://hz.chenzaomai.com/gtnkygepes.html

[L01] 发送 GET 请求
来源：http://hz.hfpthk.cn/gtjcaallxz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shanyushiyangkeji.top/gtmslekxms.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ywan-chungtsiang.top/gtsanedssk.html

JS:   await fetch(url)
来源：http://hz.zhiwuduotai.top/gtxbfujzxr.html

TS:   await fetch(url)
来源：http://hz.sufxvd.cn/gtvzcrzxkd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.316326.xyz/gtfyeuagac.html

Go:   resp, err := http.Get(url)
来源：http://hz.kuanghao11.cn/gtapvbeqsv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hnqzz.top/gtdpxbfkxj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jlsjyb.cn/gtlwmbugxa.html

[L02] 发送 POST JSON
来源：http://hz.meibo888.top/gtpchjhqyd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yueranfly.top/gterhhwreg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xuanzx.com/gtsltzhxdm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guannengcc.top/gtxawnozau.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jlsjyb.cn/gtadwxjmpt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhaomingkeji.xyz/gtashftqui.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.mhx1999.top/gthetdrsjl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xuanzx.com/gtigilfcuj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shuidangran.top/gtgvoukxhq.html

[L03] 设置自定义请求头
来源：http://hz.yuxming.cn/gtqrhwsuid.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.shzxlz.cn/gtbqkbvsos.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gogol.net.cn/gteitikhul.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pycfn.com/gtkjpnzknu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.316326.xyz/gtstazccfi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sweek.top/gtyvwzwnea.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.316326.xyz/gtqhekrxmz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.havefunace.top/gtymqhppde.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yueranfly.top/gtyeylcafx.html

[L04] 设置超时
来源：http://hz.ydzc1.top/gttrvhmuad.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yonumen.top/gtytstgkdp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.redwolf501.top/gtdpusjdze.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.feifeiyinyue.top/gttklygeao.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dianchejie.cn/gtdzzjedsw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ydjk.org.cn/gtwepkqgnf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cashguo.top/gtobeeewgx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.chenjidiqi.icu/gtrjsifnxk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ivvv.top/gtcwddzmcs.html

[L05] 上传文件（multipart）
来源：http://hz.yangfankeji.com/gtdatumdhe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.guannengcc.top/gtyjjuhmfm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.pycfn.com/gtqdiqefzz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zycfv.cn/gtkowgzyod.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zycfv.cn/gtwijlvkvy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sufxvd.cn/gtmuozxygq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinqigfzy.top/gtoslhsysn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yj20258888.top/gtssnmpcib.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gogol.net.cn/gtkxvzpszk.html

[L06] 解析响应为 JSON
来源：http://hz.0kj1m.cn/gtviekfhvt.html

Py:   resp.json()
来源：http://hz.zhiwuduotai.top/gtqfcomcil.html

PHP:  json_decode($body, true);
来源：http://hz.andypj.xyz/gttybsotrx.html

JS:   await resp.json()
来源：http://hz.snrcjt.cn/gtzuqvdmjp.html

TS:   await resp.json()
来源：http://hz.feifeiyinyue.top/gtpgprragu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.c1oappe.top/gthzknzpar.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.316326.xyz/gtrlbkznkh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xziqi.cn/gtgnugtclj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.pycfn.com/gtztziavcp.html

[L07] 处理 HTTP 状态码
来源：http://hz.yangfankeji.com/gtienmdmpu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.pengpengdd.cyou/gtwboifefn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj20258888.top/gtchkrobcp.html

JS:   resp.ok;  resp.status
来源：http://hz.cdnleiting.top/gtugtahsrq.html

TS:   resp.ok;  resp.status
来源：http://hz.tian-w.cn/gtvvwegdum.html

Java: resp.statusCode()
来源：http://hz.chenzaomai.com/gtiqbkzvrs.html

Go:   resp.StatusCode
来源：http://hz.zhaomingkeji.xyz/gtbyxtrzkf.html

Ruby: resp.code.to_i
来源：http://hz.aibaodan.cn/gtxuowxhop.html

C#:   (int)resp.StatusCode
来源：http://hz.ybcxt.top/gtenawosop.html

[L08] 并发请求多个地址
来源：http://hz.daria6918.cn/gteuqcyuxo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.bjfxy.top/gtrhsdxzun.html

PHP:  curl_multi_init() 系列
来源：http://hz.fzhhl.top/gtdwgypxyd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ybcxt.top/gtfamsiioz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.bjfxy.top/gtnchfuoap.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.pycfn.com/gtljrtkkea.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.nanxinkj.top/gtfryopvuz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.guowangkeji.top/gtkbvuxdem.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhixingplan.top/gtdbsysvee.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtrvopzjeo.html

M. 命令行 / 进程 / 环境
来源：http://hz.smart0.xyz/gtdkuuptea.html

================================================================================
来源：http://hz.yonumen.top/gtnlmqoxob.html

[M01] 读取命令行参数
来源：http://hz.nanxuanxn.top/gthihphuzk.html

Py:   sys.argv[1:]
来源：http://hz.ywan-chungtsiang.top/gtwaclummz.html

PHP:  $argv;  $argc;
来源：http://hz.zhongyouzk.top/gtshjmbeig.html

JS:   process.argv.slice(2)
来源：http://hz.hnqzz.top/gtedhpnkig.html

TS:   process.argv.slice(2)
来源：http://hz.daria6918.cn/gtkuxcajtd.html

Java: args 数组（main 方法参数）
来源：http://hz.yuxming.cn/gtlrwkfasm.html

Go:   os.Args[1:]
来源：http://hz.jinghuilouyu.cn/gtfztzsbla.html

Ruby: ARGV
来源：http://hz.yuanzhike.top/gtmouxcuhr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cheryme.top/gtqsitbauz.html

[M02] 读取环境变量
来源：http://hz.aibaodan.cn/gtngcimgmw.html

Py:   os.environ.get("HOME")
来源：http://hz.snrcjt.cn/gtdvbvmhpd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ehwqpu.com/gteaxcejsa.html

JS:   process.env.HOME
来源：http://hz.zhiwuduotai.top/gtpjqgtedf.html

TS:   process.env.HOME
来源：http://hz.jyoumei.cn/gttdkefevj.html

Java: System.getenv("HOME")
来源：http://hz.0kj1m.cn/gtqqxuytom.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.haohaochexian.top/gtcobadeid.html

Ruby: ENV["HOME"]
来源：http://hz.cheryme.top/gtlsysfcja.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.iojbl.cn/gtkkikklkk.html

[M03] 执行外部命令
来源：http://hz.zhengqikj.top/gtvuamtpgj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.daxiang520.top/gtvpplozbf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.nanxuanxn.top/gtjciuuuxl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xziqi.cn/gttznkwudp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hywenlv.cn/gtpmxncjzv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yuanzhike.top/gtznnhxnfp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.redwolf501.top/gtguahdgfk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gaohongyu789.top/gtihtvccmx.html

C#:   Process.Start("ls", "-l");
来源：http://hz.mhx1999.top/gtfqxvulgs.html

[M04] 获取当前工作目录
来源：http://hz.jinghuilouyu.cn/gtiuegjtre.html

Py:   os.getcwd()
来源：http://hz.jlsjyb.cn/gtywxanpin.html

PHP:  getcwd();
来源：http://hz.redwolf501.top/gtngwfcghy.html

JS:   process.cwd()
来源：http://hz.ivvv.top/gtrssuemxu.html

TS:   process.cwd()
来源：http://hz.xuanzx.com/gtgsqzfabv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.guowangkeji.top/gtfksbpred.html

Go:   os.Getwd()
来源：http://hz.jqgfzy.top/gtdgtphmkv.html

Ruby: Dir.pwd
来源：http://hz.shanyushiyangkeji.top/gtbnrckrcq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yj202588.top/gtaqdgjqln.html

[M05] 设置退出码
来源：http://hz.c1oappe.top/gtmkfxjnjc.html

Py:   sys.exit(1)
来源：http://hz.chenlongwang.top/gtubtyakwh.html

PHP:  exit(1);
来源：http://hz.gaohongyu789.top/gtpvioeovk.html

JS:   process.exit(1)
来源：http://hz.gogol.net.cn/gtotmdquhq.html

TS:   process.exit(1)
来源：http://hz.sufxvd.cn/gtxpfxorae.html

Java: System.exit(1)
来源：http://hz.nanxinkj.top/gtdohpkcic.html

Go:   os.Exit(1)
来源：http://hz.ivvv.top/gtpdpknkst.html

Ruby: exit 1
来源：http://hz.hfpthk.cn/gtvemurxdw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.feifeiyinyue.top/gtwxcnzkcf.html

[M06] 向标准错误输出
来源：http://hz.mhx1999.top/gttyqvjxsu.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xylfe.cn/gtnyouihtw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shanyushiyangtech.top/gtmrhhycry.html

JS:   console.error("err")
来源：http://hz.ehwqpu.com/gtmnpdjoxq.html

TS:   console.error("err")
来源：http://hz.ppjwa.cn/gtmvgzlnot.html

Java: System.err.println("err")
来源：http://hz.dashuyun.cn/gtmsnqfunp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.redwolf501.top/gtsgnnmmks.html

Ruby: warn "err"
来源：http://hz.pycfn.com/gtuqxmlirn.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.tian-w.cn/gtowmcxazl.html

[M07] 判断是否为主入口
来源：http://hz.chenzaomai.com/gtzjobddiz.html

Py:   if __name__ == "__main__":
来源：http://hz.nanxuanxn.top/gtfrnbjjzw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhaomingkeji.xyz/gteydptuvz.html

JS:   require.main === module
来源：http://hz.gotoacloud.top/gtojdzfaky.html

TS:   require.main === module
来源：http://hz.gotoacloud.top/gtssyvybbp.html

Java: public static void main(String[] args)
来源：http://hz.shanyushiyangtech.top/gtbfrkwpjp.html

Go:   func main()
来源：http://hz.zhixingplan.top/gtjpijmqsz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.daria6918.cn/gtlunknmza.html

C#:   static void Main(string[] args)
来源：http://hz.daxiang520.top/gtjhglghbd.html

[M08] 获取系统与运行时信息
来源：http://hz.hnqzz.top/gtjyjsftyj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shanyushiyangkeji.top/gtqgzeyfoy.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ivvv.top/gtbtvtqdmr.html

JS:   process.platform;  process.version
来源：http://hz.haohaochexian.top/gtmgxavcpr.html

TS:   process.platform;  process.version
来源：http://hz.cheryme.top/gtfofokqek.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.quarkkingdee.top/gtpzhmlodp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yj20258888.top/gtwfxfxpxo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.nwbrower.top/gtkdqwdaqw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj202588.top/gtsndywwpv.html

================================================================================
来源：http://hz.yanxiufei.cn/gtpdtgkhbs.html

N. 数据结构与算法
来源：http://hz.yj202588.top/gtzbjhrjrb.html

================================================================================
来源：http://hz.aibaodan.cn/gtmbhwnwfy.html

[N01] 二分查找（有序数组）
来源：http://hz.bjfxy.top/gtmsoslkis.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.wangshuangyany.cn/gtohgtohct.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ydzc1.top/gtlsawrmje.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tian-w.cn/gtpbeocbbz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sxryk.cn/gtgbfrosbs.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.guowangkeji.top/gtkbjcxrki.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jiagoushi.top/gtezodtjxt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.wangdashe.top/gtjamspojo.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.bjfxy.top/gttdfcpioj.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.snrcjt.cn/gtmzccveyr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tianlin.xyz/gtxmcedaim.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cashguo.top/gtrsjxyjsz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258888.top/gtkbttgcap.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.0kj1m.cn/gtoedzuvpe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yonumen.top/gtqjpqufys.html

Go:   slices.Sort(arr)
来源：http://hz.hywenlv.cn/gtwqifzpyu.html

Ruby: arr.sort
来源：http://hz.xuanzx.com/gtydbznoho.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.wangshuangyany.cn/gthjmdzcll.html

[N03] 快速排序（分治示例）
来源：http://hz.gogol.net.cn/gtvyhnakna.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinghuilouyu.cn/gttsptyont.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gzhubu.top/gtaclpawjf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pengpengdd.cyou/gtcufbqbdr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shangyingyoupin.top/gtgqpstcje.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xinyue.icu/gtezjxpfrt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hywenlv.cn/gtnnpompdl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yongpay.top/gtsnjoutvz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shangyingyoupin.top/gtbfnwyxgr.html

[N04] 斐波那契数列
来源：http://hz.kuanghao11.cn/gtpcwzftlu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.gotoacloud.top/gtnfzhdjfa.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hongshengwenyu.top/gtjelzejdz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yonumen.top/gtgkaxadsu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dianchejie.cn/gthemzemzt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.feifeiyinyue.top/gtyfqtnthb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cucudq.cn/gtcincvvsr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cqqwz.cn/gttyfnvkbg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.bjfxy.top/gtiwaskuoi.html

[N05] 最大公约数
来源：http://hz.yuanzhike.top/gtuqbbitvy.html

Py:   math.gcd(a, b)
来源：http://hz.cdnleiting.top/gtrenhwtif.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.chenzaomai.com/gtcbkqyoss.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gzhubu.top/gtyvloyujh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daria6918.cn/gtkxvtywdo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hfpthk.cn/gttstwqwjr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.snrcjt.cn/gtpgyetbdx.html

Ruby: a.gcd(b)
来源：http://hz.xingfuxueyuan.xyz/gtqehazgxy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gaohongyu789.top/gtbtpbancu.html

[N06] 判断回文字符串
来源：http://hz.sweek.top/gtbtreopfk.html

Py:   s == s[::-1]
来源：http://hz.jinqigufen.top/gtjnauqbmh.html

PHP:  $s === strrev($s);
来源：http://hz.shanyushiyangkeji.top/gtiqywsrda.html

JS:   s === [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtslfjgejq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yuxming.cn/gtgcjirdyh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ehwqpu.com/gtscqtoswg.html

Go:   // 双指针从两端比较
来源：http://hz.jqgfzy.top/gtrbrvetyu.html

Ruby: s == s.reverse
来源：http://hz.0kj1m.cn/gtqishpgyu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yj202588.top/gtkpxeaazi.html

[N07] 两数之和（返回下标）
来源：http://hz.hammf.cn/gtgqisfpnr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.9152youxi.cn/gtwkdtrmpr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hfpthk.cn/gtikfdiakr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.tian-w.cn/gtzeiddbzn.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj202588.top/gtwaiffemp.html

Java: // 手写 HashMap
来源：http://hz.gzhubu.top/gtjjbvglpv.html

Go:   // 手写 map[int]int
来源：http://hz.nwbrower.top/gtociinlys.html

Ruby: // 手写 Hash
来源：http://hz.zhoulong.xyz/gtkcmaevgt.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yangfankeji.com/gtdptkbmgn.html

[N08] 生成全排列
来源：http://hz.gaohongyu789.top/gturhtnnwq.html

Py:   itertools.permutations(arr)
来源：http://hz.yueranfly.top/gtmphzbhps.html

PHP:  // 手写递归交换
来源：http://hz.jyoumei.cn/gtqadjeolj.html

JS:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtwmlofveu.html

TS:   // 手写回溯递归
来源：http://hz.jqgfzy.top/gtstqospig.html

Java: // 手写回溯递归
来源：http://hz.zhongyouzk.top/gteyscimfc.html

Go:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gthtzszqwy.html

Ruby: arr.permutation.to_a
来源：http://hz.xingfuxueyuan.xyz/gtgvkoyjhz.html

C#:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtmgimgarm.html

[N09] 栈与队列
来源：http://hz.hnqzz.top/gtlouvcjyv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.chenzaomai.com/gthygzzesv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.fzhhl.top/gtfjywopbz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jqgufenzy.top/gtvvmswmcb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.pycfn.com/gtyoyvrgvn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhiwuduotai.top/gtorrwqgha.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.c1oappe.top/gtxzzmzjet.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.pengpengdd.cyou/gtvlmssadk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.daria6918.cn/gtdomzxrpw.html

[N10] 链表节点定义
来源：http://hz.ppjwa.cn/gtxqvbahum.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ydzc1.top/gtvrvgnsjk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.tian-w.cn/gtenioxcnz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhaomingkeji.xyz/gtjfgqetwc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jlsjyb.cn/gtboyiorhv.html

Java: class Node { int v; Node next; }
来源：http://hz.jinqigfzy.top/gtwydzvqvp.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ppjwa.cn/gtlmhtnnmb.html


<!-- 参考信息 -->