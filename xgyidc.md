代发 wailian999

PHP:  implode(",", $items);
来源：http://hz.hnxiangtu.top/gtvfibzape.html

JS:   items.join(",")
来源：http://hz.shzxlz.cn/gtehyfmpmo.html

TS:   items.join(",")
来源：http://hz.aizwys.cn/gtnccqayeu.html

Java: String.join(",", items)
来源：http://hz.guowangkeji.top/gthwjimncf.html

Go:   strings.Join(items, ",")
来源：http://hz.ppjwa.cn/gthnhqirju.html

Ruby: items.join(",")
来源：http://hz.dianchejie.cn/gtskbbvycc.html

C#:   string.Join(",", items)
来源：http://hz.birdmap.top/gtkuprctni.html

[E09] 去除所有空白字符
来源：http://hz.haohaochexian.top/gthraffmjh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ybcxt.top/gtpatpoodv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.fzhhl.top/gtykfwolro.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.gotoacloud.top/gtxdoolhjw.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jianghu66.top/gtlftcdjaf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yj20258.top/gtvntnsqzs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yangfankeji.com/gtkujmgmhh.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.dashuyun.cn/gtnwauebku.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.smart0.xyz/gtioqgqvxj.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yuanzhike.top/gttfaurhlj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.mhx1999.top/gtiqhxgzfg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.cheryme.top/gticdfmuvr.html

JS:   "7".padStart(3, "0")
来源：http://hz.fzhhl.top/gtplszhwmi.html

TS:   "7".padStart(3, "0")
来源：http://hz.gzhubu.top/gtxniramdl.html

Java: String.format("%03d", 7)
来源：http://hz.nanxuanxn.top/gtuxzmjbqs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zdqjudy.top/gtghzbqfzg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hongshengwenyu.top/gtgidqfqbf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.haohaochexian.top/gtnsgizthr.html

[E11] 反转字符串
来源：http://hz.shuidangran.top/gthglpbozy.html

Py:   s[::-1]
来源：http://hz.zhiwuduotai.top/gttstwjfvt.html

PHP:  strrev($s);
来源：http://hz.zhongyouzk.top/gtwgvlihnf.html

JS:   [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtyzdngwos.html

TS:   [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtnpmtremc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yueranfly.top/gtpzomqukj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.dianchejie.cn/gtethkifww.html

Ruby: s.reverse
来源：http://hz.jqgfzy.top/gtyrehctfd.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.sweek.top/gtvwdekfaw.html

[E12] 统计某字符出现次数
来源：http://hz.nanxinkj.top/gtvsumlgzb.html

Py:   s.count("a")
来源：http://hz.yanxiufei.cn/gtfaxwvtkv.html

PHP:  substr_count($s, "a");
来源：http://hz.zdqjudy.top/gtfsxcjace.html

JS:   s.split("a").length - 1
来源：http://hz.ydjk.org.cn/gttuhzufce.html

TS:   s.split("a").length - 1
来源：http://hz.zhiwuduotai.top/gtnzwctyel.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ybcxt.top/gtjkdjqkum.html

Go:   strings.Count(s, "a")
来源：http://hz.hnxiangtu.top/gtlowhxcio.html

Ruby: s.count("a")
来源：http://hz.jqgfzy.top/gtdoausfqm.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhiwuduotai.top/gtycrxryat.html

[E13] 逐字符遍历
来源：http://hz.xingfuxueyuan.xyz/gtjhbaetxm.html

Py:   for ch in s: print(ch)
来源：http://hz.ybcxt.top/gtergihuoq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.bjfxy.top/gtjpkylyzt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258.top/gtjynqyydw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hysaishi.cn/gtcodvqayc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yangfankeji.com/gtafzglvhl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.tanke756.top/gtsmcjvfqu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jqgfzy.top/gtbfrwxiki.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.nwbrower.top/gtxevpedcm.html

[E14] URL 编码与 Base64
来源：http://hz.yvedp.cn/gtjhzurxgg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.52xcode.cn/gtzxxabebq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinghuilouyu.cn/gtnzwwlfde.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.dashuyun.cn/gtknduhyfj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xylfe.cn/gticpsheyb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ywan-chungtsiang.top/gttmaensyy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhoulong.xyz/gtdhyxchsc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhiwuduotai.top/gtqyzooekr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jinghuilouyu.cn/gtflkkabrw.html

[E15] HTML 转义 / 反转义
来源：http://hz.yangfankeji.com/gtjcfvbxds.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.chenjidiqi.icu/gtdkphgyix.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jinghuilouyu.cn/gtjnqieqkk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zycfv.cn/gtapywwzbh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.havefunace.top/gttvwodien.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zdqjudy.top/gteorblpsv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.guannengcc.top/gtzcpzsyhs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yj20258888.top/gtnuesmkfz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ehwqpu.com/gtdcesalzl.html

[E16] 数字千分位
来源：http://hz.zhijiandao.cn/gtfbdcyduo.html

Py:   f"{1234567:,}"
来源：http://hz.guannengcc.top/gttahwzasb.html

PHP:  number_format(1234567);
来源：http://hz.ivvv.top/gtimuflgcy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sxryk.cn/gtkhoqetuw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydjk.org.cn/gtscwkcbqk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zdqjudy.top/gtpvzsajdt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.mhx1999.top/gtpovirjep.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gaohongyu789.top/gtiichchhq.html

C#:   1234567.ToString("N0")
来源：http://hz.xylfe.cn/gtyxbrmeha.html

[E17] 首字母大写
来源：http://hz.aizwys.cn/gtpykwgfep.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xuanzx.com/gtwlgtuipl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.chenjidiqi.icu/gttgtgtood.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.c1oappe.top/gtqdivrvew.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dianchejie.cn/gtkgdazvqd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.haohaochexian.top/gtjxvwxxrg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xingfuxueyuan.xyz/gtemgjylrd.html

Ruby: s.capitalize
来源：http://hz.xylfe.cn/gtmfyhqext.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yanxiufei.cn/gtunnzeagh.html

[E18] 模板占位符替换
来源：http://hz.xinyue.icu/gtdxgjsmgp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jinghuilouyu.cn/gtdilwsgmw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xuanzx.com/gtenpgqntf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.daria6918.cn/gthsszsjrx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtltxdrfma.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhiwuduotai.top/gtsvgidwpw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.nanxuanxn.top/gteilvtkes.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hammf.cn/gtctwnwblq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.kuanghao11.cn/gtvgaummgc.html

[E19] 多行文本按行拆分
来源：http://hz.dianchejie.cn/gtejdbticq.html

Py:   s.splitlines()
来源：http://hz.jiagoushi.top/gtmgcjvqln.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yj202588.top/gtzapguisg.html

JS:   s.split(/\r?\n/)
来源：http://hz.dianchejie.cn/gtyktckmde.html

TS:   s.split(/\r?\n/)
来源：http://hz.gotoacloud.top/gtyxyhxxxg.html

Java: s.lines().toList()
来源：http://hz.jqgfzy.top/gtnprjkquo.html

Go:   strings.Split(s, "\n")
来源：http://hz.0kj1m.cn/gttgzrmcbk.html

Ruby: s.lines
来源：http://hz.gaohongyu789.top/gtonmqhctu.html

C#:   s.Split('\n')
来源：http://hz.chenlongwang.top/gtxoceshbv.html

[E20] 判断字符串是否为空
来源：http://hz.yvedp.cn/gtnfydpcgi.html

Py:   if not s:
来源：http://hz.nwbrower.top/gtgyxauhmn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.dashuyun.cn/gtbdthfuiy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zdqjudy.top/gtbyvmpzjh.html

TS:   if (s === "") {}
来源：http://hz.sweek.top/gtuncgjpxc.html

Java: if (s.isEmpty()) {}
来源：http://hz.svipenyu.cn/gtfaodjwcj.html

Go:   if s == "" {}
来源：http://hz.zhongyouzk.top/gtsntpndcs.html

Ruby: if s.empty?
来源：http://hz.zhengqikj.top/gtcomyxeot.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.feifeiyinyue.top/gtpnpnvgdr.html

[E21] 超长截断加省略号
来源：http://hz.shzxlz.cn/gtfplclozc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yongpay.top/gtgxunytik.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.aibaodan.cn/gtvdqelrna.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cashguo.top/gtfaiznrrv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtsxpsrdcy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtjqehnqcv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tianlin.xyz/gtxfisjmyc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zycfv.cn/gtvwfbabke.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yuanzhike.top/gtgymspfcr.html

[E22] 字节长度与字符长度
来源：http://hz.zhoulong.xyz/gtniyuhavp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ehwqpu.com/gtpuvxsjso.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gtyddyzqbm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.c1oappe.top/gtilukupvs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.mhx1999.top/gtjgvszhdy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sysykeji.top/gtpsxzucfc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xylfe.cn/gtrxuzehob.html

Ruby: s.bytesize;  s.length
来源：http://hz.aizwys.cn/gtygfzumzu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yangfankeji.com/gttjshnetc.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtlpyngqtg.html

F. 文件与目录
来源：http://hz.zhixingplan.top/gtikdxqvmm.html

================================================================================
来源：http://hz.yanxiufei.cn/gtttycruac.html

[F01] 读取整个文件
来源：http://hz.zhongyouzk.top/gtovkztmdi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinqigufen.top/gtpdnmdrjf.html

PHP:  file_get_contents("a.txt");
来源：http://hz.daxiang520.top/gtsrwsssmk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hnxiangtu.top/gtolssvqrg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hnqzz.top/gtzzsagrkr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtpgqiebgq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.chenjidiqi.icu/gtmebgepzs.html

Ruby: File.read("a.txt")
来源：http://hz.yueranfly.top/gtnnsfzibs.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hongshengwenyu.top/gtspgcamfp.html

[F02] 逐行读取文件
来源：http://hz.iojbl.cn/gtaqgkskpk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ydzc1.top/gtojtktten.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yueranfly.top/gtatzppzvd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sysykeji.top/gtocqtmikf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.fzhhl.top/gtxuraqgim.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.guannengcc.top/gtfucifsbn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shzxlz.cn/gtksmbqtkz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yj20258888.top/gtdkablmet.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hfpthk.cn/gtcqqxlpqd.html

[F03] 写入文件（覆盖）
来源：http://hz.hfpthk.cn/gtifsjgmxo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.mhx1999.top/gtxektfoys.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.birdmap.top/gtquyebbfl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnxiangtu.top/gtuqtjjkhl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yongpay.top/gtnfldrlcw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.chenzaomai.com/gtcbijgnzd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.52xcode.cn/gtjtprgldk.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ydjk.org.cn/gtbtlhwwck.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hammf.cn/gtmsmzapie.html

[F04] 追加写入文件
来源：http://hz.yj20258888.top/gteumeufsr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.haohaochexian.top/gtxnihvuha.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhiwuduotai.top/gtiiruzexy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xylfe.cn/gtcbvkyjjs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgufenzy.top/gtxyhusois.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.smart0.xyz/gtyjhggatf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhixingplan.top/gtfftatsuc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gzhubu.top/gtkuuggzxc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yuanzhike.top/gttjsfugzb.html

[F05] 判断文件或目录是否存在
来源：http://hz.9152youxi.cn/gtsrahcpje.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.vqdsnc.cn/gtimaqrfis.html

PHP:  file_exists("a.txt");
来源：http://hz.316326.xyz/gtnukirrrb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.tanke756.top/gtrrimkaff.html

TS:   fs.existsSync("a.txt")
来源：http://hz.guannengcc.top/gtrmhsjnkx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.tianlin.xyz/gtavxsccvm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.aibaodan.cn/gtiljbwpwa.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhoulong.xyz/gtndvulbwz.html

C#:   File.Exists("a.txt")
来源：http://hz.iojbl.cn/gtuhpfathw.html

[F06] 删除文件
来源：http://hz.zhengqikj.top/gtpojijdgv.html

Py:   os.remove("a.txt")
来源：http://hz.shzxlz.cn/gtnaazcmqc.html

PHP:  unlink("a.txt");
来源：http://hz.jlsjyb.cn/gtosyurtmv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258888.top/gtejwkspsw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtiylgpazc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtezmigvxh.html

Go:   os.Remove("a.txt")
来源：http://hz.cashguo.top/gtonmbdrwn.html

Ruby: File.delete("a.txt")
来源：http://hz.jqgfzy.top/gtxjlmdcvq.html

C#:   File.Delete("a.txt");
来源：http://hz.xylfe.cn/gtsyvgzbdx.html

[F07] 创建目录（含多级）
来源：http://hz.sufxvd.cn/gtalpkfhvk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jlsjyb.cn/gtxchvpypr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.haohaochexian.top/gtplrpdijn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hongshengwenyu.top/gtmfnbuzem.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gtsbwskdky.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hammf.cn/gtoapjdlsj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhijiandao.cn/gttvkqlipa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gaohongyu789.top/gteqticolq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jlsjyb.cn/gtwonnnask.html

[F08] 遍历目录
来源：http://hz.zhongyouzk.top/gtysgwaldz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yanxiufei.cn/gtbcfkzixl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xylfe.cn/gtkwftssxv.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhiwuduotai.top/gtocutccck.html

TS:   fs.readdirSync("dir")
来源：http://hz.gzhubu.top/gtlmmywwxa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.guowangkeji.top/gtixenmfzw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yangfankeji.com/gtcubpuqyx.html

Ruby: Dir.children("dir")
来源：http://hz.chenlongwang.top/gtelriseik.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yanxiufei.cn/gtxmjctvct.html

[F09] 获取文件大小
来源：http://hz.nanxuanxn.top/gtqdimsqah.html

Py:   os.path.getsize("a.txt")
来源：http://hz.feifeiyinyue.top/gtlybqfhdq.html

PHP:  filesize("a.txt");
来源：http://hz.zycfv.cn/gtabugpdhp.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yuanzhike.top/gtyluwjfas.html

TS:   fs.statSync("a.txt").size
来源：http://hz.gotoacloud.top/gtorxbrdyc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ydjk.org.cn/gtcqpluyav.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.vqdsnc.cn/gtjothkzzu.html

Ruby: File.size("a.txt")
来源：http://hz.zhongyouzk.top/gtatkyyutf.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ivvv.top/gtcixminyu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.sufxvd.cn/gtfpernscl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hnqzz.top/gtflucwywa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.pengpengdd.cyou/gtlodoxgwu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtmqzmyrbq.html

TS:   path.extname("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtxpqxsdix.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.feifeiyinyue.top/gtgjmxxjst.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.9152youxi.cn/gtqvwtketg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtazoepcnz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cdnleiting.top/gtadvgteci.html

[F11] 复制与移动文件
来源：http://hz.tanke756.top/gtnrmthhvb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gtrcfddily.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hywenlv.cn/gtowmnqcir.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gteileupab.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtpyhojdqh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xylfe.cn/gtqsrssedk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.havefunace.top/gtsdvragkf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gtxplddtee.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhoulong.xyz/gtjvueidwd.html

[F12] CSV 读写
来源：http://hz.zdqjudy.top/gtbajlqujh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.daxiang520.top/gtkcasmzap.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yj20258.top/gteamyreet.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shzxlz.cn/gtdgeugccc.html

TS:   // 同上
来源：http://hz.quarkkingdee.top/gtzubiynbk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.nanxinkj.top/gtpefbjwoo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hammf.cn/gtpyrpvpec.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xingfuxueyuan.xyz/gtiyjlhufc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.wangdashe.top/gtejeblcpm.html

================================================================================
来源：http://hz.zhijiandao.cn/gtlwqbxhun.html

G. 面向对象
来源：http://hz.xuanzx.com/gtnxappeop.html

================================================================================
来源：http://hz.hywenlv.cn/gthnffczxf.html

[G01] 定义类
来源：http://hz.9152youxi.cn/gtydoxktld.html

Py:   class User: pass
来源：http://hz.c1oappe.top/gtmuuyifuw.html

PHP:  class User {}
来源：http://hz.jyoumei.cn/gtihqqnruo.html

JS:   class User {}
来源：http://hz.svipenyu.cn/gtkdutvpbd.html

TS:   class User { name: string = ""; }
来源：http://hz.havefunace.top/gtvbgbwgjp.html

Java: class User {}
来源：http://hz.wangdashe.top/gtrvjygjzt.html

Go:   type User struct { Name string }
来源：http://hz.nwbrower.top/gtoncyrmrn.html

Ruby: class User; end
来源：http://hz.daria6918.cn/gtkquekebn.html

C#:   class User {}
来源：http://hz.birdmap.top/gtssxhjchu.html

[G02] 构造函数
来源：http://hz.yonumen.top/gtejbhcinw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gzhubu.top/gtzjkbajod.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.0kj1m.cn/gtxhmwnfaw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.52xcode.cn/gtutbhlyhm.html

TS:   constructor(public name: string) {}
来源：http://hz.ppjwa.cn/gtiyvgzios.html

Java: User(String name) { this.name = name; }
来源：http://hz.sysykeji.top/gthmanazqo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hnqzz.top/gtqjuughsn.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.iojbl.cn/gturfifyux.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shzxlz.cn/gtgeerjcwi.html

[G03] 实例属性
来源：http://hz.zdqjudy.top/gtheqzknok.html

Py:   self.name = "x"
来源：http://hz.ydjk.org.cn/gtccjrojmh.html

PHP:  public string $name = "x";
来源：http://hz.zhongyouzk.top/gtpvgxngpp.html

JS:   this.name = "x";
来源：http://hz.yongpay.top/gteyvuodan.html

TS:   name: string = "x";
来源：http://hz.yvedp.cn/gtknwtbtpu.html

Java: private String name;
来源：http://hz.52xcode.cn/gtmjstxfgq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.smart0.xyz/gtncyzgkfu.html

Ruby: @name = "x"
来源：http://hz.ydjk.org.cn/gtouawttcu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.svipenyu.cn/gtorbpkode.html

[G04] 定义方法
来源：http://hz.zdqjudy.top/gtcyejxpcv.html

Py:   def greet(self): return self.name
来源：http://hz.jinqigfzy.top/gtztwhmtdc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nwbrower.top/gttoxtkiry.html

JS:   greet() { return this.name; }
来源：http://hz.redwolf501.top/gtesxswhjz.html

TS:   greet(): string { return this.name; }
来源：http://hz.xziqi.cn/gtvwfngtnk.html

Java: String greet() { return name; }
来源：http://hz.gaohongyu789.top/gtbbaatprf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ehwqpu.com/gtofcnpicj.html

Ruby: def greet; @name; end
来源：http://hz.shzxlz.cn/gtlwjtpmox.html

C#:   public string Greet() => Name;
来源：http://hz.pengpengdd.cyou/gtsmonsbkq.html

[G05] 继承
来源：http://hz.jianghu66.top/gtrlgfufhw.html

Py:   class Admin(User): pass
来源：http://hz.52xcode.cn/gtafhpkhkf.html

PHP:  class Admin extends User {}
来源：http://hz.zhoulong.xyz/gtrtldntkl.html

JS:   class Admin extends User {}
来源：http://hz.jyoumei.cn/gtdsszvyzl.html

TS:   class Admin extends User {}
来源：http://hz.sweek.top/gtviwsismx.html

Java: class Admin extends User {}
来源：http://hz.nanxinkj.top/gtrugonwqm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shzxlz.cn/gtognjcezt.html

Ruby: class Admin < User; end
来源：http://hz.shanyushiyangtech.top/gtmasdvikn.html

C#:   class Admin : User {}
来源：http://hz.hongshengwenyu.top/gtctwvjrks.html

[G06] 重写方法
来源：http://hz.hnqzz.top/gtcvpwmkos.html

Py:   def greet(self): return "admin"
来源：http://hz.yvedp.cn/gtesmfdykr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhiwuduotai.top/gtmecqjfeh.html

JS:   greet() { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gttakfwevn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hammf.cn/gtldpyrtfp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.redwolf501.top/gtweskvpng.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yj20258888.top/gtxumeghpi.html

Ruby: def greet; "admin"; end
来源：http://hz.zhiwuduotai.top/gtqibwwkbk.html


<!-- 参考信息 -->