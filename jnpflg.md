代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tanke756.top/gttoyxdgbt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.andypj.xyz/gtlzzuftvs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.aibaodan.cn/gtmovxiezk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ppjwa.cn/gttemgzerh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jlsjyb.cn/gtlaizswqe.html

[K07] 进制转换
来源：http://hz.sufxvd.cn/gtwnecyyot.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj202588.top/gtyowkkqoa.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenjidiqi.icu/gtzyonyeqb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj202588.top/gtgnqcnaoq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yuanzhike.top/gteryfqupy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sysykeji.top/gtpnwghmol.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.kuanghao11.cn/gtwspjwlxv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xylfe.cn/gtiverseug.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.wangdashe.top/gtwgoebdjv.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj202588.top/gtawcnpcoe.html

Py:   pickle.dumps(obj)
来源：http://hz.shanyushiyangtech.top/gtxbunkhnk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yanxiufei.cn/gtwmwaesjb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shuidangran.top/gtqbjlqsgz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.andypj.xyz/gtylbwppqr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shuidangran.top/gtgybtyoro.html

Go:   encoding/gob
来源：http://hz.jinqigufen.top/gtkhfgnpck.html

Ruby: Marshal.dump(obj)
来源：http://hz.fengsongda.top/gtnhaeudre.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jianghu66.top/gtgzzrzgsw.html

================================================================================
来源：http://hz.wangdashe.top/gtznpdfiqs.html

L. 网络请求
来源：http://hz.sxryk.cn/gtdludhmdm.html

================================================================================
来源：http://hz.smart0.xyz/gtnyigxild.html

[L01] 发送 GET 请求
来源：http://hz.fengsongda.top/gthyxgvptw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cdnleiting.top/gtnefbbbfr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhijiandao.cn/gtklnqdomc.html

JS:   await fetch(url)
来源：http://hz.hnxiangtu.top/gtvzosbwlw.html

TS:   await fetch(url)
来源：http://hz.xuetiantiany.cn/gtsxpoaowe.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhongyouzk.top/gtcjxyqvij.html

Go:   resp, err := http.Get(url)
来源：http://hz.cashguo.top/gtvzfnwflf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ivvv.top/gtxlvgssfl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shanyushiyangtech.top/gtzqckphcw.html

[L02] 发送 POST JSON
来源：http://hz.gzhubu.top/gtvwxwdllp.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yuanzhike.top/gtsohdxwvs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.52xcode.cn/gthcviejvf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jlsjyb.cn/gthoobjzek.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.daria6918.cn/gtomhhuxtg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xuanzx.com/gtkuualcsd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.chenzaomai.com/gtxtwazeeb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.gzhubu.top/gtwfqrevxv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zdqjudy.top/gtohpjokrx.html

[L03] 设置自定义请求头
来源：http://hz.nwbrower.top/gtsernvkfo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhixingplan.top/gtlaxxaauv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gzhubu.top/gtwzflqzaa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenlongwang.top/gtvuybgqam.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sxryk.cn/gtvvclunuw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinqigfzy.top/gtridgumdj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.aizwys.cn/gthlpdqhze.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.0kj1m.cn/gtaviqfdyr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nwbrower.top/gtpvrbdqfe.html

[L04] 设置超时
来源：http://hz.ppjwa.cn/gtumlbvzgp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.c1oappe.top/gtttrywgaf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sysykeji.top/gtvcchtieq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.kuanghao11.cn/gtcthqgian.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ppjwa.cn/gtbtabmuov.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yj20258888.top/gtfxaooxdf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yuxming.cn/gtvxiollzm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xylfe.cn/gtgditdqsk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.andypj.xyz/gtdhjrhhct.html

[L05] 上传文件（multipart）
来源：http://hz.daxiang520.top/gtpebgacgb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.aizwys.cn/gtxskywpoj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ppjwa.cn/gtbkwlnqxf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.meibo888.top/gtwmdwhpbi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cashguo.top/gthzlpzvwb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhaomingkeji.xyz/gttomooicp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ydjk.org.cn/gtuygqelmx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cqqwz.cn/gtttxlbasb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.guowangkeji.top/gtxhbbxfpr.html

[L06] 解析响应为 JSON
来源：http://hz.yj20258.top/gtjrazkbtg.html

Py:   resp.json()
来源：http://hz.yongpay.top/gtcgqdqeyd.html

PHP:  json_decode($body, true);
来源：http://hz.nwbrower.top/gtoysbamda.html

JS:   await resp.json()
来源：http://hz.hammf.cn/gtbdavhbvh.html

TS:   await resp.json()
来源：http://hz.nanxinkj.top/gtuiuojpbm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yanxiufei.cn/gtwtptyybz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gaohongyu789.top/gtzcvvtthr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xuetiantiany.cn/gtkxtfacuc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.sxryk.cn/gtrscrolun.html

[L07] 处理 HTTP 状态码
来源：http://hz.hnxiangtu.top/gtcmpyssbr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hywenlv.cn/gtufzsjxvr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cucudq.cn/gtoyfgvuyr.html

JS:   resp.ok;  resp.status
来源：http://hz.svipenyu.cn/gtvnkmkjpf.html

TS:   resp.ok;  resp.status
来源：http://hz.pycfn.com/gtnvvvxtai.html

Java: resp.statusCode()
来源：http://hz.daxiang520.top/gtapvfbdna.html

Go:   resp.StatusCode
来源：http://hz.quarkkingdee.top/gtedzfkidw.html

Ruby: resp.code.to_i
来源：http://hz.xylfe.cn/gtffdvrxkv.html

C#:   (int)resp.StatusCode
来源：http://hz.aizwys.cn/gtmwwxkmpu.html

[L08] 并发请求多个地址
来源：http://hz.ehwqpu.com/gtqolzasii.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gaohongyu789.top/gtkaagbgtw.html

PHP:  curl_multi_init() 系列
来源：http://hz.jqgufenzy.top/gtxomchuld.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cdnleiting.top/gtqgxmnabh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtpgkuvfef.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.nwbrower.top/gtawxqxyma.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jqgufenzy.top/gtuftxepzp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.quarkkingdee.top/gtzntbribz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.chenjidiqi.icu/gteuuwxpko.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtbuozlxvu.html

M. 命令行 / 进程 / 环境
来源：http://hz.jinqigufen.top/gtpyolvryq.html

================================================================================
来源：http://hz.52xcode.cn/gthhbcuuqj.html

[M01] 读取命令行参数
来源：http://hz.hfpthk.cn/gtjvktfgcr.html

Py:   sys.argv[1:]
来源：http://hz.jyoumei.cn/gtiwonkeae.html

PHP:  $argv;  $argc;
来源：http://hz.0kj1m.cn/gtyjlyktlt.html

JS:   process.argv.slice(2)
来源：http://hz.yuxming.cn/gtsvpchoby.html

TS:   process.argv.slice(2)
来源：http://hz.yanxiufei.cn/gtogtuqalc.html

Java: args 数组（main 方法参数）
来源：http://hz.nwbrower.top/gttrnwnzxt.html

Go:   os.Args[1:]
来源：http://hz.zhoulong.xyz/gtdgpkxaml.html

Ruby: ARGV
来源：http://hz.nanxuanxn.top/gthqgrnjxx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yueranfly.top/gtxzgxdaja.html

[M02] 读取环境变量
来源：http://hz.cheryme.top/gtmwfzjfbp.html

Py:   os.environ.get("HOME")
来源：http://hz.nanxinkj.top/gtrozzmyia.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jlsjyb.cn/gtqsjqwaua.html

JS:   process.env.HOME
来源：http://hz.smart0.xyz/gtpyrrdqkt.html

TS:   process.env.HOME
来源：http://hz.andypj.xyz/gtmdvhphpo.html

Java: System.getenv("HOME")
来源：http://hz.zycfv.cn/gtxtbxdnbc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.c1oappe.top/gtuujxhseh.html

Ruby: ENV["HOME"]
来源：http://hz.snrcjt.cn/gtkpwoyoae.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cqqwz.cn/gtzfxznvna.html

[M03] 执行外部命令
来源：http://hz.quarkkingdee.top/gtcnsehsyu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.snrcjt.cn/gtqslwbcll.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ehwqpu.com/gtjzlryros.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.pycfn.com/gtrpohqhtz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.andypj.xyz/gtudmkptqn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.dashuyun.cn/gthuekview.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.pycfn.com/gtqziytoau.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhixingplan.top/gtiaxtwihn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhongyouzk.top/gtoxafecwf.html

[M04] 获取当前工作目录
来源：http://hz.pycfn.com/gtzmvkbkjb.html

Py:   os.getcwd()
来源：http://hz.xylfe.cn/gtepwonzou.html

PHP:  getcwd();
来源：http://hz.cucudq.cn/gtihkkvtti.html

JS:   process.cwd()
来源：http://hz.xylfe.cn/gtjrzawvln.html

TS:   process.cwd()
来源：http://hz.hammf.cn/gtbvsyznor.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ehwqpu.com/gtbyuipeko.html

Go:   os.Getwd()
来源：http://hz.cdnleiting.top/gtncfhmdjd.html

Ruby: Dir.pwd
来源：http://hz.zycfv.cn/gtilxvcuce.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.fzhhl.top/gtwsykjirl.html

[M05] 设置退出码
来源：http://hz.zhongyouzk.top/gttirfapzs.html

Py:   sys.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtvjrvmjyj.html

PHP:  exit(1);
来源：http://hz.pengpengdd.cyou/gtpoquyuse.html

JS:   process.exit(1)
来源：http://hz.jqgufenzy.top/gtthaveixy.html

TS:   process.exit(1)
来源：http://hz.tianlin.xyz/gtfweohtmq.html

Java: System.exit(1)
来源：http://hz.ppjwa.cn/gtaqfxxqlq.html

Go:   os.Exit(1)
来源：http://hz.ivvv.top/gtfvyezrhj.html

Ruby: exit 1
来源：http://hz.ppjwa.cn/gtoqojfqtw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cucudq.cn/gtxxbyqbte.html

[M06] 向标准错误输出
来源：http://hz.cheryme.top/gtorqmgrwk.html

Py:   print("err", file=sys.stderr)
来源：http://hz.c1oappe.top/gtplpyttxx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.316326.xyz/gtnzmbdwbl.html

JS:   console.error("err")
来源：http://hz.jyoumei.cn/gtekbzlfmy.html

TS:   console.error("err")
来源：http://hz.jyoumei.cn/gtcibaioqc.html

Java: System.err.println("err")
来源：http://hz.yvedp.cn/gtozompzmt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sufxvd.cn/gtuvtsgsni.html

Ruby: warn "err"
来源：http://hz.52xcode.cn/gtjsmrxvsq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.sufxvd.cn/gtbmgjayaw.html

[M07] 判断是否为主入口
来源：http://hz.daria6918.cn/gttrckktdx.html

Py:   if __name__ == "__main__":
来源：http://hz.ydzc1.top/gtgyhvmdmh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xylfe.cn/gthbcbpkaj.html

JS:   require.main === module
来源：http://hz.tian-w.cn/gtfdcxycrd.html

TS:   require.main === module
来源：http://hz.cheryme.top/gtvzoijbdq.html

Java: public static void main(String[] args)
来源：http://hz.ehwqpu.com/gtfhxrjuhv.html

Go:   func main()
来源：http://hz.sxryk.cn/gtteqrgxnt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yvedp.cn/gtkqqjgacc.html

C#:   static void Main(string[] args)
来源：http://hz.ppjwa.cn/gtaiokqull.html

[M08] 获取系统与运行时信息
来源：http://hz.zycfv.cn/gtmzcbypad.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jiagoushi.top/gtxfocqhsr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ydjk.org.cn/gtamcfduuv.html

JS:   process.platform;  process.version
来源：http://hz.tianlin.xyz/gtydryrlxu.html

TS:   process.platform;  process.version
来源：http://hz.zdqjudy.top/gtvhcjdrei.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jqgufenzy.top/gtewhywvlm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jyoumei.cn/gtsocamyby.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hammf.cn/gtsjjerrym.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hammf.cn/gtkmyflvoa.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtowpcejxi.html

N. 数据结构与算法
来源：http://hz.jinqigfzy.top/gtblayjmzt.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtepotqdeo.html

[N01] 二分查找（有序数组）
来源：http://hz.mhx1999.top/gtouyzmkos.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xinyue.icu/gtlhxivggx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ybcxt.top/gtflmjwcjl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shanyushiyangkeji.top/gtaaudnjbp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gotoacloud.top/gtiiygeojg.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hammf.cn/gtndplhuur.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhongyouzk.top/gtavaqfyvg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhoulong.xyz/gtagdupxoq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ehwqpu.com/gtvcpwngal.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.aibaodan.cn/gtqjxcrgkq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ywan-chungtsiang.top/gtmkdkzmpn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.dashuyun.cn/gtmctueebh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hysaishi.cn/gtvoneifyq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zdqjudy.top/gtmtscoqcs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yvedp.cn/gthifjktvw.html

Go:   slices.Sort(arr)
来源：http://hz.zhongyouzk.top/gtnkwkijpr.html

Ruby: arr.sort
来源：http://hz.nanxinkj.top/gtmkuicnbw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.daxiang520.top/gtobtfqtfi.html

[N03] 快速排序（分治示例）
来源：http://hz.shanyushiyangkeji.top/gtiajzwhgo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jlsjyb.cn/gtnzqoartz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gaohongyu789.top/gtdskrjwot.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xinyue.icu/gtfwvjoxbf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.meibo888.top/gtamkwaivd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hfpthk.cn/gtrylkezhw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.wangdashe.top/gtcqeirrrs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhengqikj.top/gtyzqjgtzt.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shanyushiyangtech.top/gtoxmrncab.html

[N04] 斐波那契数列
来源：http://hz.xuanzx.com/gtbobzvnwa.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jqgufenzy.top/gtzuvtttpe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jqgufenzy.top/gtajsnqhqv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnqzz.top/gtqlwbihuo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hysaishi.cn/gtvzmfxgfp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xingfuxueyuan.xyz/gtzatuepzs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.nanxinkj.top/gtjlbqdcet.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.52xcode.cn/gtcauxidlk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sufxvd.cn/gtjqhzucvt.html

[N05] 最大公约数
来源：http://hz.hywenlv.cn/gtzigbzsip.html

Py:   math.gcd(a, b)
来源：http://hz.kuanghao11.cn/gtkgmrtufy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.gotoacloud.top/gtftjmudne.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.meibo888.top/gtyuyerrfo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cashguo.top/gtxkmklity.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ydjk.org.cn/gteedyqwvn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhixingplan.top/gtvwejzivt.html

Ruby: a.gcd(b)
来源：http://hz.vqdsnc.cn/gtarahmtqq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jyoumei.cn/gtytrxwfzu.html

[N06] 判断回文字符串
来源：http://hz.zhijiandao.cn/gtbijwptny.html

Py:   s == s[::-1]
来源：http://hz.yueranfly.top/gtofasvypd.html

PHP:  $s === strrev($s);
来源：http://hz.hysaishi.cn/gtlpgpjuaz.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ydzc1.top/gtiupwvyrl.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtghmbvodm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hongshengwenyu.top/gtdhwitcdf.html

Go:   // 双指针从两端比较
来源：http://hz.yonumen.top/gtgzcbbysb.html

Ruby: s == s.reverse
来源：http://hz.yj20258888.top/gtkoqwdlnh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.smart0.xyz/gtayvsgskk.html

[N07] 两数之和（返回下标）
来源：http://hz.shanyushiyangkeji.top/gtoljfhtiq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jqgufenzy.top/gtaagrwwax.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.9152youxi.cn/gtgtcqfxkb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.0kj1m.cn/gtbpbalxlx.html

TS:   // 手写 Map<string, number>
来源：http://hz.havefunace.top/gttmilpjnk.html

Java: // 手写 HashMap
来源：http://hz.yongpay.top/gtzdhbndas.html

Go:   // 手写 map[int]int
来源：http://hz.sweek.top/gtrhrzokuy.html

Ruby: // 手写 Hash
来源：http://hz.0kj1m.cn/gtnwaiztyn.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hammf.cn/gtznxjikou.html

[N08] 生成全排列
来源：http://hz.jinqigufen.top/gtrefchhbh.html

Py:   itertools.permutations(arr)
来源：http://hz.cashguo.top/gtgpthcrro.html

PHP:  // 手写递归交换
来源：http://hz.xuanzx.com/gtjfybqmcv.html

JS:   // 手写回溯递归
来源：http://hz.52xcode.cn/gtyscsdycn.html

TS:   // 手写回溯递归
来源：http://hz.daxiang520.top/gtqhzqxotv.html

Java: // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtnyyierps.html

Go:   // 手写回溯递归
来源：http://hz.yuanzhike.top/gtzmuxseqp.html

Ruby: arr.permutation.to_a
来源：http://hz.daxiang520.top/gtvcvdwcht.html

C#:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtuyxqkgyn.html

[N09] 栈与队列
来源：http://hz.sysykeji.top/gtbzjgfzpt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.redwolf501.top/gtljsqtgud.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.gzhubu.top/gtiayxuxau.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.chenzaomai.com/gtllcsdipo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zdqjudy.top/gthynzlxnl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.fengsongda.top/gtojgasxax.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.smart0.xyz/gtbllbmjik.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cucudq.cn/gtbzbzanxo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xinyue.icu/gtnqpncgep.html

[N10] 链表节点定义
来源：http://hz.smart0.xyz/gtccewmcnq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.iojbl.cn/gtgxkeqkag.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.52xcode.cn/gtvupanjjp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ehwqpu.com/gtojizuvmj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xuetiantiany.cn/gtdgmphcgs.html

Java: class Node { int v; Node next; }
来源：http://hz.xylfe.cn/gtrxerunel.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jlsjyb.cn/gtmgyjekcj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sysykeji.top/gtaronekvj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.tian-w.cn/gtcidhmcmz.html

[N11] 二叉树中序遍历
来源：http://hz.tanke756.top/gtmczovraj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hfpthk.cn/gtupyrcmyp.html

PHP:  // 手写递归函数
来源：http://hz.zdqjudy.top/gtqztcgbgh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jiagoushi.top/gtafiaepjk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhoulong.xyz/gtwsctcpas.html

Java: // 手写递归
来源：http://hz.andypj.xyz/gtjvsfywzd.html

Go:   // 手写递归
来源：http://hz.aizwys.cn/gttttrlckf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cheryme.top/gtzwhyhqca.html

C#:   // 手写递归
来源：http://hz.nanxuanxn.top/gtxurilztu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yongpay.top/gtopqyvawb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.nanxuanxn.top/gtevhnkwhg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gotoacloud.top/gtkdrblxyq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aibaodan.cn/gtdnwpwreq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tianlin.xyz/gthviyfvej.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigfzy.top/gttzzjyjfn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xuanzx.com/gtpyozalxq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ehwqpu.com/gtzkpvxxdu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangshuangyany.cn/gtwcrorure.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtrlctetqf.html

O. 并发与异步
来源：http://hz.ppjwa.cn/gtypjabgtr.html

================================================================================
来源：http://hz.gotoacloud.top/gtpcgsspvf.html

[O01] 启动一个线程
来源：http://hz.hongshengwenyu.top/gtjdgvcqau.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xuetiantiany.cn/gttzboxqfg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ivvv.top/gtztquxswn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xingfuxueyuan.xyz/gtthkpgbim.html

TS:   // 同 JS
来源：http://hz.ivvv.top/gtimuilasa.html

Java: new Thread(() -> f()).start()
来源：http://hz.yongpay.top/gtclmdykzw.html

Go:   go f()
来源：http://hz.gotoacloud.top/gtadjujkss.html

Ruby: Thread.new { f }
来源：http://hz.aizwys.cn/gtfvpjfuhf.html

C#:   Task.Run(() => F());
来源：http://hz.snrcjt.cn/gtdseqazht.html

[O02] 使用线程池
来源：http://hz.xylfe.cn/gttslzhmly.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.pycfn.com/gtapvlnkcm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.guannengcc.top/gtbjxushqz.html

JS:   // worker_threads 线程池
来源：http://hz.shanyushiyangkeji.top/gtraydphqy.html


<!-- 参考信息 -->