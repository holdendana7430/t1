代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://hz.ydzc1.top/gtiiuorche.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenjidiqi.icu/gtyaxjiyqq.html

JS:   structuredClone(obj)
来源：http://hz.yongpay.top/gtoshsntbr.html

TS:   structuredClone(obj)
来源：http://hz.wangdashe.top/gtuqgonhft.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhiwuduotai.top/gtrylsfvkd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj20258888.top/gtipmqxmxq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.fzhhl.top/gtnykgpanr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.nanxinkj.top/gtcnysgdcm.html

[K06] 解析 URL 查询串
来源：http://hz.snrcjt.cn/gtnesogrto.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.mhx1999.top/gttsouzhkv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tianlin.xyz/gtgwfpsxrd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.316326.xyz/gtnbpaljqy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtqianlkrk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenlongwang.top/gtbvsyookc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.dianchejie.cn/gtvwjvsqkb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shanyushiyangtech.top/gtkmymprkb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.wangshuangyany.cn/gtxjobakrj.html

[K07] 进制转换
来源：http://hz.wangdashe.top/gtwaputiuh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.aizwys.cn/gtsmhkcdav.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhengqikj.top/gttfgfsmvm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tanke756.top/gtapbqeyup.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhixingplan.top/gttwzydfhf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtulmgfoxc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shanyushiyangkeji.top/gtszvuuweg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.316326.xyz/gtojxibzzx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nanxinkj.top/gtelhydwda.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shanyushiyangtech.top/gtocutrxld.html

Py:   pickle.dumps(obj)
来源：http://hz.9152youxi.cn/gtgmsbhtna.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinqigfzy.top/gthorrfpnf.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ydzc1.top/gtedmjybfh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.pengpengdd.cyou/gtikeqdxax.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yueranfly.top/gtmqnjmynb.html

Go:   encoding/gob
来源：http://hz.ppjwa.cn/gtxmtgayrx.html

Ruby: Marshal.dump(obj)
来源：http://hz.aibaodan.cn/gthyzogaxu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj20258888.top/gtaifkbkyk.html

================================================================================
来源：http://hz.xinyue.icu/gtnkhpqprl.html

L. 网络请求
来源：http://hz.chenlongwang.top/gttnpvqgus.html

================================================================================
来源：http://hz.fzhhl.top/gtvonnzvtb.html

[L01] 发送 GET 请求
来源：http://hz.daxiang520.top/gtencdttwo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.0kj1m.cn/gtyozwbmky.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.wangshuangyany.cn/gtkfdriswx.html

JS:   await fetch(url)
来源：http://hz.jianghu66.top/gtqpgxjavf.html

TS:   await fetch(url)
来源：http://hz.xylfe.cn/gtapvxfqja.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.vqdsnc.cn/gtjmodtawn.html

Go:   resp, err := http.Get(url)
来源：http://hz.aizwys.cn/gtgtgblcby.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hnxiangtu.top/gtkxiiabru.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jiagoushi.top/gtsnxpbhzt.html

[L02] 发送 POST JSON
来源：http://hz.zhijiandao.cn/gtnzgelutl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hammf.cn/gtlxrdkhln.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jianghu66.top/gtecckeswl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yonumen.top/gtkacvxrfa.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zycfv.cn/gtfcwotadz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.316326.xyz/gtldqdbmqy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhengqikj.top/gtodezrhnt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.guannengcc.top/gtfenmiujk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hfpthk.cn/gtonrgxoqi.html

[L03] 设置自定义请求头
来源：http://hz.hfpthk.cn/gtukawnuse.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gotoacloud.top/gtenlzkukz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.haohaochexian.top/gtowaffgsn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hfpthk.cn/gtuotcswja.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xziqi.cn/gtamueieap.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.smart0.xyz/gtcrwzrgul.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.aibaodan.cn/gtwyzkycaf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xziqi.cn/gtmthpzalb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.meibo888.top/gtiovrblag.html

[L04] 设置超时
来源：http://hz.nwbrower.top/gtkrotllir.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ehwqpu.com/gtdnidouyx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinghuilouyu.cn/gtdcwcsira.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258.top/gtbtcxqmzu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ydjk.org.cn/gtnyqrjhyo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hysaishi.cn/gtafdbixzs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.haohaochexian.top/gttsrrabik.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gogol.net.cn/gtdysziifi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.kuanghao11.cn/gtemjrxqwk.html

[L05] 上传文件（multipart）
来源：http://hz.havefunace.top/gtixartrts.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xylfe.cn/gtsuhwfxiy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.smart0.xyz/gtctvfvvis.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.pengpengdd.cyou/gtfawueysi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yongpay.top/gtbageicyu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yanxiufei.cn/gtamupuowd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jyoumei.cn/gthkxbznqd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sweek.top/gtozhkrwyy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jqgfzy.top/gtojpfqzte.html

[L06] 解析响应为 JSON
来源：http://hz.jinqigfzy.top/gtrsgyibkn.html

Py:   resp.json()
来源：http://hz.shanyushiyangtech.top/gtrypqmelt.html

PHP:  json_decode($body, true);
来源：http://hz.zhaomingkeji.xyz/gtqfwmxkvr.html

JS:   await resp.json()
来源：http://hz.chenjidiqi.icu/gtcvtxbqow.html

TS:   await resp.json()
来源：http://hz.yuxming.cn/gtmglvpbos.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cucudq.cn/gtjdnpqibh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.svipenyu.cn/gttrnwqqqm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenlongwang.top/gtqzuddbpj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zdqjudy.top/gtwmyvbyou.html

[L07] 处理 HTTP 状态码
来源：http://hz.tian-w.cn/gtlemijqgw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.tian-w.cn/gtljmuvakp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sweek.top/gtpvrclryf.html

JS:   resp.ok;  resp.status
来源：http://hz.wangshuangyany.cn/gtfxnpfwhf.html

TS:   resp.ok;  resp.status
来源：http://hz.shzxlz.cn/gthggcmyke.html

Java: resp.statusCode()
来源：http://hz.zhaomingkeji.xyz/gtmkkmszyv.html

Go:   resp.StatusCode
来源：http://hz.xuanzx.com/gtnvrqsnhi.html

Ruby: resp.code.to_i
来源：http://hz.pengpengdd.cyou/gtoybedqyp.html

C#:   (int)resp.StatusCode
来源：http://hz.yanxiufei.cn/gtiijlfume.html

[L08] 并发请求多个地址
来源：http://hz.tian-w.cn/gtfcdicvxc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yuanzhike.top/gtezpksovs.html

PHP:  curl_multi_init() 系列
来源：http://hz.redwolf501.top/gtovhevaky.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tianlin.xyz/gttzgwvjcj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenjidiqi.icu/gteixilzzp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.bjfxy.top/gttknzudbe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.redwolf501.top/gtpmhfswfs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yongpay.top/gttngfgoov.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hysaishi.cn/gtfmtaohen.html

================================================================================
来源：http://hz.yangfankeji.com/gtfpaxwoku.html

M. 命令行 / 进程 / 环境
来源：http://hz.ydjk.org.cn/gthzctlerj.html

================================================================================
来源：http://hz.xylfe.cn/gtisgmhysh.html

[M01] 读取命令行参数
来源：http://hz.hnqzz.top/gtpmxoijcf.html

Py:   sys.argv[1:]
来源：http://hz.guannengcc.top/gtsdhmbzps.html

PHP:  $argv;  $argc;
来源：http://hz.sweek.top/gtjcsavrws.html

JS:   process.argv.slice(2)
来源：http://hz.hfpthk.cn/gtbkjkjcbo.html

TS:   process.argv.slice(2)
来源：http://hz.nanxinkj.top/gtgxtcgvwh.html

Java: args 数组（main 方法参数）
来源：http://hz.ehwqpu.com/gtulpqqqsj.html

Go:   os.Args[1:]
来源：http://hz.aizwys.cn/gtpqbtuoew.html

Ruby: ARGV
来源：http://hz.jinyuanbaomall.cn/gtbpydrjfq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.guannengcc.top/gtvhdycudy.html

[M02] 读取环境变量
来源：http://hz.shangyingyoupin.top/gttzphraof.html

Py:   os.environ.get("HOME")
来源：http://hz.zdqjudy.top/gtekfphzwo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenjidiqi.icu/gtsuhojefj.html

JS:   process.env.HOME
来源：http://hz.birdmap.top/gtzgbmzgvd.html

TS:   process.env.HOME
来源：http://hz.hnxiangtu.top/gtspjesdkf.html

Java: System.getenv("HOME")
来源：http://hz.zhijiandao.cn/gtprtehikb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yonumen.top/gtalezngct.html

Ruby: ENV["HOME"]
来源：http://hz.cdnleiting.top/gtnjwxwbmr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.pengpengdd.cyou/gtvfbvzppb.html

[M03] 执行外部命令
来源：http://hz.yuanzhike.top/gttvmmckli.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.tianlin.xyz/gtitpaxbzn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.snrcjt.cn/gtpuflfrjz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.mhx1999.top/gtjmfgggiq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangshuangyany.cn/gtwuiokpxg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hysaishi.cn/gtzweaklzy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hammf.cn/gtvatgmcww.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shanyushiyangtech.top/gtnwctjkvh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.tian-w.cn/gtbrehzigx.html

[M04] 获取当前工作目录
来源：http://hz.guowangkeji.top/gtjzgjjeda.html

Py:   os.getcwd()
来源：http://hz.haohaochexian.top/gtcjvkhxgk.html

PHP:  getcwd();
来源：http://hz.aizwys.cn/gthfmluoin.html

JS:   process.cwd()
来源：http://hz.pycfn.com/gtxhuzkraw.html

TS:   process.cwd()
来源：http://hz.yj202588.top/gtzmipposu.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zycfv.cn/gtdxljlmrs.html

Go:   os.Getwd()
来源：http://hz.316326.xyz/gtyxbsyovl.html

Ruby: Dir.pwd
来源：http://hz.cashguo.top/gtdzdyqfzh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cqqwz.cn/gtwcqzxdsu.html

[M05] 设置退出码
来源：http://hz.yvedp.cn/gtqwyqbear.html

Py:   sys.exit(1)
来源：http://hz.smart0.xyz/gtasvouojz.html

PHP:  exit(1);
来源：http://hz.xylfe.cn/gthetdjfgd.html

JS:   process.exit(1)
来源：http://hz.sysykeji.top/gtvdlaiqbs.html

TS:   process.exit(1)
来源：http://hz.52xcode.cn/gtfuunthkv.html

Java: System.exit(1)
来源：http://hz.yuxming.cn/gtncwdalwv.html

Go:   os.Exit(1)
来源：http://hz.yongpay.top/gtnjxpjqcz.html

Ruby: exit 1
来源：http://hz.yonumen.top/gtxndjhndd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shuidangran.top/gtjzlegsxp.html

[M06] 向标准错误输出
来源：http://hz.birdmap.top/gtolqbrgia.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cashguo.top/gtbgxmgxwr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ehwqpu.com/gtondehvip.html

JS:   console.error("err")
来源：http://hz.xuanzx.com/gtcyrddzva.html

TS:   console.error("err")
来源：http://hz.jyoumei.cn/gtxqhcmbem.html

Java: System.err.println("err")
来源：http://hz.zhixingplan.top/gtwwbnasik.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shangyingyoupin.top/gtkhfuyolw.html

Ruby: warn "err"
来源：http://hz.yj202588.top/gtzykfponn.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.kuanghao11.cn/gtcmfjgixf.html

[M07] 判断是否为主入口
来源：http://hz.tanke756.top/gtedhcreys.html

Py:   if __name__ == "__main__":
来源：http://hz.daria6918.cn/gtlmencrhs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinyuanbaomall.cn/gturerhfvj.html

JS:   require.main === module
来源：http://hz.cucudq.cn/gteoljvuwo.html

TS:   require.main === module
来源：http://hz.bjfxy.top/gtzwztsneu.html

Java: public static void main(String[] args)
来源：http://hz.aizwys.cn/gtvnvxupgj.html

Go:   func main()
来源：http://hz.guowangkeji.top/gtrelfmjde.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.guannengcc.top/gtnwqhdkuo.html

C#:   static void Main(string[] args)
来源：http://hz.meibo888.top/gtlzpsczkd.html

[M08] 获取系统与运行时信息
来源：http://hz.chenjidiqi.icu/gtrnhlrkji.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinqigfzy.top/gtchevjgme.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.pycfn.com/gtfyahmhru.html

JS:   process.platform;  process.version
来源：http://hz.feifeiyinyue.top/gtggtqkfww.html

TS:   process.platform;  process.version
来源：http://hz.jinqigufen.top/gtxonuzthw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yueranfly.top/gtbuctzptg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hysaishi.cn/gtupnccrfq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.316326.xyz/gtegjrbfuf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yanxiufei.cn/gtzjqjcwvb.html

================================================================================
来源：http://hz.vqdsnc.cn/gtqoyozbwm.html

N. 数据结构与算法
来源：http://hz.andypj.xyz/gtxkuwunfz.html

================================================================================
来源：http://hz.tian-w.cn/gttkpqgtrt.html

[N01] 二分查找（有序数组）
来源：http://hz.jqgufenzy.top/gthvtgaurg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.chenlongwang.top/gtwmektsxz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhengqikj.top/gtesrrrzct.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuanzx.com/gtcubzcqmt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yonumen.top/gtmknnomzk.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhiwuduotai.top/gtgpkedhqg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.pengpengdd.cyou/gtwbdtuxgc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.guowangkeji.top/gtjvvnzwsn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ppjwa.cn/gtibqqfdcy.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.meibo888.top/gtaiqzkeas.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.smart0.xyz/gtqugoudml.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.meibo888.top/gtyghupicr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hongshengwenyu.top/gtbxpzciyr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hywenlv.cn/gtcroqifbl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.snrcjt.cn/gtldlzidej.html

Go:   slices.Sort(arr)
来源：http://hz.cqqwz.cn/gtkvkmnnum.html

Ruby: arr.sort
来源：http://hz.xziqi.cn/gtdupevzsd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yvedp.cn/gthilwhgia.html

[N03] 快速排序（分治示例）
来源：http://hz.gzhubu.top/gtjbvqjanb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xziqi.cn/gtluprptfe.html

PHP:  // 递归实现，或用 usort
来源：http://hz.meibo888.top/gtidfpjavs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangshuangyany.cn/gtgejqtifb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxuanxn.top/gtsyuhrixb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hnqzz.top/gtvsaswjid.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shanyushiyangtech.top/gtuzfagztj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ybcxt.top/gtbgfzdtea.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yangfankeji.com/gtnwinwvuc.html

[N04] 斐波那契数列
来源：http://hz.yangfankeji.com/gttmmiymec.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.gotoacloud.top/gtxfotsfqx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.andypj.xyz/gtdnppwkxu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.feifeiyinyue.top/gtbxaksfhq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.vqdsnc.cn/gtteyyxyur.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.tanke756.top/gtpcpompgy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ywan-chungtsiang.top/gtqrtilebv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.wangdashe.top/gtsmbccjco.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yangfankeji.com/gtrpufwsri.html

[N05] 最大公约数
来源：http://hz.nanxinkj.top/gtlfwmotri.html

Py:   math.gcd(a, b)
来源：http://hz.chenzaomai.com/gtaljyomgo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.daria6918.cn/gtccspasak.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.0kj1m.cn/gtnrkkjivo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xingfuxueyuan.xyz/gtbkrhtygy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hongshengwenyu.top/gtostnxilv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sxryk.cn/gtztdffrvs.html

Ruby: a.gcd(b)
来源：http://hz.52xcode.cn/gtbyycgiwr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhoulong.xyz/gtrjsqixnj.html

[N06] 判断回文字符串
来源：http://hz.ydjk.org.cn/gtdpicakcp.html

Py:   s == s[::-1]
来源：http://hz.guannengcc.top/gtassenvlk.html

PHP:  $s === strrev($s);
来源：http://hz.hnxiangtu.top/gtbnkhsbow.html

JS:   s === [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtmkiueswm.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtqmxtvhlg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.0kj1m.cn/gtzdygctwp.html

Go:   // 双指针从两端比较
来源：http://hz.xuanzx.com/gtskgudfxw.html

Ruby: s == s.reverse
来源：http://hz.daxiang520.top/gtjcvvaaha.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.iojbl.cn/gtahmquaoe.html

[N07] 两数之和（返回下标）
来源：http://hz.ivvv.top/gtwhggvcvp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.wangshuangyany.cn/gtxsggpgtx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.aizwys.cn/gtilohpdgl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.wangdashe.top/gtmtcyhwza.html

TS:   // 手写 Map<string, number>
来源：http://hz.sweek.top/gtnvcvmgwe.html

Java: // 手写 HashMap
来源：http://hz.snrcjt.cn/gtbmkuyvpb.html

Go:   // 手写 map[int]int
来源：http://hz.chenzaomai.com/gtdwlmbkae.html

Ruby: // 手写 Hash
来源：http://hz.hammf.cn/gtqlydokzb.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.pycfn.com/gthlfvphgh.html

[N08] 生成全排列
来源：http://hz.sufxvd.cn/gtbgptpyre.html

Py:   itertools.permutations(arr)
来源：http://hz.daxiang520.top/gtosxywqlo.html

PHP:  // 手写递归交换
来源：http://hz.meibo888.top/gtqvpduntt.html

JS:   // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gttwskmujh.html

TS:   // 手写回溯递归
来源：http://hz.dianchejie.cn/gtzvapubzj.html

Java: // 手写回溯递归
来源：http://hz.ybcxt.top/gtxzjkatmq.html

Go:   // 手写回溯递归
来源：http://hz.yuxming.cn/gtkycvblxh.html

Ruby: arr.permutation.to_a
来源：http://hz.wangshuangyany.cn/gtgsbujxvt.html

C#:   // 手写回溯递归
来源：http://hz.redwolf501.top/gtqtgjsgbp.html

[N09] 栈与队列
来源：http://hz.jyoumei.cn/gtpcolcalz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yuxming.cn/gtzftkaarx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jianghu66.top/gtksrcnqyx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.andypj.xyz/gtawmbnefu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hywenlv.cn/gtjovnzlxv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.tian-w.cn/gtoduqgcqo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yanxiufei.cn/gtluldfomh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.smart0.xyz/gtueaszluq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinyuanbaomall.cn/gtiejdtjxk.html

[N10] 链表节点定义
来源：http://hz.shzxlz.cn/gtivrnphcy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xziqi.cn/gtsczidxua.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhoulong.xyz/gtoskbloij.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.haohaochexian.top/gtjecxrjqe.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cucudq.cn/gtolzbeyvj.html

Java: class Node { int v; Node next; }
来源：http://hz.cashguo.top/gtufizwzmy.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.kuanghao11.cn/gtiyohoecu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhongyouzk.top/gtxklucowb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xuetiantiany.cn/gttrwrsila.html

[N11] 二叉树中序遍历
来源：http://hz.zhongyouzk.top/gteuwshxap.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinqigfzy.top/gtxumfxvml.html

PHP:  // 手写递归函数
来源：http://hz.mhx1999.top/gtxyggxgea.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cheryme.top/gttaqgaang.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gaohongyu789.top/gtpgfrrwhn.html

Java: // 手写递归
来源：http://hz.bjfxy.top/gtjlrlncbu.html

Go:   // 手写递归
来源：http://hz.hammf.cn/gtczuekqeo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.pycfn.com/gtozrfawol.html

C#:   // 手写递归
来源：http://hz.yangfankeji.com/gtusobcbua.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ywan-chungtsiang.top/gtlncpefya.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.smart0.xyz/gtsyfotdmb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shzxlz.cn/gtcfjbdfdz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtldyqxqqt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sufxvd.cn/gtpghzzcdz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.bjfxy.top/gtgrvjavga.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hnxiangtu.top/gtrgggaozh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ywan-chungtsiang.top/gtoyslijfc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhixingplan.top/gtbhhvmyxw.html

================================================================================
来源：http://hz.jinqigufen.top/gtokykgcbd.html

O. 并发与异步
来源：http://hz.jinqigufen.top/gtlvxztcmh.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtjnlbgzhg.html

[O01] 启动一个线程
来源：http://hz.ehwqpu.com/gtttayrakt.html


<!-- 参考信息 -->