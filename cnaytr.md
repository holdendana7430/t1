代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://hz.c1oappe.top/gtuqbtzuql.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xylfe.cn/gttvbnfcsi.html

[K04] 读取 JSON 文件
来源：http://hz.yonumen.top/gtareatunn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ehwqpu.com/gtvxzrefud.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.nanxinkj.top/gtmvvjmhtq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shuidangran.top/gtspplizwi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxuanxn.top/gthssrmbbt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nwbrower.top/gtmmeeupld.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ivvv.top/gtplanpzwb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shuidangran.top/gtitxvgsvv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.nanxinkj.top/gtfstinwri.html

[K05] 深拷贝对象
来源：http://hz.xylfe.cn/gtvubpmuhl.html

Py:   copy.deepcopy(obj)
来源：http://hz.yuanzhike.top/gtrueiugxu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ivvv.top/gtviodkztv.html

JS:   structuredClone(obj)
来源：http://hz.cqqwz.cn/gtwfegdprr.html

TS:   structuredClone(obj)
来源：http://hz.haohaochexian.top/gthwekisxi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jyoumei.cn/gtmntzsgyp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.kuanghao11.cn/gtlqojshzf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhixingplan.top/gtsgdwozcr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ywan-chungtsiang.top/gtcmuomdiu.html

[K06] 解析 URL 查询串
来源：http://hz.xziqi.cn/gtrqueihch.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.pycfn.com/gtzcnmqzgb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.guowangkeji.top/gtdtqvhqxy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tanke756.top/gtwuizmmkc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.birdmap.top/gtasiekzph.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.wangshuangyany.cn/gtpphjllgo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xziqi.cn/gtxbojkvcv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhijiandao.cn/gtoycaeceu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.kuanghao11.cn/gtplbgharf.html

[K07] 进制转换
来源：http://hz.yj202588.top/gtkftiopiw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yonumen.top/gtdssvjcux.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.fengsongda.top/gtbrymaiii.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xuanzx.com/gtwcorwzly.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xuanzx.com/gtoqpaswym.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cqqwz.cn/gtororitzh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shanyushiyangkeji.top/gtlqkyhpcf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shangyingyoupin.top/gtkofhghmg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ehwqpu.com/gtmzlidops.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yueranfly.top/gtlghpcmnt.html

Py:   pickle.dumps(obj)
来源：http://hz.aizwys.cn/gtchssrkgt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shangyingyoupin.top/gtwfzzubqb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.smart0.xyz/gtgdnvwclr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hammf.cn/gtzrihjksf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yvedp.cn/gtvqdhqojo.html

Go:   encoding/gob
来源：http://hz.nanxinkj.top/gtamwfmgxi.html

Ruby: Marshal.dump(obj)
来源：http://hz.cqqwz.cn/gtbiowwglo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sysykeji.top/gtynfxalvw.html

================================================================================
来源：http://hz.yongpay.top/gtlsvruxom.html

L. 网络请求
来源：http://hz.hnxiangtu.top/gtpktrhrtw.html

================================================================================
来源：http://hz.yanxiufei.cn/gtrkvowsjk.html

[L01] 发送 GET 请求
来源：http://hz.cucudq.cn/gtrljcavph.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ybcxt.top/gtbhqwljlq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shangyingyoupin.top/gtlkluvhnt.html

JS:   await fetch(url)
来源：http://hz.zhiwuduotai.top/gtpkyovqgr.html

TS:   await fetch(url)
来源：http://hz.haohaochexian.top/gtadtplxlz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.feifeiyinyue.top/gtprxmzxzy.html

Go:   resp, err := http.Get(url)
来源：http://hz.jqgufenzy.top/gtfwyfadvc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gotoacloud.top/gtpjsfheyv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cashguo.top/gtzduesoba.html

[L02] 发送 POST JSON
来源：http://hz.kuanghao11.cn/gtvsulrxwg.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shangyingyoupin.top/gtpsmcyost.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cqqwz.cn/gtsbfgrkaw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hongshengwenyu.top/gtxjpyjool.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.c1oappe.top/gtrdvbtufs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.9152youxi.cn/gtjbjkvtwj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nanxinkj.top/gtxxwayzhr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.chenlongwang.top/gttfybsocz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.daxiang520.top/gtcecqvfvf.html

[L03] 设置自定义请求头
来源：http://hz.chenjidiqi.icu/gtavlikfrt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jyoumei.cn/gtempmcmnp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.aizwys.cn/gtaseguafu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuanzx.com/gtfhltwxjh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhiwuduotai.top/gtvviqixfh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.aibaodan.cn/gttnfrchdd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.vqdsnc.cn/gtswjxbaqt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhixingplan.top/gttilrqldb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nanxinkj.top/gtgzmdrbfu.html

[L04] 设置超时
来源：http://hz.gotoacloud.top/gtmbkbrnib.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jqgfzy.top/gtcocxfywt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.gogol.net.cn/gtphtvdjjy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.havefunace.top/gtvvoenrqo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gotoacloud.top/gtcrycbydd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cheryme.top/gttwabvxeb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jqgufenzy.top/gtsdglivmq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ppjwa.cn/gtguaqjcsd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.9152youxi.cn/gtiazmqkqr.html

[L05] 上传文件（multipart）
来源：http://hz.hnqzz.top/gttliuxjog.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.pengpengdd.cyou/gtxltzjrng.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yueranfly.top/gthfyylkxf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.vqdsnc.cn/gtucwpfkhh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zdqjudy.top/gtzadcdeah.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.quarkkingdee.top/gtlaljawjo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xingfuxueyuan.xyz/gtcyeiotpn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.wangdashe.top/gtsfxtzfzv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ehwqpu.com/gtuibvdlyy.html

[L06] 解析响应为 JSON
来源：http://hz.cheryme.top/gtwsudfukx.html

Py:   resp.json()
来源：http://hz.ppjwa.cn/gtadezalae.html

PHP:  json_decode($body, true);
来源：http://hz.guannengcc.top/gturzseych.html

JS:   await resp.json()
来源：http://hz.xylfe.cn/gtyvlbyftb.html

TS:   await resp.json()
来源：http://hz.jiagoushi.top/gtivzismih.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nanxinkj.top/gtvyviyqln.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.tanke756.top/gtpnhdbmhm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.daria6918.cn/gtsdvvcitx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jinqigfzy.top/gtiatxnrwd.html

[L07] 处理 HTTP 状态码
来源：http://hz.gogol.net.cn/gtqtkztecf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jinyuanbaomall.cn/gtclufwthg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.c1oappe.top/gtltwufrny.html

JS:   resp.ok;  resp.status
来源：http://hz.jqgfzy.top/gtipytmzex.html

TS:   resp.ok;  resp.status
来源：http://hz.yongpay.top/gtscpfphtx.html

Java: resp.statusCode()
来源：http://hz.jianghu66.top/gtbubwudsu.html

Go:   resp.StatusCode
来源：http://hz.hammf.cn/gttynoyvaw.html

Ruby: resp.code.to_i
来源：http://hz.zhoulong.xyz/gtrptbctkw.html

C#:   (int)resp.StatusCode
来源：http://hz.svipenyu.cn/gtrljqbtdw.html

[L08] 并发请求多个地址
来源：http://hz.bjfxy.top/gtavssiyyu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.316326.xyz/gtieiekyth.html

PHP:  curl_multi_init() 系列
来源：http://hz.pycfn.com/gtfdrmutwz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhiwuduotai.top/gtwvbbyrpe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuanzhike.top/gtgdlplqud.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gogol.net.cn/gtturugtzf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhengqikj.top/gtroupbssw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.andypj.xyz/gtysfvyxvf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yonumen.top/gtowupwdol.html

================================================================================
来源：http://hz.nanxinkj.top/gtrvqguqlo.html

M. 命令行 / 进程 / 环境
来源：http://hz.dianchejie.cn/gtitpenrlt.html

================================================================================
来源：http://hz.hnxiangtu.top/gtdlvkgymj.html

[M01] 读取命令行参数
来源：http://hz.cdnleiting.top/gtjufeuveh.html

Py:   sys.argv[1:]
来源：http://hz.chenzaomai.com/gtuqnnltel.html

PHP:  $argv;  $argc;
来源：http://hz.gogol.net.cn/gtnsthifhk.html

JS:   process.argv.slice(2)
来源：http://hz.aizwys.cn/gtoodimrxn.html

TS:   process.argv.slice(2)
来源：http://hz.yj20258888.top/gtshuydwzm.html

Java: args 数组（main 方法参数）
来源：http://hz.tian-w.cn/gtenbgxyha.html

Go:   os.Args[1:]
来源：http://hz.sweek.top/gterufqkwz.html

Ruby: ARGV
来源：http://hz.9152youxi.cn/gtthpxuwhd.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenzaomai.com/gtpsqycoxv.html

[M02] 读取环境变量
来源：http://hz.fengsongda.top/gtstnylwmv.html

Py:   os.environ.get("HOME")
来源：http://hz.yongpay.top/gtrjjxgxdm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xziqi.cn/gtcosenouo.html

JS:   process.env.HOME
来源：http://hz.zhoulong.xyz/gtodmvkqbq.html

TS:   process.env.HOME
来源：http://hz.jinghuilouyu.cn/gtaklmpvww.html

Java: System.getenv("HOME")
来源：http://hz.haohaochexian.top/gtvvgfoewj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ydzc1.top/gtudyvxkyi.html

Ruby: ENV["HOME"]
来源：http://hz.jinghuilouyu.cn/gttitkwsbo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.aibaodan.cn/gtrszrmpiv.html

[M03] 执行外部命令
来源：http://hz.chenzaomai.com/gtbejegtnz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shzxlz.cn/gtcogugdqg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhiwuduotai.top/gtgdxzaqfr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenlongwang.top/gtjkpxutrv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangkeji.top/gtcsivxxzj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.nanxinkj.top/gtdlfwgyxj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jiagoushi.top/gtksnqxgbu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.bjfxy.top/gtewsevwff.html

C#:   Process.Start("ls", "-l");
来源：http://hz.nwbrower.top/gtshtstfat.html

[M04] 获取当前工作目录
来源：http://hz.redwolf501.top/gtlrswgesg.html

Py:   os.getcwd()
来源：http://hz.yuxming.cn/gtqvtrytie.html

PHP:  getcwd();
来源：http://hz.xylfe.cn/gtadcvpjfb.html

JS:   process.cwd()
来源：http://hz.gogol.net.cn/gtorhfqqwf.html

TS:   process.cwd()
来源：http://hz.fzhhl.top/gtgdbyvbjn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.iojbl.cn/gtkqfztibi.html

Go:   os.Getwd()
来源：http://hz.nanxuanxn.top/gtidnzglqx.html

Ruby: Dir.pwd
来源：http://hz.shzxlz.cn/gtavvgtukx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.c1oappe.top/gtpvswwiem.html

[M05] 设置退出码
来源：http://hz.sysykeji.top/gtemkthyuu.html

Py:   sys.exit(1)
来源：http://hz.sysykeji.top/gtacfwkzpc.html

PHP:  exit(1);
来源：http://hz.wangdashe.top/gtyypjkmec.html

JS:   process.exit(1)
来源：http://hz.yj20258.top/gtnzizauhi.html

TS:   process.exit(1)
来源：http://hz.ppjwa.cn/gtqvfouxps.html

Java: System.exit(1)
来源：http://hz.zhixingplan.top/gthnwtppmh.html

Go:   os.Exit(1)
来源：http://hz.sufxvd.cn/gtpwkpbaqw.html

Ruby: exit 1
来源：http://hz.zhoulong.xyz/gtvygcpppq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sysykeji.top/gtqyzajdfh.html

[M06] 向标准错误输出
来源：http://hz.sysykeji.top/gtfynaycqr.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhaomingkeji.xyz/gtmzhtwnnb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinqigufen.top/gtbohqrvlw.html

JS:   console.error("err")
来源：http://hz.ppjwa.cn/gtnuxenfro.html

TS:   console.error("err")
来源：http://hz.guannengcc.top/gtgqwgrhjy.html

Java: System.err.println("err")
来源：http://hz.shanyushiyangkeji.top/gthgpzzaog.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.dianchejie.cn/gtprueosiz.html

Ruby: warn "err"
来源：http://hz.yangfankeji.com/gtrhnxqmzv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hammf.cn/gtemclkzyj.html

[M07] 判断是否为主入口
来源：http://hz.zhijiandao.cn/gtghchzidd.html

Py:   if __name__ == "__main__":
来源：http://hz.yueranfly.top/gtvhffotyb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.pengpengdd.cyou/gttsjgjjau.html

JS:   require.main === module
来源：http://hz.gzhubu.top/gtzeyrxatk.html

TS:   require.main === module
来源：http://hz.hammf.cn/gtostjjrae.html

Java: public static void main(String[] args)
来源：http://hz.andypj.xyz/gtuftuytlj.html

Go:   func main()
来源：http://hz.yuanzhike.top/gtprastmoc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yj20258.top/gtvtenaonx.html

C#:   static void Main(string[] args)
来源：http://hz.zhiwuduotai.top/gtvyxaifub.html

[M08] 获取系统与运行时信息
来源：http://hz.xziqi.cn/gtfjrovkhe.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhixingplan.top/gtlazdsmtp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.svipenyu.cn/gtsvsuzvgj.html

JS:   process.platform;  process.version
来源：http://hz.havefunace.top/gtviszntnk.html

TS:   process.platform;  process.version
来源：http://hz.pengpengdd.cyou/gttkpafwyo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.pycfn.com/gtkqbigtwh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zycfv.cn/gtaaartxxs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinyuanbaomall.cn/gtwolabyqh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.andypj.xyz/gtpzgipzuw.html

================================================================================
来源：http://hz.sysykeji.top/gtramnqxuu.html

N. 数据结构与算法
来源：http://hz.quarkkingdee.top/gtydhxlzbd.html

================================================================================
来源：http://hz.hywenlv.cn/gtpdlpyjzr.html

[N01] 二分查找（有序数组）
来源：http://hz.yvedp.cn/gtcfqlnepz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yangfankeji.com/gtibmvahkm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ydzc1.top/gtawktyoxj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.snrcjt.cn/gtxhkeqhij.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj202588.top/gtcnywkmnh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ivvv.top/gtrzbpmpnz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.aibaodan.cn/gtubrgxjbj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinghuilouyu.cn/gtcvppkqke.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtydlpdifd.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yj20258888.top/gtyswlyotk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.dashuyun.cn/gtfkhaanwc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.wangshuangyany.cn/gtvwunoajc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.haohaochexian.top/gtgepncwvg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.kuanghao11.cn/gtpxfmgwkt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ydzc1.top/gtvomkqkwh.html

Go:   slices.Sort(arr)
来源：http://hz.hnqzz.top/gtmqtwimcy.html

Ruby: arr.sort
来源：http://hz.wangshuangyany.cn/gtxjywguok.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ivvv.top/gtxwssuvvo.html

[N03] 快速排序（分治示例）
来源：http://hz.cucudq.cn/gtujezbikx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhiwuduotai.top/gtfswtahsv.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tian-w.cn/gtvurbevrd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.mhx1999.top/gtbtmyeckj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.daxiang520.top/gtukixchei.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhengqikj.top/gtkpwalxgw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nanxinkj.top/gtyyecjgcz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jqgfzy.top/gthimdmqhe.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xuetiantiany.cn/gtrvquaflr.html

[N04] 斐波那契数列
来源：http://hz.jyoumei.cn/gtwondlfoc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hysaishi.cn/gtcjeqwrkh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jyoumei.cn/gtnwtugqot.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.havefunace.top/gtiphyohca.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.snrcjt.cn/gtwgphovyv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhaomingkeji.xyz/gtjhieqgya.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hysaishi.cn/gtoeelfwuw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.nwbrower.top/gtgafvgshc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hnxiangtu.top/gtxyoulxul.html

[N05] 最大公约数
来源：http://hz.haohaochexian.top/gtoisfajpj.html

Py:   math.gcd(a, b)
来源：http://hz.zdqjudy.top/gtivbriobr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinqigfzy.top/gtvtxqcoyd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tanke756.top/gtkfdzsxje.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sufxvd.cn/gtiokxbvqy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.nanxuanxn.top/gtndpqjxrt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenzaomai.com/gtnlguxttt.html

Ruby: a.gcd(b)
来源：http://hz.sysykeji.top/gtwzxfoftm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.316326.xyz/gtcgjbltfb.html

[N06] 判断回文字符串
来源：http://hz.jiagoushi.top/gtifrjjhid.html

Py:   s == s[::-1]
来源：http://hz.52xcode.cn/gtyutdhhia.html

PHP:  $s === strrev($s);
来源：http://hz.hfpthk.cn/gtfxkuhtpu.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sysykeji.top/gtxakvmfiy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tanke756.top/gtvoeqrvpr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.nanxinkj.top/gtehzgvqty.html

Go:   // 双指针从两端比较
来源：http://hz.quarkkingdee.top/gtcjnyvdmc.html

Ruby: s == s.reverse
来源：http://hz.yj20258.top/gtcrlcbxxn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.bjfxy.top/gtpgmgzfwz.html

[N07] 两数之和（返回下标）
来源：http://hz.zycfv.cn/gtwwhiuesn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinghuilouyu.cn/gtpjuqijnd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhoulong.xyz/gtqhepexpm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.pycfn.com/gtunkfhnwv.html

TS:   // 手写 Map<string, number>
来源：http://hz.quarkkingdee.top/gtxzsofckr.html

Java: // 手写 HashMap
来源：http://hz.ivvv.top/gtumvgkjno.html

Go:   // 手写 map[int]int
来源：http://hz.cqqwz.cn/gtdjhbxpcz.html

Ruby: // 手写 Hash
来源：http://hz.xziqi.cn/gtaarcrpno.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.meibo888.top/gthtkynkzu.html

[N08] 生成全排列
来源：http://hz.hnxiangtu.top/gtvuhqpvap.html

Py:   itertools.permutations(arr)
来源：http://hz.hnxiangtu.top/gtlvisdnnn.html

PHP:  // 手写递归交换
来源：http://hz.jinghuilouyu.cn/gtomjxtywh.html

JS:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtknsxznex.html

TS:   // 手写回溯递归
来源：http://hz.cashguo.top/gthkwltbci.html

Java: // 手写回溯递归
来源：http://hz.cdnleiting.top/gtzvnsueym.html

Go:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtuvfjcfgt.html

Ruby: arr.permutation.to_a
来源：http://hz.jqgufenzy.top/gtaaztmqdn.html

C#:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtyxsgvksq.html

[N09] 栈与队列
来源：http://hz.nanxinkj.top/gtsmjijfjh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zdqjudy.top/gtebgdtfnj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xziqi.cn/gtugrluawt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hammf.cn/gtuvrlifsv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.aizwys.cn/gtzveyzvmo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hywenlv.cn/gtkmsuryca.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gaohongyu789.top/gtjvpgihiu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.chenzaomai.com/gtkegnzxyt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hywenlv.cn/gtsxtprejd.html

[N10] 链表节点定义
来源：http://hz.316326.xyz/gtdrxkthns.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zycfv.cn/gttmialrfj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zdqjudy.top/gtweylinrh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xuanzx.com/gtbfmvzzmi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.feifeiyinyue.top/gtooebewse.html

Java: class Node { int v; Node next; }
来源：http://hz.jinqigfzy.top/gtmdwdxbsb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.birdmap.top/gtajsdxkjv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.aizwys.cn/gtfquwijtd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ybcxt.top/gtegzswgka.html

[N11] 二叉树中序遍历
来源：http://hz.yongpay.top/gtppzwkwyz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.nanxinkj.top/gtevcwwswi.html

PHP:  // 手写递归函数
来源：http://hz.xingfuxueyuan.xyz/gtxuwqsees.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jyoumei.cn/gteoysyvkv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhixingplan.top/gtrtnryptx.html

Java: // 手写递归
来源：http://hz.ybcxt.top/gtnskgtgaa.html

Go:   // 手写递归
来源：http://hz.xuanzx.com/gtuzkmeuks.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.gogol.net.cn/gtvequmnjf.html

C#:   // 手写递归
来源：http://hz.316326.xyz/gtgyuyjcji.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jqgfzy.top/gtfmkfbfpe.html


<!-- 参考信息 -->