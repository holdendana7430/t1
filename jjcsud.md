代发 wailian999

PHP:  implode(",", $items);
来源：http://hz.nanxinkj.top/gtfanmxfzl.html

JS:   items.join(",")
来源：http://hz.sysykeji.top/gtpoqkgfju.html

TS:   items.join(",")
来源：http://hz.tanke756.top/gtkglqikct.html

Java: String.join(",", items)
来源：http://hz.aizwys.cn/gtvsmeselh.html

Go:   strings.Join(items, ",")
来源：http://hz.fzhhl.top/gtjdhwokyd.html

Ruby: items.join(",")
来源：http://hz.guannengcc.top/gtxbfanjzi.html

C#:   string.Join(",", items)
来源：http://hz.xuanzx.com/gtaomhifeq.html

[E09] 去除所有空白字符
来源：http://hz.havefunace.top/gtrhhwhwxr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.chenlongwang.top/gthndzcviy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhoulong.xyz/gtgibacxbc.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.aizwys.cn/gthvyodhpj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.wangshuangyany.cn/gtryqfkbwa.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hysaishi.cn/gtztvcvicx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shangyingyoupin.top/gtdpotrymy.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.bjfxy.top/gtzrdxlgat.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.0kj1m.cn/gtyptyqpjn.html

[E10] 左侧补零 / 定长填充
来源：http://hz.snrcjt.cn/gtrwxxiuco.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xylfe.cn/gttkfinwew.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hywenlv.cn/gtsqfnffuu.html

JS:   "7".padStart(3, "0")
来源：http://hz.cashguo.top/gtscusyqvm.html

TS:   "7".padStart(3, "0")
来源：http://hz.shanyushiyangkeji.top/gtlohplfsb.html

Java: String.format("%03d", 7)
来源：http://hz.zhixingplan.top/gtajvxknjx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhongyouzk.top/gtyytwjwkm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.0kj1m.cn/gtrvqceouq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.ehwqpu.com/gtupquxdnx.html

[E11] 反转字符串
来源：http://hz.zhixingplan.top/gtacxkndjt.html

Py:   s[::-1]
来源：http://hz.sufxvd.cn/gtouadjbfd.html

PHP:  strrev($s);
来源：http://hz.nanxuanxn.top/gtlncuycvt.html

JS:   [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtanlwrkzp.html

TS:   [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtbyrrzhkk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinqigfzy.top/gtjdpkpjja.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.aibaodan.cn/gtebvjcqlf.html

Ruby: s.reverse
来源：http://hz.yuxming.cn/gtbwuicuwb.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xylfe.cn/gtkalihuhk.html

[E12] 统计某字符出现次数
来源：http://hz.shanyushiyangtech.top/gttzlpbmks.html

Py:   s.count("a")
来源：http://hz.birdmap.top/gtcsthxjco.html

PHP:  substr_count($s, "a");
来源：http://hz.jinyuanbaomall.cn/gtrzmhyciw.html

JS:   s.split("a").length - 1
来源：http://hz.zdqjudy.top/gtnlbnbaha.html

TS:   s.split("a").length - 1
来源：http://hz.hongshengwenyu.top/gteagwmhvh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xylfe.cn/gtjixdnhpp.html

Go:   strings.Count(s, "a")
来源：http://hz.gzhubu.top/gtqqomcbcc.html

Ruby: s.count("a")
来源：http://hz.yj20258888.top/gtlgbmqyfo.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zycfv.cn/gtaavjnaab.html

[E13] 逐字符遍历
来源：http://hz.zhengqikj.top/gtuqxhjxfv.html

Py:   for ch in s: print(ch)
来源：http://hz.zhengqikj.top/gtxpwfowhl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhaomingkeji.xyz/gtfaqwtdtp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuxming.cn/gtrvjatizu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.iojbl.cn/gttfeelfvf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shanyushiyangtech.top/gtohrfucba.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shzxlz.cn/gtyhzmgzal.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.daria6918.cn/gtcwmvrzpq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jqgufenzy.top/gtwhhjaraq.html

[E14] URL 编码与 Base64
来源：http://hz.ehwqpu.com/gtgzrfktjo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.cashguo.top/gtxbwdciqo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cucudq.cn/gtdqybcetx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jqgufenzy.top/gtbzketydx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.svipenyu.cn/gtvkupkung.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hnqzz.top/gtptcgqbov.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cqqwz.cn/gtqmhxrmik.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xingfuxueyuan.xyz/gttfoheqna.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.meibo888.top/gtyzlrvvxv.html

[E15] HTML 转义 / 反转义
来源：http://hz.shangyingyoupin.top/gtemmhxuas.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ywan-chungtsiang.top/gtrfmlcgyn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.havefunace.top/gtpjhugvrc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.sufxvd.cn/gtjnxxayta.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cucudq.cn/gtuxmwmgol.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinqigufen.top/gthquwoebs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.quarkkingdee.top/gthfmknumy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.andypj.xyz/gtuijrechy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jiagoushi.top/gtuyturjtu.html

[E16] 数字千分位
来源：http://hz.cashguo.top/gtgnxdymxq.html

Py:   f"{1234567:,}"
来源：http://hz.fengsongda.top/gtirqkmltc.html

PHP:  number_format(1234567);
来源：http://hz.dianchejie.cn/gtcwygkidq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hongshengwenyu.top/gtzeiaihzd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yongpay.top/gtzriciwzo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xingfuxueyuan.xyz/gtyxglzbug.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hnxiangtu.top/gtgcraietm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ydjk.org.cn/gtlhvqsqsh.html

C#:   1234567.ToString("N0")
来源：http://hz.daxiang520.top/gtwnfkeuub.html

[E17] 首字母大写
来源：http://hz.sxryk.cn/gtswcvksgs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.guowangkeji.top/gttgffqobn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cucudq.cn/gtuszvdomt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangtech.top/gttvtskjxo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hammf.cn/gtkbpmzvvg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yongpay.top/gtmdkxlcsd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.snrcjt.cn/gtfqyyuznb.html

Ruby: s.capitalize
来源：http://hz.pengpengdd.cyou/gtselyqpqw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ppjwa.cn/gtkguwkhbq.html

[E18] 模板占位符替换
来源：http://hz.xziqi.cn/gtucqdfumu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.iojbl.cn/gtjjgrbjar.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.sufxvd.cn/gtomzcyjpn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hammf.cn/gtuavlwwcs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ppjwa.cn/gtzheabvjn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shanyushiyangtech.top/gtqltkwevm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinqigfzy.top/gtucxxntwq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.daxiang520.top/gtqbblslya.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.redwolf501.top/gtshrrretj.html

[E19] 多行文本按行拆分
来源：http://hz.ydjk.org.cn/gtjapohjbt.html

Py:   s.splitlines()
来源：http://hz.tanke756.top/gthyqulima.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cashguo.top/gtrhxkwefp.html

JS:   s.split(/\r?\n/)
来源：http://hz.cashguo.top/gtlnxpbnrd.html

TS:   s.split(/\r?\n/)
来源：http://hz.chenzaomai.com/gtjznqeivf.html

Java: s.lines().toList()
来源：http://hz.zdqjudy.top/gttehgggab.html

Go:   strings.Split(s, "\n")
来源：http://hz.cashguo.top/gtxcrfehte.html

Ruby: s.lines
来源：http://hz.bjfxy.top/gtiedxzroy.html

C#:   s.Split('\n')
来源：http://hz.iojbl.cn/gtlkutowin.html

[E20] 判断字符串是否为空
来源：http://hz.iojbl.cn/gtmoanixmu.html

Py:   if not s:
来源：http://hz.tian-w.cn/gtnixutkib.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.guowangkeji.top/gtuwiwygbl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.quarkkingdee.top/gtvibbffyl.html

TS:   if (s === "") {}
来源：http://hz.daxiang520.top/gtqfgjvvmc.html

Java: if (s.isEmpty()) {}
来源：http://hz.bjfxy.top/gttljiovdl.html

Go:   if s == "" {}
来源：http://hz.0kj1m.cn/gtaxejiuag.html

Ruby: if s.empty?
来源：http://hz.gotoacloud.top/gtiguwfszi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jinghuilouyu.cn/gtfjijjnkl.html

[E21] 超长截断加省略号
来源：http://hz.shzxlz.cn/gtwyszabhz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.nanxuanxn.top/gtlckmclwh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.c1oappe.top/gtekntexas.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.52xcode.cn/gtktkpfzag.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pycfn.com/gtvkhevmfj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hnqzz.top/gttrfhgqlo.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.nwbrower.top/gtdwkycmmx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenjidiqi.icu/gtyooxdnzf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.havefunace.top/gtrkzetdkl.html

[E22] 字节长度与字符长度
来源：http://hz.haohaochexian.top/gtegdugwjd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hfpthk.cn/gtyvlkgjvo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gotoacloud.top/gtfqhwzcnf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zycfv.cn/gtrnolmnrl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.0kj1m.cn/gtitbwdnfu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.snrcjt.cn/gtjgykcuqu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cdnleiting.top/gtuavkhkcf.html

Ruby: s.bytesize;  s.length
来源：http://hz.fengsongda.top/gtrfgjsqta.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.mhx1999.top/gtcybrynuh.html

================================================================================
来源：http://hz.andypj.xyz/gtedsatjmr.html

F. 文件与目录
来源：http://hz.snrcjt.cn/gtyatarimx.html

================================================================================
来源：http://hz.zhongyouzk.top/gtiwznfsrh.html

[F01] 读取整个文件
来源：http://hz.xuetiantiany.cn/gtmrxzwvli.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.c1oappe.top/gtfucglwod.html

PHP:  file_get_contents("a.txt");
来源：http://hz.daxiang520.top/gtelwgrcqy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.aibaodan.cn/gtcqrexnuo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yuanzhike.top/gtiofswrvp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.gaohongyu789.top/gtlfnppjvl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xinyue.icu/gtugoiuuxy.html

Ruby: File.read("a.txt")
来源：http://hz.sysykeji.top/gtvcsidfub.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ivvv.top/gtboolvjsy.html

[F02] 逐行读取文件
来源：http://hz.jinqigufen.top/gtbmquhomr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jqgfzy.top/gtsmqmurhq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhixingplan.top/gtemystzed.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.fzhhl.top/gtroroquox.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgfzy.top/gtvhlmwbet.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhijiandao.cn/gtbitgbyci.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gotoacloud.top/gtfzqmgujq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shuidangran.top/gtkqcfunkl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yueranfly.top/gtbppmohus.html

[F03] 写入文件（覆盖）
来源：http://hz.jiagoushi.top/gtagzpwpgp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yj20258.top/gtndpmoctm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xuanzx.com/gthhfkjqmt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhijiandao.cn/gtcmglxdae.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xuanzx.com/gtuwkasnal.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhiwuduotai.top/gtkedpmbfz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.tian-w.cn/gtcdkjlmjg.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.birdmap.top/gtzmyyxenj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yj202588.top/gtqtxvmawa.html

[F04] 追加写入文件
来源：http://hz.yanxiufei.cn/gtebfhdjjg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ydjk.org.cn/gttzhyjphi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cucudq.cn/gtiuhopsue.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhongyouzk.top/gtexhwpqll.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgfzy.top/gtcpmmghaj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.daxiang520.top/gtkdelqlfz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.9152youxi.cn/gtzteqpclz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yuanzhike.top/gtpmtbcxeu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gogol.net.cn/gtqcmsqehm.html

[F05] 判断文件或目录是否存在
来源：http://hz.xingfuxueyuan.xyz/gtqujejzuz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jinghuilouyu.cn/gthnhoytov.html

PHP:  file_exists("a.txt");
来源：http://hz.shzxlz.cn/gtdirpnnhc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinqigfzy.top/gtaavzrjjk.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtbevbvuhc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtpxlfnksc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ivvv.top/gtuwawuwbq.html

Ruby: File.exist?("a.txt")
来源：http://hz.haohaochexian.top/gtlrjvofhg.html

C#:   File.Exists("a.txt")
来源：http://hz.xinyue.icu/gtqczibjxd.html

[F06] 删除文件
来源：http://hz.52xcode.cn/gtqedemuuv.html

Py:   os.remove("a.txt")
来源：http://hz.nwbrower.top/gtlzozgphf.html

PHP:  unlink("a.txt");
来源：http://hz.ppjwa.cn/gtuasyoysj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.wangdashe.top/gtlhzjzmul.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxinkj.top/gtkboqwzmu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gaohongyu789.top/gtcldtguoj.html

Go:   os.Remove("a.txt")
来源：http://hz.zhoulong.xyz/gtgzpnvxwc.html

Ruby: File.delete("a.txt")
来源：http://hz.0kj1m.cn/gtkylsyqvb.html

C#:   File.Delete("a.txt");
来源：http://hz.hfpthk.cn/gtghiexrhm.html

[F07] 创建目录（含多级）
来源：http://hz.jinghuilouyu.cn/gtxgtnemkc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.pengpengdd.cyou/gtawvrpksz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.iojbl.cn/gtkdakypns.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sweek.top/gtjnrsxfnp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sufxvd.cn/gtcbroethp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jqgfzy.top/gtccupdpuj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gotoacloud.top/gtnanldhdy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.dashuyun.cn/gtkypakuxr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.snrcjt.cn/gtqznvybht.html

[F08] 遍历目录
来源：http://hz.hongshengwenyu.top/gtkjihmner.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gotoacloud.top/gttccnrdwm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.svipenyu.cn/gtqjmuqbvc.html

JS:   fs.readdirSync("dir")
来源：http://hz.hywenlv.cn/gtcydqgbmh.html

TS:   fs.readdirSync("dir")
来源：http://hz.jianghu66.top/gtvwqrhxkf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.sufxvd.cn/gtysjnklkd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.sysykeji.top/gtrbkzohgc.html

Ruby: Dir.children("dir")
来源：http://hz.jqgufenzy.top/gtthdjzqfk.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhengqikj.top/gtgrrqtgmi.html

[F09] 获取文件大小
来源：http://hz.bjfxy.top/gthxoglolt.html

Py:   os.path.getsize("a.txt")
来源：http://hz.c1oappe.top/gtbikuahcq.html

PHP:  filesize("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtuwpwzhzp.html

JS:   fs.statSync("a.txt").size
来源：http://hz.dashuyun.cn/gtlrzuphox.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinqigfzy.top/gtrumnezvy.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sweek.top/gtmwiazgfq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hammf.cn/gtisaxnvof.html

Ruby: File.size("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtsoebmhzw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ybcxt.top/gtkmfhuzuu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.dashuyun.cn/gtgefkebfz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtmoijksjl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sufxvd.cn/gttuacejil.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.chenzaomai.com/gtbyoexrpd.html

TS:   path.extname("a.txt")
来源：http://hz.jyoumei.cn/gtsfjyylra.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.wangdashe.top/gtsgykyhja.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.smart0.xyz/gtnlhmmrgv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.smart0.xyz/gtgthtsfkb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtfkvdxrbj.html

[F11] 复制与移动文件
来源：http://hz.dianchejie.cn/gtrfcjuwys.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhoulong.xyz/gtlethcbve.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.tian-w.cn/gtnnhlipyp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gtgogdntjt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gthzfynigh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yanxiufei.cn/gtxfwlekis.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cqqwz.cn/gtuubyeuah.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gtmcvogerh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hywenlv.cn/gtskbyakeo.html

[F12] CSV 读写
来源：http://hz.cqqwz.cn/gtdyinnojw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jqgufenzy.top/gtxzglzxbo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.tianlin.xyz/gtzfjxvnyy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.aibaodan.cn/gtcuiqyidr.html

TS:   // 同上
来源：http://hz.pengpengdd.cyou/gtdwpybjmf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinqigfzy.top/gteeculerp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhiwuduotai.top/gtorketfdf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinqigfzy.top/gtjqjkdrub.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yonumen.top/gtdryhudvn.html

================================================================================
来源：http://hz.meibo888.top/gtajkhjfsq.html

G. 面向对象
来源：http://hz.jqgfzy.top/gtutmzetxt.html

================================================================================
来源：http://hz.andypj.xyz/gtyolsdecm.html

[G01] 定义类
来源：http://hz.chenlongwang.top/gtpcfcltht.html

Py:   class User: pass
来源：http://hz.shanyushiyangtech.top/gtmothxovo.html

PHP:  class User {}
来源：http://hz.shuidangran.top/gtjxnpkgag.html

JS:   class User {}
来源：http://hz.jianghu66.top/gtjwndmwki.html

TS:   class User { name: string = ""; }
来源：http://hz.xziqi.cn/gtiazwaylw.html

Java: class User {}
来源：http://hz.guowangkeji.top/gtcpolhnbj.html

Go:   type User struct { Name string }
来源：http://hz.shuidangran.top/gtgvsxvsor.html

Ruby: class User; end
来源：http://hz.zhoulong.xyz/gtoecdoues.html

C#:   class User {}
来源：http://hz.tian-w.cn/gtkeeedzxm.html

[G02] 构造函数
来源：http://hz.ybcxt.top/gtnbdbfken.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hongshengwenyu.top/gtjkxkzhaw.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zdqjudy.top/gtvcovutuu.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tianlin.xyz/gtbahrtdmy.html

TS:   constructor(public name: string) {}
来源：http://hz.zhoulong.xyz/gtzzfgaagx.html

Java: User(String name) { this.name = name; }
来源：http://hz.gotoacloud.top/gtiasabtzn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.tian-w.cn/gttkelzfcj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.fengsongda.top/gtdercqfik.html

C#:   public User(string name) { Name = name; }
来源：http://hz.pengpengdd.cyou/gtbucnaqla.html

[G03] 实例属性
来源：http://hz.ppjwa.cn/gtvqgdxoxp.html

Py:   self.name = "x"
来源：http://hz.ywan-chungtsiang.top/gtpxcdjdan.html

PHP:  public string $name = "x";
来源：http://hz.meibo888.top/gtzjcamsgn.html

JS:   this.name = "x";
来源：http://hz.mhx1999.top/gtfrxgrlhi.html

TS:   name: string = "x";
来源：http://hz.daxiang520.top/gtxkupuogr.html

Java: private String name;
来源：http://hz.yj20258.top/gtqamchtls.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shanyushiyangkeji.top/gtpxlwxkkn.html

Ruby: @name = "x"
来源：http://hz.birdmap.top/gtfpavwaix.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yj20258.top/gttzdjluyf.html

[G04] 定义方法
来源：http://hz.hnqzz.top/gthrxhzcbh.html

Py:   def greet(self): return self.name
来源：http://hz.yj20258.top/gtmbayhlfh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.guowangkeji.top/gtvebggtea.html

JS:   greet() { return this.name; }
来源：http://hz.cqqwz.cn/gttnqgvxsg.html

TS:   greet(): string { return this.name; }
来源：http://hz.0kj1m.cn/gtvwgonpwb.html

Java: String greet() { return name; }
来源：http://hz.nanxuanxn.top/gtciejmkhc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinyuanbaomall.cn/gttomltrgt.html

Ruby: def greet; @name; end
来源：http://hz.jinqigufen.top/gtlmgwciap.html

C#:   public string Greet() => Name;
来源：http://hz.xingfuxueyuan.xyz/gtlgkintch.html

[G05] 继承
来源：http://hz.zhoulong.xyz/gtqpqszkhe.html

Py:   class Admin(User): pass
来源：http://hz.ydjk.org.cn/gtqappzuuj.html

PHP:  class Admin extends User {}
来源：http://hz.dashuyun.cn/gtwqpwcoof.html

JS:   class Admin extends User {}
来源：http://hz.hysaishi.cn/gtimufafpk.html

TS:   class Admin extends User {}
来源：http://hz.gzhubu.top/gtzutqfzzi.html

Java: class Admin extends User {}
来源：http://hz.aizwys.cn/gthfhbcteq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhijiandao.cn/gtswvlxhkp.html

Ruby: class Admin < User; end
来源：http://hz.feifeiyinyue.top/gtqmtsiikj.html

C#:   class Admin : User {}
来源：http://hz.jinghuilouyu.cn/gtdrqouocg.html

[G06] 重写方法
来源：http://hz.ywan-chungtsiang.top/gtaszjzglw.html

Py:   def greet(self): return "admin"
来源：http://hz.jinqigufen.top/gtkgmgdokc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hysaishi.cn/gtecjgvqrp.html

JS:   greet() { return "admin"; }
来源：http://hz.guowangkeji.top/gtsmnhisze.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jqgfzy.top/gtzuyjlboj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtprbssada.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.9152youxi.cn/gtbxapqdgy.html

Ruby: def greet; "admin"; end
来源：http://hz.bjfxy.top/gtfozazgdm.html


<!-- 参考信息 -->