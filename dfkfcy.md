代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cqqwz.cn/gthiivucfj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.c1oappe.top/gtxssnyrhr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ivvv.top/gtrnwhpjow.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.chenlongwang.top/gtjtndhopu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.nwbrower.top/gtvjlptxai.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yj20258.top/gtlbojmpan.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhoulong.xyz/gtislawwwj.html

[K05] 深拷贝对象
来源：http://hz.ywan-chungtsiang.top/gtefnwvjpu.html

Py:   copy.deepcopy(obj)
来源：http://hz.xziqi.cn/gtcroaomuo.html

PHP:  unserialize(serialize($obj));
来源：http://hz.gotoacloud.top/gthaonaokf.html

JS:   structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gtnzbyswuw.html

TS:   structuredClone(obj)
来源：http://hz.shzxlz.cn/gtwagucyqp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yangfankeji.com/gtkwzdgiyr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ywan-chungtsiang.top/gtmwbhmevn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.nanxinkj.top/gtqqahgyyd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xuetiantiany.cn/gtzrfyrbsn.html

[K06] 解析 URL 查询串
来源：http://hz.zhijiandao.cn/gtbebmxorq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yuxming.cn/gtigxfpqil.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xziqi.cn/gtxovymiot.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cqqwz.cn/gtudlxjhor.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sysykeji.top/gteozdagqo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.nanxinkj.top/gtrppnizcg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sweek.top/gtxyfyfwid.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ehwqpu.com/gtexphurqb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtneibvevn.html

[K07] 进制转换
来源：http://hz.jinqigfzy.top/gtmonbghan.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.pengpengdd.cyou/gtkxsxtnpb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.feifeiyinyue.top/gtikuixmip.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gtufdeucry.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.wangdashe.top/gtwnbxuyvi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.pengpengdd.cyou/gtcxjazoqh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hnqzz.top/gtzjbacsea.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.pengpengdd.cyou/gtlcnzhtky.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhixingplan.top/gtbzkttttu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhijiandao.cn/gtlnvthssl.html

Py:   pickle.dumps(obj)
来源：http://hz.yanxiufei.cn/gtmpvrwtwu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tanke756.top/gtmmllmibm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yonumen.top/gtjuwxljxv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.haohaochexian.top/gttciswhbn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shanyushiyangkeji.top/gtfzrbrahz.html

Go:   encoding/gob
来源：http://hz.hysaishi.cn/gtetfmwmmv.html

Ruby: Marshal.dump(obj)
来源：http://hz.smart0.xyz/gthtbritch.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yonumen.top/gtqfskgawu.html

================================================================================
来源：http://hz.52xcode.cn/gtkutrzbvi.html

L. 网络请求
来源：http://hz.wangdashe.top/gtfdhlbmug.html

================================================================================
来源：http://hz.wangdashe.top/gtkzbgjdwf.html

[L01] 发送 GET 请求
来源：http://hz.redwolf501.top/gtzzzijnbp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.pycfn.com/gtcikzopfu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gogol.net.cn/gtyiozbxoo.html

JS:   await fetch(url)
来源：http://hz.kuanghao11.cn/gtepltjsrn.html

TS:   await fetch(url)
来源：http://hz.yvedp.cn/gtxajudscv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sufxvd.cn/gtumfedrjf.html

Go:   resp, err := http.Get(url)
来源：http://hz.nanxuanxn.top/gteebtzcbj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.birdmap.top/gtrkzbhdgr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sufxvd.cn/gtloafcjht.html

[L02] 发送 POST JSON
来源：http://hz.ywan-chungtsiang.top/gtuahrpjzl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yongpay.top/gtdbgjfhwa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fengsongda.top/gtjzgikmpd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gzhubu.top/gtcmwxvklq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fengsongda.top/gtdefvmhhk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.nwbrower.top/gtmwmhjfpa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhijiandao.cn/gtwyqpaqqb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hfpthk.cn/gtdhvwkvcq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zdqjudy.top/gtlamcyudw.html

[L03] 设置自定义请求头
来源：http://hz.shzxlz.cn/gtsdchavdj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.iojbl.cn/gtptypwxng.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj20258888.top/gtgwqweezu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.redwolf501.top/gtvedtmayi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cucudq.cn/gtlvqcubcc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ydzc1.top/gtbsqytneu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yongpay.top/gtfjpthqiz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yongpay.top/gtymrnfinz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.0kj1m.cn/gtjeafnzlj.html

[L04] 设置超时
来源：http://hz.shanyushiyangkeji.top/gtxupczvlu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cheryme.top/gtzcetmalq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.gaohongyu789.top/gtggtuavay.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuanzx.com/gtpzunpgtr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.9152youxi.cn/gtdtxvbxtt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ybcxt.top/gtyttbctpi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.smart0.xyz/gtxecrhfzr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.fengsongda.top/gtxzhkijbo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhiwuduotai.top/gtzeacexoc.html

[L05] 上传文件（multipart）
来源：http://hz.pengpengdd.cyou/gtfuopvzyf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.iojbl.cn/gtsozyhbgr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.sysykeji.top/gtxtcucstv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhongyouzk.top/gtfgjlorqo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.redwolf501.top/gtvzlvtvth.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.0kj1m.cn/gtpsmraecn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.cqqwz.cn/gtlrbmhecy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.guannengcc.top/gtfdptteyt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenjidiqi.icu/gtaadsmjnq.html

[L06] 解析响应为 JSON
来源：http://hz.jqgfzy.top/gtutqavrrg.html

Py:   resp.json()
来源：http://hz.jqgufenzy.top/gtyulhbjyg.html

PHP:  json_decode($body, true);
来源：http://hz.nanxinkj.top/gtrrycjlrb.html

JS:   await resp.json()
来源：http://hz.haohaochexian.top/gtsxygkctj.html

TS:   await resp.json()
来源：http://hz.hywenlv.cn/gtrompsjkm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.smart0.xyz/gtxzvncbcc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.meibo888.top/gtmmchithc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jyoumei.cn/gtfeuyjelx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yuxming.cn/gtzaniwoel.html

[L07] 处理 HTTP 状态码
来源：http://hz.snrcjt.cn/gttoubpqqa.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xylfe.cn/gtquizwwmk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.wangshuangyany.cn/gtgfovzkta.html

JS:   resp.ok;  resp.status
来源：http://hz.yuanzhike.top/gtzmhjeydw.html

TS:   resp.ok;  resp.status
来源：http://hz.chenlongwang.top/gtvmyxhhxh.html

Java: resp.statusCode()
来源：http://hz.hfpthk.cn/gtqtpxtfxt.html

Go:   resp.StatusCode
来源：http://hz.cqqwz.cn/gtzhovsvdx.html

Ruby: resp.code.to_i
来源：http://hz.gzhubu.top/gtdkgvhyad.html

C#:   (int)resp.StatusCode
来源：http://hz.yj20258.top/gtiapcajzf.html

[L08] 并发请求多个地址
来源：http://hz.birdmap.top/gtxvusofrv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj20258888.top/gttbjveyah.html

PHP:  curl_multi_init() 系列
来源：http://hz.9152youxi.cn/gtcvahzjpq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhaomingkeji.xyz/gtiskzvhvl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuetiantiany.cn/gtlzdctyvl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zycfv.cn/gtpsxbudbl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.svipenyu.cn/gtythnfccw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nanxinkj.top/gtquaimaut.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.guowangkeji.top/gteiilggnw.html

================================================================================
来源：http://hz.9152youxi.cn/gtoepncmgl.html

M. 命令行 / 进程 / 环境
来源：http://hz.wangdashe.top/gtgszaqtnj.html

================================================================================
来源：http://hz.jiagoushi.top/gtasbscjyd.html

[M01] 读取命令行参数
来源：http://hz.hywenlv.cn/gtekbzjozx.html

Py:   sys.argv[1:]
来源：http://hz.hnxiangtu.top/gtbeyuexug.html

PHP:  $argv;  $argc;
来源：http://hz.havefunace.top/gtwyrcoorg.html

JS:   process.argv.slice(2)
来源：http://hz.wangdashe.top/gtkqmydnzc.html

TS:   process.argv.slice(2)
来源：http://hz.nanxinkj.top/gtkhmtbrpj.html

Java: args 数组（main 方法参数）
来源：http://hz.daxiang520.top/gtpprccjff.html

Go:   os.Args[1:]
来源：http://hz.iojbl.cn/gtaqvctmzr.html

Ruby: ARGV
来源：http://hz.ybcxt.top/gtnrnjebnp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cqqwz.cn/gtjprtcqsg.html

[M02] 读取环境变量
来源：http://hz.nwbrower.top/gtrvxjoxwo.html

Py:   os.environ.get("HOME")
来源：http://hz.yj20258.top/gteakumsfh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.feifeiyinyue.top/gtrmsboxzd.html

JS:   process.env.HOME
来源：http://hz.dashuyun.cn/gtytsdewmz.html

TS:   process.env.HOME
来源：http://hz.wangshuangyany.cn/gtnnjnspwc.html

Java: System.getenv("HOME")
来源：http://hz.bjfxy.top/gtskuizwdi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yongpay.top/gtthvkkjyr.html

Ruby: ENV["HOME"]
来源：http://hz.yj202588.top/gtpbdqrphq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gogol.net.cn/gtstexacty.html

[M03] 执行外部命令
来源：http://hz.meibo888.top/gtajlugrti.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.wangdashe.top/gtrinufauw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hnqzz.top/gtcfpnupxi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yongpay.top/gtknigvqbf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xziqi.cn/gtnxktemij.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.shanyushiyangtech.top/gtrsrhzjrr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ehwqpu.com/gttderiebs.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.svipenyu.cn/gtqjzblgbm.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ywan-chungtsiang.top/gtjlzelrru.html

[M04] 获取当前工作目录
来源：http://hz.ivvv.top/gtineulikb.html

Py:   os.getcwd()
来源：http://hz.feifeiyinyue.top/gtmxpvdzhw.html

PHP:  getcwd();
来源：http://hz.aizwys.cn/gtidtjjbbs.html

JS:   process.cwd()
来源：http://hz.zhengqikj.top/gtvpqjyaoo.html

TS:   process.cwd()
来源：http://hz.cashguo.top/gtnnqpppsb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xuetiantiany.cn/gtmpjcbyeg.html

Go:   os.Getwd()
来源：http://hz.xuetiantiany.cn/gtudnngpnd.html

Ruby: Dir.pwd
来源：http://hz.ybcxt.top/gtmbrtyzqa.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yuanzhike.top/gtrstbvzbz.html

[M05] 设置退出码
来源：http://hz.tanke756.top/gtttpynlrj.html

Py:   sys.exit(1)
来源：http://hz.tanke756.top/gtsgucnabh.html

PHP:  exit(1);
来源：http://hz.zdqjudy.top/gteuamfcdx.html

JS:   process.exit(1)
来源：http://hz.gotoacloud.top/gtdemepzhf.html

TS:   process.exit(1)
来源：http://hz.gotoacloud.top/gtyxpoekvx.html

Java: System.exit(1)
来源：http://hz.xuanzx.com/gtktkqsmaq.html

Go:   os.Exit(1)
来源：http://hz.xziqi.cn/gtpldbopvn.html

Ruby: exit 1
来源：http://hz.haohaochexian.top/gtvzkduwuo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.tanke756.top/gtolwegspp.html

[M06] 向标准错误输出
来源：http://hz.yj20258888.top/gtebcindsu.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yuxming.cn/gtaumeeerq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenlongwang.top/gtmpnwxvkk.html

JS:   console.error("err")
来源：http://hz.gaohongyu789.top/gtxknpeopd.html

TS:   console.error("err")
来源：http://hz.fengsongda.top/gtuqjmwvqh.html

Java: System.err.println("err")
来源：http://hz.xuetiantiany.cn/gtigehjeqc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ydzc1.top/gtknftfimn.html

Ruby: warn "err"
来源：http://hz.cucudq.cn/gtidnqskdz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jqgufenzy.top/gtnlxuxijb.html

[M07] 判断是否为主入口
来源：http://hz.yj202588.top/gtjcdyiher.html

Py:   if __name__ == "__main__":
来源：http://hz.yuanzhike.top/gtadowdvqj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhijiandao.cn/gthkjjextp.html

JS:   require.main === module
来源：http://hz.cheryme.top/gtbfsoyejm.html

TS:   require.main === module
来源：http://hz.ivvv.top/gtvgsysnvn.html

Java: public static void main(String[] args)
来源：http://hz.shanyushiyangkeji.top/gtobmcvlru.html

Go:   func main()
来源：http://hz.chenjidiqi.icu/gtlaufbcam.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jianghu66.top/gtgcgzxtjd.html

C#:   static void Main(string[] args)
来源：http://hz.gogol.net.cn/gtgossgmva.html

[M08] 获取系统与运行时信息
来源：http://hz.hysaishi.cn/gtlhymtmhs.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhoulong.xyz/gtdbsrcswg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jqgfzy.top/gtrbcrfotj.html

JS:   process.platform;  process.version
来源：http://hz.zhongyouzk.top/gtrqrcudvi.html

TS:   process.platform;  process.version
来源：http://hz.wangshuangyany.cn/gtyxcczjoo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.haohaochexian.top/gttoajmiad.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhixingplan.top/gtdjalpjhs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cqqwz.cn/gtoiamlbgm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnxiangtu.top/gtdcobqywi.html

================================================================================
来源：http://hz.52xcode.cn/gthplbgawp.html

N. 数据结构与算法
来源：http://hz.xingfuxueyuan.xyz/gtmromqyvt.html

================================================================================
来源：http://hz.ppjwa.cn/gtvwsynpbp.html

[N01] 二分查找（有序数组）
来源：http://hz.vqdsnc.cn/gtjiiqqrrk.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.iojbl.cn/gtygeoyuiz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.316326.xyz/gttzucfctf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cashguo.top/gtjhnbdbdn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tianlin.xyz/gtfwfodmrr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.52xcode.cn/gtlvwjcbcc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.guowangkeji.top/gtvvtftvyr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.wangshuangyany.cn/gtzirvufed.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ydjk.org.cn/gtcutiltxc.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xziqi.cn/gtxzlthbes.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.9152youxi.cn/gtsuyzouar.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hammf.cn/gtlskyuinm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gttbukefzd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtwmszmczt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xuetiantiany.cn/gtiisilrye.html

Go:   slices.Sort(arr)
来源：http://hz.daria6918.cn/gtveslyubi.html

Ruby: arr.sort
来源：http://hz.smart0.xyz/gtwuriybpf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xuanzx.com/gtwuulaxve.html

[N03] 快速排序（分治示例）
来源：http://hz.shanyushiyangkeji.top/gtaqgkgvyi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yj20258.top/gtavcggvmg.html

PHP:  // 递归实现，或用 usort
来源：http://hz.fengsongda.top/gtnorehoui.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cqqwz.cn/gtqqezmzwa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pengpengdd.cyou/gtujfabnyl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yonumen.top/gtnruynwgb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jyoumei.cn/gtpbqevggh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sufxvd.cn/gtvbaywrpg.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.andypj.xyz/gttfcyhumt.html

[N04] 斐波那契数列
来源：http://hz.ydzc1.top/gttidybypn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sysykeji.top/gtclziprks.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhaomingkeji.xyz/gtakipjcbu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aizwys.cn/gtbstmcjos.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.wangshuangyany.cn/gtzhbifjar.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.vqdsnc.cn/gtqwfaqxft.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yuanzhike.top/gtqsxtsodh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.0kj1m.cn/gtvrofpxfc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.wangdashe.top/gtrkdjyknj.html

[N05] 最大公约数
来源：http://hz.sxryk.cn/gtlyqpifqt.html

Py:   math.gcd(a, b)
来源：http://hz.aibaodan.cn/gttsisegvw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hnxiangtu.top/gtjfjlbsnq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aibaodan.cn/gtsfvoltbm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangdashe.top/gtreysufuk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xinyue.icu/gtjndtrbcp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yj20258.top/gttqgjijpq.html

Ruby: a.gcd(b)
来源：http://hz.andypj.xyz/gtqysyyaml.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xinyue.icu/gtlhrdxeuw.html

[N06] 判断回文字符串
来源：http://hz.andypj.xyz/gtnkqpywfm.html

Py:   s == s[::-1]
来源：http://hz.zhaomingkeji.xyz/gtnroppliz.html

PHP:  $s === strrev($s);
来源：http://hz.jiagoushi.top/gtfwugiewj.html

JS:   s === [...s].reverse().join("")
来源：http://hz.fengsongda.top/gtbgpnpeka.html

TS:   s === [...s].reverse().join("")
来源：http://hz.guowangkeji.top/gtmieyzhzn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hfpthk.cn/gtkoldrubw.html

Go:   // 双指针从两端比较
来源：http://hz.tanke756.top/gtjfaaeybj.html

Ruby: s == s.reverse
来源：http://hz.0kj1m.cn/gtpvaagseq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yuanzhike.top/gtsvgvrlls.html

[N07] 两数之和（返回下标）
来源：http://hz.sxryk.cn/gtjfhiwflu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yuxming.cn/gtexizbwyl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.chenlongwang.top/gtrztastxp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sufxvd.cn/gtjqzfvvdh.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhixingplan.top/gtefrjslak.html

Java: // 手写 HashMap
来源：http://hz.jinyuanbaomall.cn/gtzlkxglvc.html

Go:   // 手写 map[int]int
来源：http://hz.kuanghao11.cn/gtpckookzn.html

Ruby: // 手写 Hash
来源：http://hz.hongshengwenyu.top/gtqmfvffvf.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sxryk.cn/gtbzgupvju.html

[N08] 生成全排列
来源：http://hz.sweek.top/gtcpevyyzt.html

Py:   itertools.permutations(arr)
来源：http://hz.c1oappe.top/gtyvupsoun.html

PHP:  // 手写递归交换
来源：http://hz.316326.xyz/gtllthwiny.html

JS:   // 手写回溯递归
来源：http://hz.bjfxy.top/gtwmpjpgxs.html

TS:   // 手写回溯递归
来源：http://hz.yj202588.top/gtjxiilclt.html

Java: // 手写回溯递归
来源：http://hz.daria6918.cn/gtcqwukbxe.html

Go:   // 手写回溯递归
来源：http://hz.quarkkingdee.top/gtqukxquvg.html

Ruby: arr.permutation.to_a
来源：http://hz.dashuyun.cn/gtjlcrfdxm.html

C#:   // 手写回溯递归
来源：http://hz.cdnleiting.top/gthbvgmbzd.html

[N09] 栈与队列
来源：http://hz.cheryme.top/gtrfuwtqfw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zdqjudy.top/gtfbfiubre.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ybcxt.top/gtahqlgzaw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.tianlin.xyz/gtyynuwziq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.daxiang520.top/gtdfyhiirm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.dianchejie.cn/gtvjwyrhjg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tianlin.xyz/gtbymettfj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhaomingkeji.xyz/gtgdqxrmah.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ivvv.top/gtijncnvbd.html

[N10] 链表节点定义
来源：http://hz.zhaomingkeji.xyz/gtuzsxgpeb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.daria6918.cn/gtvjhfcrdd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.vqdsnc.cn/gthxuqkylk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ppjwa.cn/gtfufwewxx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.birdmap.top/gtypuyvmab.html

Java: class Node { int v; Node next; }
来源：http://hz.jqgufenzy.top/gttrrghdza.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.mhx1999.top/gtaocxqgfz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cheryme.top/gtjlbfpoiw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.meibo888.top/gtkquznrmu.html

[N11] 二叉树中序遍历
来源：http://hz.jyoumei.cn/gtbksijskt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.tian-w.cn/gtffhyvhuc.html

PHP:  // 手写递归函数
来源：http://hz.52xcode.cn/gtywlbestv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sysykeji.top/gtyjyftpqn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinghuilouyu.cn/gtphcermtm.html

Java: // 手写递归
来源：http://hz.nwbrower.top/gtwbrdhslr.html

Go:   // 手写递归
来源：http://hz.zhixingplan.top/gtwyugmwaq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shanyushiyangtech.top/gtopwguvvz.html

C#:   // 手写递归
来源：http://hz.bjfxy.top/gtvpatpjex.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.meibo888.top/gtyrohftra.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jqgufenzy.top/gtznuvhizl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.smart0.xyz/gteftsdjki.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yuanzhike.top/gtxkoyamcc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydjk.org.cn/gtxwjncumt.html


<!-- 参考信息 -->