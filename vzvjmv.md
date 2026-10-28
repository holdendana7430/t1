代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.quarkkingdee.top/gtkidolnuz.html

TS:   s.split(",")
来源：http://hz.feifeiyinyue.top/gtigugnjuj.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhoulong.xyz/gtvnibaeil.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sweek.top/gtymwqecdl.html

Ruby: s.split(",");  s.split
来源：http://hz.quarkkingdee.top/gtnmszbcfe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hongshengwenyu.top/gtbzdxokak.html

[E08] 数组按分隔符合并
来源：http://hz.yanxiufei.cn/gtthabahwy.html

Py:   ",".join(items)
来源：http://hz.yuxming.cn/gtyrabagxy.html

PHP:  implode(",", $items);
来源：http://hz.shuidangran.top/gtencymhjj.html

JS:   items.join(",")
来源：http://hz.dianchejie.cn/gtydvdwtnb.html

TS:   items.join(",")
来源：http://hz.zhoulong.xyz/gtznrakeqc.html

Java: String.join(",", items)
来源：http://hz.aibaodan.cn/gtlbbrzufu.html

Go:   strings.Join(items, ",")
来源：http://hz.cucudq.cn/gtycrqjski.html

Ruby: items.join(",")
来源：http://hz.hysaishi.cn/gttilachmp.html

C#:   string.Join(",", items)
来源：http://hz.fengsongda.top/gtklagwfhi.html

[E09] 去除所有空白字符
来源：http://hz.yj20258.top/gtvalybcmu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jiagoushi.top/gtvkdmbwhw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.snrcjt.cn/gthrvzzmfv.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yj20258888.top/gtuawuqxdq.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ydjk.org.cn/gttxmisvhb.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jqgufenzy.top/gtrenfrqdn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yuanzhike.top/gtvydjflnf.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.tian-w.cn/gtxnljocin.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.quarkkingdee.top/gtpnrylxtc.html

[E10] 左侧补零 / 定长填充
来源：http://hz.andypj.xyz/gtrtmhuutv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.mhx1999.top/gtsasgnjqr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhongyouzk.top/gtzdwukgkl.html

JS:   "7".padStart(3, "0")
来源：http://hz.havefunace.top/gtbdaquvum.html

TS:   "7".padStart(3, "0")
来源：http://hz.ywan-chungtsiang.top/gtdpoarrfq.html

Java: String.format("%03d", 7)
来源：http://hz.cashguo.top/gtcgsfzvjj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yuanzhike.top/gtcoiowhzf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hnxiangtu.top/gtbeheoscu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.aizwys.cn/gtnvmretif.html

[E11] 反转字符串
来源：http://hz.jinqigufen.top/gtjtfsweqh.html

Py:   s[::-1]
来源：http://hz.sysykeji.top/gtpvlatdql.html

PHP:  strrev($s);
来源：http://hz.cqqwz.cn/gtkpklrhnk.html

JS:   [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtfgivrssy.html

TS:   [...s].reverse().join("")
来源：http://hz.hywenlv.cn/gtqjwktfdk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yuxming.cn/gthbugqygr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.tian-w.cn/gtwqeywnqj.html

Ruby: s.reverse
来源：http://hz.tianlin.xyz/gtikdsaebq.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hysaishi.cn/gtdqvhskbw.html

[E12] 统计某字符出现次数
来源：http://hz.zhijiandao.cn/gtiszsqxcb.html

Py:   s.count("a")
来源：http://hz.jinghuilouyu.cn/gtowweyeqa.html

PHP:  substr_count($s, "a");
来源：http://hz.yangfankeji.com/gtawrpffym.html

JS:   s.split("a").length - 1
来源：http://hz.jinyuanbaomall.cn/gtzdjaynwj.html

TS:   s.split("a").length - 1
来源：http://hz.zhixingplan.top/gteacykfis.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yvedp.cn/gtmefmqyof.html

Go:   strings.Count(s, "a")
来源：http://hz.zhongyouzk.top/gtytwbtazy.html

Ruby: s.count("a")
来源：http://hz.jianghu66.top/gtzgqewxje.html

C#:   s.Count(c => c == 'a')
来源：http://hz.nwbrower.top/gtvbdgdhnk.html

[E13] 逐字符遍历
来源：http://hz.sweek.top/gtcozcdqgl.html

Py:   for ch in s: print(ch)
来源：http://hz.iojbl.cn/gtqxidnkzi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinghuilouyu.cn/gtzcoebyjj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.kuanghao11.cn/gtzkfklwbw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xziqi.cn/gthxfnmbwu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gzhubu.top/gtuvirffzi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yuanzhike.top/gtppjcmidx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yvedp.cn/gtdbumsipt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.svipenyu.cn/gtkqwectxr.html

[E14] URL 编码与 Base64
来源：http://hz.feifeiyinyue.top/gtyzmzmjpz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.iojbl.cn/gtzxxfriji.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xuetiantiany.cn/gtwteyauzi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.chenzaomai.com/gtlcfjtlem.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.chenjidiqi.icu/gtfmofbcli.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.gzhubu.top/gtfgwjwpmz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cucudq.cn/gthueoynrz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.wangshuangyany.cn/gttemrmhse.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xingfuxueyuan.xyz/gtswwzzlot.html

[E15] HTML 转义 / 反转义
来源：http://hz.tanke756.top/gtfxikaxlh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhijiandao.cn/gtnmavkxlv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.0kj1m.cn/gthvbdppnd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.nwbrower.top/gtsmuaadyh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.dianchejie.cn/gtqyxmiiql.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.aibaodan.cn/gtwwfwlici.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.redwolf501.top/gtqnknfaur.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.nanxuanxn.top/gtjoxcjkhc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhijiandao.cn/gttwxyibpp.html

[E16] 数字千分位
来源：http://hz.daxiang520.top/gteetixemw.html

Py:   f"{1234567:,}"
来源：http://hz.birdmap.top/gtbucjdibw.html

PHP:  number_format(1234567);
来源：http://hz.hnxiangtu.top/gtqdjjqigw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.smart0.xyz/gtjncvoyaa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinghuilouyu.cn/gtqvviiidt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xinyue.icu/gtqqvxqdsd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.iojbl.cn/gthowvrtvo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yanxiufei.cn/gtclezelpa.html

C#:   1234567.ToString("N0")
来源：http://hz.shanyushiyangtech.top/gtwyhaapfs.html

[E17] 首字母大写
来源：http://hz.shuidangran.top/gtzarnajol.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nanxuanxn.top/gtehxnjiba.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.wangdashe.top/gtjzxrbqvo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinyuanbaomall.cn/gtdyjcfqkx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258888.top/gtzyizsxwd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.aibaodan.cn/gtqtfcpsfn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.daxiang520.top/gtoyihofff.html

Ruby: s.capitalize
来源：http://hz.jlsjyb.cn/gtozkutkxb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yangfankeji.com/gtatlnivgn.html

[E18] 模板占位符替换
来源：http://hz.jinqigufen.top/gtwlenvcne.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hywenlv.cn/gtdkbnbcrm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinqigufen.top/gtflwbnfvf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shzxlz.cn/gtshxmerbe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cqqwz.cn/gtwpqnwdol.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.meibo888.top/gtausrznsk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.mhx1999.top/gtttajutcx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yuxming.cn/gtemgvuyzy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.shuidangran.top/gtqyvaevuu.html

[E19] 多行文本按行拆分
来源：http://hz.haohaochexian.top/gtarsvubkm.html

Py:   s.splitlines()
来源：http://hz.shuidangran.top/gtcjtgjitc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.pengpengdd.cyou/gttsceywui.html

JS:   s.split(/\r?\n/)
来源：http://hz.jqgufenzy.top/gtzfkujopo.html

TS:   s.split(/\r?\n/)
来源：http://hz.fengsongda.top/gtefeckfrf.html

Java: s.lines().toList()
来源：http://hz.chenzaomai.com/gtergqxuey.html

Go:   strings.Split(s, "\n")
来源：http://hz.xingfuxueyuan.xyz/gtofjsrddm.html

Ruby: s.lines
来源：http://hz.xuetiantiany.cn/gtiflqhiqd.html

C#:   s.Split('\n')
来源：http://hz.zycfv.cn/gthipesszb.html

[E20] 判断字符串是否为空
来源：http://hz.jinyuanbaomall.cn/gtjyuhyvll.html

Py:   if not s:
来源：http://hz.zhoulong.xyz/gtefwjygwx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.tian-w.cn/gtqtykhenw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.snrcjt.cn/gtamkljzzt.html

TS:   if (s === "") {}
来源：http://hz.fengsongda.top/gtscxzehut.html

Java: if (s.isEmpty()) {}
来源：http://hz.jinyuanbaomall.cn/gtmrbcnvfb.html

Go:   if s == "" {}
来源：http://hz.yanxiufei.cn/gtexbvwxli.html

Ruby: if s.empty?
来源：http://hz.tianlin.xyz/gtckgpthyj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cqqwz.cn/gtfoypwnfv.html

[E21] 超长截断加省略号
来源：http://hz.bjfxy.top/gtltwaakah.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hysaishi.cn/gtypkjwtog.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.tianlin.xyz/gtmdsfudqf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sysykeji.top/gtcixekklt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.redwolf501.top/gtuqviudab.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.daxiang520.top/gtcyoqzyej.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tian-w.cn/gtjiybgqat.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yvedp.cn/gtwhilhwyx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.vqdsnc.cn/gtmpjewtmd.html

[E22] 字节长度与字符长度
来源：http://hz.svipenyu.cn/gtlsaqkkal.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yangfankeji.com/gtgbcndlnn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.birdmap.top/gtxrlcyelt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenjidiqi.icu/gtttjcqatu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangkeji.top/gthmgzjiaa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gogol.net.cn/gtbbblpjyn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.tanke756.top/gtaxstnbbe.html

Ruby: s.bytesize;  s.length
来源：http://hz.shzxlz.cn/gtouwmkxkz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.smart0.xyz/gtwqpizhpa.html

================================================================================
来源：http://hz.yvedp.cn/gtykziymjv.html

F. 文件与目录
来源：http://hz.bjfxy.top/gtihlczzwx.html

================================================================================
来源：http://hz.sufxvd.cn/gtdjttravp.html

[F01] 读取整个文件
来源：http://hz.jqgfzy.top/gtrarnqgyw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.pycfn.com/gtdkmksbzk.html

PHP:  file_get_contents("a.txt");
来源：http://hz.snrcjt.cn/gtjdaddcpe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hfpthk.cn/gtgomkadrl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.52xcode.cn/gtbifrahsp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtnnqqkpdp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jiagoushi.top/gtbcechytk.html

Ruby: File.read("a.txt")
来源：http://hz.mhx1999.top/gtcqckwwfl.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhongyouzk.top/gthfzkkvld.html

[F02] 逐行读取文件
来源：http://hz.hfpthk.cn/gtssqssitq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.chenlongwang.top/gthnuecjaj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xziqi.cn/gtykslprzz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.bjfxy.top/gtyjwvswzb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yangfankeji.com/gtpccnqtxv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nanxuanxn.top/gtcvtzlgao.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zycfv.cn/gtzprtukkm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hfpthk.cn/gtpxdtjiln.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xuanzx.com/gttbfqrvuq.html

[F03] 写入文件（覆盖）
来源：http://hz.yongpay.top/gtknhzuufk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.nwbrower.top/gtuwfrfcyj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.smart0.xyz/gtiffoxaxa.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258888.top/gtndvnmnqd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sweek.top/gtogqtxwbw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yj20258.top/gtapwpknwc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ivvv.top/gtszwatdvv.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.pengpengdd.cyou/gtxsohpqgy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yanxiufei.cn/gtacyuuubo.html

[F04] 追加写入文件
来源：http://hz.yj202588.top/gthijnuflc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.dashuyun.cn/gtnsqwkneu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.pycfn.com/gtsgefqjoo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinghuilouyu.cn/gttmgfpaah.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.bjfxy.top/gtpbrseevw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.meibo888.top/gtvlvicsai.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.gzhubu.top/gtnezqzsmc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.sxryk.cn/gtncqfzqnr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hnqzz.top/gttgmxrmsc.html

[F05] 判断文件或目录是否存在
来源：http://hz.ybcxt.top/gtlwptkjxa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jqgufenzy.top/gtxgtyjjvg.html

PHP:  file_exists("a.txt");
来源：http://hz.nwbrower.top/gtudbgcltz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.meibo888.top/gtkjmeokou.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xuanzx.com/gtnetxakxn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtgmtdtzkr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhijiandao.cn/gtdicqlofc.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhoulong.xyz/gthapqoxyf.html

C#:   File.Exists("a.txt")
来源：http://hz.yueranfly.top/gtnqsurpmk.html

[F06] 删除文件
来源：http://hz.cdnleiting.top/gtcgjmfhbu.html

Py:   os.remove("a.txt")
来源：http://hz.andypj.xyz/gtdcuntcgn.html

PHP:  unlink("a.txt");
来源：http://hz.zhoulong.xyz/gtcilgskyj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxinkj.top/gtitakmqsa.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.svipenyu.cn/gtqpzbqrfn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtisfwtjho.html

Go:   os.Remove("a.txt")
来源：http://hz.jinghuilouyu.cn/gtrawoagkd.html

Ruby: File.delete("a.txt")
来源：http://hz.andypj.xyz/gthjnvkiwm.html

C#:   File.Delete("a.txt");
来源：http://hz.yangfankeji.com/gtxowclrfm.html

[F07] 创建目录（含多级）
来源：http://hz.kuanghao11.cn/gtnjmbwdzx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.9152youxi.cn/gteodatvql.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zycfv.cn/gtvbksuydq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.guowangkeji.top/gtjqezsrby.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ybcxt.top/gteahgbbcq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.c1oappe.top/gtuevmzrov.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.smart0.xyz/gtwneisboj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ivvv.top/gtawydewuo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinqigfzy.top/gtugafgdhm.html

[F08] 遍历目录
来源：http://hz.sysykeji.top/gtbcvvhlfy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.52xcode.cn/gtzjmsvyxd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jyoumei.cn/gtdxktmgth.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhongyouzk.top/gtlaagyntr.html

TS:   fs.readdirSync("dir")
来源：http://hz.ywan-chungtsiang.top/gtczursflc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hywenlv.cn/gtenvxjaee.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jqgufenzy.top/gtxbcqqflr.html

Ruby: Dir.children("dir")
来源：http://hz.chenzaomai.com/gtxuvvpnbs.html

C#:   Directory.GetFiles("dir")
来源：http://hz.quarkkingdee.top/gtecwzrwqh.html

[F09] 获取文件大小
来源：http://hz.sysykeji.top/gtxjkysgdr.html

Py:   os.path.getsize("a.txt")
来源：http://hz.fzhhl.top/gtwputvxko.html

PHP:  filesize("a.txt");
来源：http://hz.ehwqpu.com/gtlzbpxcmn.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yueranfly.top/gtmrghbmwk.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ppjwa.cn/gtajvqijkr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.chenzaomai.com/gtpussnanp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hfpthk.cn/gtblexvadj.html

Ruby: File.size("a.txt")
来源：http://hz.yonumen.top/gtgigjzajc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hnxiangtu.top/gtzzvolray.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yuanzhike.top/gtpkuuaqjg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.mhx1999.top/gttublwvir.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinghuilouyu.cn/gtrvjwjncm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtgmrdjjrl.html

TS:   path.extname("a.txt")
来源：http://hz.gogol.net.cn/gtlnurrsbr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zdqjudy.top/gtbtvqauxc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cashguo.top/gthtbtzppo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.sxryk.cn/gtskawfydj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nanxinkj.top/gtfhgktwbm.html

[F11] 复制与移动文件
来源：http://hz.fzhhl.top/gthywolrsg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gtfuqkvyxh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ppjwa.cn/gtaofhjqap.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtqrnacaji.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gtjilbogjj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.haohaochexian.top/gtqmregwme.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.gotoacloud.top/gtqkkkmrej.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cashguo.top/gtctczagtp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gaohongyu789.top/gtdjtxgemm.html

[F12] CSV 读写
来源：http://hz.iojbl.cn/gtyytgrfag.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hnxiangtu.top/gtyfdtdvbg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.pycfn.com/gtpkimwxhy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jlsjyb.cn/gtlengddtg.html

TS:   // 同上
来源：http://hz.yj20258.top/gtddxnxgli.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jqgfzy.top/gttrjdahot.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.kuanghao11.cn/gtanrougau.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ybcxt.top/gtasowdtek.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ydzc1.top/gtigeevanq.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtpkiyxvfh.html

G. 面向对象
来源：http://hz.yj202588.top/gtijjrcdqx.html

================================================================================
来源：http://hz.jinqigufen.top/gtkfybizna.html

[G01] 定义类
来源：http://hz.sufxvd.cn/gtydfipxrd.html

Py:   class User: pass
来源：http://hz.yj20258.top/gteqoaptkc.html

PHP:  class User {}
来源：http://hz.meibo888.top/gtizrszaee.html

JS:   class User {}
来源：http://hz.pycfn.com/gtgdwjipqb.html

TS:   class User { name: string = ""; }
来源：http://hz.ivvv.top/gtntipluln.html

Java: class User {}
来源：http://hz.havefunace.top/gtzdljkggs.html

Go:   type User struct { Name string }
来源：http://hz.chenzaomai.com/gtbfrofhwy.html

Ruby: class User; end
来源：http://hz.jyoumei.cn/gtzricthrc.html

C#:   class User {}
来源：http://hz.yueranfly.top/gtrzyzinik.html

[G02] 构造函数
来源：http://hz.jqgufenzy.top/gtkuqiedpu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cdnleiting.top/gthbruhrhm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hnxiangtu.top/gtwjusjobp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhongyouzk.top/gtkeupnaeu.html

TS:   constructor(public name: string) {}
来源：http://hz.birdmap.top/gtdvgqnyft.html

Java: User(String name) { this.name = name; }
来源：http://hz.nanxuanxn.top/gtqstimwms.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jianghu66.top/gtntjifehp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aizwys.cn/gtcvpbyhuw.html

C#:   public User(string name) { Name = name; }
来源：http://hz.feifeiyinyue.top/gterfjcxbo.html

[G03] 实例属性
来源：http://hz.aibaodan.cn/gtgpmkalat.html

Py:   self.name = "x"
来源：http://hz.iojbl.cn/gtkvolwlsr.html

PHP:  public string $name = "x";
来源：http://hz.haohaochexian.top/gthlfyyhdw.html

JS:   this.name = "x";
来源：http://hz.smart0.xyz/gtddtysnwn.html

TS:   name: string = "x";
来源：http://hz.fzhhl.top/gtcsodnzcp.html

Java: private String name;
来源：http://hz.hnqzz.top/gtrejbwbia.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.c1oappe.top/gtkxcveofv.html

Ruby: @name = "x"
来源：http://hz.chenzaomai.com/gthhroiskg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.fengsongda.top/gtqgxvpcis.html

[G04] 定义方法
来源：http://hz.sufxvd.cn/gtdsrohkgf.html

Py:   def greet(self): return self.name
来源：http://hz.yvedp.cn/gtgjjypgnp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtbqfieinc.html

JS:   greet() { return this.name; }
来源：http://hz.gogol.net.cn/gtocvpulsk.html

TS:   greet(): string { return this.name; }
来源：http://hz.yuxming.cn/gtfgyveumh.html

Java: String greet() { return name; }
来源：http://hz.jqgfzy.top/gtzitgtjlb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cashguo.top/gtzfmnsowu.html

Ruby: def greet; @name; end
来源：http://hz.shanyushiyangkeji.top/gtmnuexefu.html

C#:   public string Greet() => Name;
来源：http://hz.wangdashe.top/gttugykzln.html

[G05] 继承
来源：http://hz.zhoulong.xyz/gtbphtqykk.html

Py:   class Admin(User): pass
来源：http://hz.yangfankeji.com/gtrfvodmlu.html

PHP:  class Admin extends User {}
来源：http://hz.sufxvd.cn/gtobgghjvz.html

JS:   class Admin extends User {}
来源：http://hz.guannengcc.top/gtrnvkpowv.html

TS:   class Admin extends User {}
来源：http://hz.zycfv.cn/gtjodbixum.html

Java: class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtbnsposyt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.haohaochexian.top/gtweyijmrq.html

Ruby: class Admin < User; end
来源：http://hz.bjfxy.top/gtgeoxbmqw.html

C#:   class Admin : User {}
来源：http://hz.ehwqpu.com/gtwuqzcdyt.html


<!-- 参考信息 -->