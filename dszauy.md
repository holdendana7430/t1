代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.daxiang520.top/gtcryeybzm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shanyushiyangtech.top/gtmrcdxahk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sxryk.cn/gtmgkyxozf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhiwuduotai.top/gtbismyxet.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nanxuanxn.top/gtwxakazlf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yuxming.cn/gtnmwdukzi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.nanxinkj.top/gtkfihbnjs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yonumen.top/gtnaoppslr.html

[E06] 替换子串
来源：http://hz.tianlin.xyz/gtgnhdgurj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.0kj1m.cn/gtbrpxbmji.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.cashguo.top/gtkebctorr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.tianlin.xyz/gtirrglwor.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hongshengwenyu.top/gtkrvcbrmw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xuanzx.com/gtidbpnkuf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yangfankeji.com/gtenqfazwd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xinyue.icu/gtpfyxvqag.html

C#:   s.Replace("a", "b")
来源：http://hz.birdmap.top/gtpvvcekfj.html

[E07] 按分隔符拆分
来源：http://hz.aizwys.cn/gttkoodcup.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.haohaochexian.top/gtnmzuviey.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ppjwa.cn/gtkkvqqiri.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sweek.top/gtwcbumxfg.html

TS:   s.split(",")
来源：http://hz.yj20258888.top/gtouthhqrb.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shangyingyoupin.top/gtecaeftpl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.0kj1m.cn/gtfgphvlur.html

Ruby: s.split(",");  s.split
来源：http://hz.shangyingyoupin.top/gtrkgqqwqw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yongpay.top/gtyynnwunj.html

[E08] 数组按分隔符合并
来源：http://hz.nanxinkj.top/gtvzdgxrib.html

Py:   ",".join(items)
来源：http://hz.xylfe.cn/gtlrogtvqk.html

PHP:  implode(",", $items);
来源：http://hz.zdqjudy.top/gtrzaaafwy.html

JS:   items.join(",")
来源：http://hz.aizwys.cn/gtgumduerd.html

TS:   items.join(",")
来源：http://hz.pycfn.com/gttohqbsfg.html

Java: String.join(",", items)
来源：http://hz.sweek.top/gtjvbuncay.html

Go:   strings.Join(items, ",")
来源：http://hz.xuetiantiany.cn/gtwhptlobo.html

Ruby: items.join(",")
来源：http://hz.quarkkingdee.top/gtcksorjhm.html

C#:   string.Join(",", items)
来源：http://hz.yj20258.top/gtbcqackpn.html

[E09] 去除所有空白字符
来源：http://hz.wangdashe.top/gtakogitbw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.wangshuangyany.cn/gtvrygdcnp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.wangdashe.top/gtfqefdyvn.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.havefunace.top/gtmajjbcxb.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ppjwa.cn/gtrfobkdau.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.daxiang520.top/gtljvjowuw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhaomingkeji.xyz/gtieegvpdt.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.fengsongda.top/gtikxpzkqx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cucudq.cn/gtvvabcjws.html

[E10] 左侧补零 / 定长填充
来源：http://hz.shangyingyoupin.top/gtvnlyhgkg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ppjwa.cn/gtadxzyqpr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.quarkkingdee.top/gtezpxwpbw.html

JS:   "7".padStart(3, "0")
来源：http://hz.sweek.top/gtfrctfgxc.html

TS:   "7".padStart(3, "0")
来源：http://hz.shzxlz.cn/gtwjhxyhva.html

Java: String.format("%03d", 7)
来源：http://hz.jqgufenzy.top/gtkipofxyh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhengqikj.top/gtfynbffvo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.svipenyu.cn/gtrcbamonn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shzxlz.cn/gtqmfqzhwz.html

[E11] 反转字符串
来源：http://hz.ydjk.org.cn/gtzpxcqxgz.html

Py:   s[::-1]
来源：http://hz.zdqjudy.top/gtjrrmbbkq.html

PHP:  strrev($s);
来源：http://hz.ppjwa.cn/gthnffsfqx.html

JS:   [...s].reverse().join("")
来源：http://hz.cheryme.top/gtxvbbheyo.html

TS:   [...s].reverse().join("")
来源：http://hz.cheryme.top/gtlhjuoxqi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.cashguo.top/gtvtwyxjjp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.cqqwz.cn/gtitolylsw.html

Ruby: s.reverse
来源：http://hz.cheryme.top/gtccjlxric.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.316326.xyz/gtnuzlebmi.html

[E12] 统计某字符出现次数
来源：http://hz.gogol.net.cn/gtndrwihha.html

Py:   s.count("a")
来源：http://hz.jiagoushi.top/gtkmeemydr.html

PHP:  substr_count($s, "a");
来源：http://hz.gogol.net.cn/gtdfugzcbm.html

JS:   s.split("a").length - 1
来源：http://hz.316326.xyz/gttatkyxfu.html

TS:   s.split("a").length - 1
来源：http://hz.gzhubu.top/gtfkhpfvsg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yanxiufei.cn/gtvbakpgtm.html

Go:   strings.Count(s, "a")
来源：http://hz.sweek.top/gtocqcfmwe.html

Ruby: s.count("a")
来源：http://hz.cashguo.top/gtapctgkkf.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sufxvd.cn/gtzctdywgx.html

[E13] 逐字符遍历
来源：http://hz.jqgufenzy.top/gtuywkfqds.html

Py:   for ch in s: print(ch)
来源：http://hz.jinqigfzy.top/gteiglirrb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.guowangkeji.top/gtthpimqll.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aibaodan.cn/gtwdywazmp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.smart0.xyz/gtztdetaeg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.bjfxy.top/gtlpjmuudf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.daxiang520.top/gtjinryoee.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.tian-w.cn/gtrsgappwj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.cashguo.top/gtgfgzgjig.html

[E14] URL 编码与 Base64
来源：http://hz.yuxming.cn/gtmioyauri.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhengqikj.top/gtjeszfxbz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sysykeji.top/gtelspgzqx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yongpay.top/gtxldlunmx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.quarkkingdee.top/gtettleacm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.pycfn.com/gtlvhfpsyi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.daxiang520.top/gtzphkuirp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhaomingkeji.xyz/gtuathogvt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cdnleiting.top/gtxihtgxkg.html

[E15] HTML 转义 / 反转义
来源：http://hz.xuetiantiany.cn/gtuotfpcuu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xinyue.icu/gtrvauctds.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.gzhubu.top/gtcboeygve.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.dianchejie.cn/gtvgmbnwrq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.9152youxi.cn/gtvlntchbs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yvedp.cn/gtpgnwppcq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhixingplan.top/gtzblfsvdx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yanxiufei.cn/gtfixpmamd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.0kj1m.cn/gtjfgnvmuw.html

[E16] 数字千分位
来源：http://hz.aibaodan.cn/gtprawmndu.html

Py:   f"{1234567:,}"
来源：http://hz.aizwys.cn/gtuitpozba.html

PHP:  number_format(1234567);
来源：http://hz.tianlin.xyz/gtbwjsvkcy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yongpay.top/gtdtxizcpe.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.daria6918.cn/gtudacbbcy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinqigufen.top/gtynbgcucr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.shangyingyoupin.top/gtfzavdquh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.bjfxy.top/gtjjpsrlrv.html

C#:   1234567.ToString("N0")
来源：http://hz.hongshengwenyu.top/gtkkfkqnoq.html

[E17] 首字母大写
来源：http://hz.cashguo.top/gtfjqrikwb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jiagoushi.top/gtdtqcerfy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yj20258.top/gtorzhpwsg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yonumen.top/gtmuoczaog.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.pycfn.com/gtisaofuoj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shzxlz.cn/gtyovunpvt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.chenlongwang.top/gtcitkfuin.html

Ruby: s.capitalize
来源：http://hz.ywan-chungtsiang.top/gtqiwremms.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ppjwa.cn/gtrtvwgesg.html

[E18] 模板占位符替换
来源：http://hz.jinyuanbaomall.cn/gtboxrbxzp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhoulong.xyz/gtypjzcrmj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.andypj.xyz/gtcudfhvnb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cdnleiting.top/gtcsfyyjsv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhiwuduotai.top/gtdwhbsylh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.guannengcc.top/gtgtxcabva.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.gogol.net.cn/gtysujlfxi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ybcxt.top/gtknjtuzvd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jianghu66.top/gtogqumrfs.html

[E19] 多行文本按行拆分
来源：http://hz.cheryme.top/gtmiyuhywr.html

Py:   s.splitlines()
来源：http://hz.jinqigufen.top/gtmvpzqerc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.tian-w.cn/gthbxoizgn.html

JS:   s.split(/\r?\n/)
来源：http://hz.havefunace.top/gtbulbsbwz.html

TS:   s.split(/\r?\n/)
来源：http://hz.jinyuanbaomall.cn/gtyuilelvc.html

Java: s.lines().toList()
来源：http://hz.c1oappe.top/gtysxkxpbo.html

Go:   strings.Split(s, "\n")
来源：http://hz.chenzaomai.com/gtbhkybfhh.html

Ruby: s.lines
来源：http://hz.jinqigufen.top/gtxijtfsuz.html

C#:   s.Split('\n')
来源：http://hz.iojbl.cn/gtzgzfprtk.html

[E20] 判断字符串是否为空
来源：http://hz.hammf.cn/gtwlizjuzl.html

Py:   if not s:
来源：http://hz.sufxvd.cn/gthevljrnq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinyuanbaomall.cn/gtmaoxreiw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.snrcjt.cn/gtyngmsjkh.html

TS:   if (s === "") {}
来源：http://hz.ybcxt.top/gtcrrzrvsz.html

Java: if (s.isEmpty()) {}
来源：http://hz.zycfv.cn/gtmvwredbz.html

Go:   if s == "" {}
来源：http://hz.tian-w.cn/gtpplondaa.html

Ruby: if s.empty?
来源：http://hz.yangfankeji.com/gtwvytcdsr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.nanxinkj.top/gtspnwwazl.html

[E21] 超长截断加省略号
来源：http://hz.shangyingyoupin.top/gteyegfgqv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shanyushiyangtech.top/gttfxiaxon.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gtyyhpyaqm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhongyouzk.top/gtcaahnabo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sufxvd.cn/gtxhccdefq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sysykeji.top/gtyjuyukvq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhixingplan.top/gtqafflbgh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.snrcjt.cn/gtziqwdeli.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gogol.net.cn/gtqqxxmkuw.html

[E22] 字节长度与字符长度
来源：http://hz.guannengcc.top/gttihttckd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jianghu66.top/gtojbrcppg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.daxiang520.top/gtqsiioqim.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sufxvd.cn/gtmhgccszw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangkeji.top/gtupzhemll.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hfpthk.cn/gtlxypdwdl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.kuanghao11.cn/gtlfetadse.html

Ruby: s.bytesize;  s.length
来源：http://hz.jlsjyb.cn/gteruxojyx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gzhubu.top/gtlcvortnp.html

================================================================================
来源：http://hz.zdqjudy.top/gtxqvdcwil.html

F. 文件与目录
来源：http://hz.gotoacloud.top/gtifmqqnca.html

================================================================================
来源：http://hz.yuanzhike.top/gtzhnbtykk.html

[F01] 读取整个文件
来源：http://hz.sxryk.cn/gtwyrsmiqe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.tanke756.top/gtqoksnpnj.html

PHP:  file_get_contents("a.txt");
来源：http://hz.wangdashe.top/gtctsbzzdo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.dashuyun.cn/gtxoopwnjx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.wangshuangyany.cn/gteyvevbrx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gthkceuryv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.sxryk.cn/gtyiccqejq.html

Ruby: File.read("a.txt")
来源：http://hz.bjfxy.top/gtiusxtonu.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhijiandao.cn/gtqzthvvfx.html

[F02] 逐行读取文件
来源：http://hz.daxiang520.top/gtweoalbnm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.fengsongda.top/gtbhypkmeb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.vqdsnc.cn/gtdckkyqzf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xylfe.cn/gtsuivasae.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.vqdsnc.cn/gtnsstivdd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xuanzx.com/gtzmobvpok.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.kuanghao11.cn/gtbrbrmglv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yanxiufei.cn/gtnyujunrh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.bjfxy.top/gtvqutiajh.html

[F03] 写入文件（覆盖）
来源：http://hz.yongpay.top/gtlsnlbdra.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.meibo888.top/gtzvwsurqz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hnqzz.top/gtxevkfzwq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gaohongyu789.top/gtquhlwhwn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xingfuxueyuan.xyz/gtfwtzepss.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhiwuduotai.top/gtcfgmkcuo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cdnleiting.top/gtvjbzrmiq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.meibo888.top/gtjqwhausq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yvedp.cn/gtmiuhwxid.html

[F04] 追加写入文件
来源：http://hz.ybcxt.top/gtvswymoeu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.guannengcc.top/gtovndowyn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.316326.xyz/gtobglpefg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cdnleiting.top/gtmwicknyi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258888.top/gtdqdrleog.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ivvv.top/gtziirenbc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.dashuyun.cn/gtmisiftdg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.bjfxy.top/gtduenfjuf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.smart0.xyz/gtrqvpmawl.html

[F05] 判断文件或目录是否存在
来源：http://hz.yangfankeji.com/gttqgkkrnz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jianghu66.top/gtfxiqdthz.html

PHP:  file_exists("a.txt");
来源：http://hz.yuxming.cn/gtaorcudmz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gzhubu.top/gtiwasybyi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jinqigfzy.top/gtczezeejs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtttaktone.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.mhx1999.top/gtzqhayhfj.html

Ruby: File.exist?("a.txt")
来源：http://hz.daxiang520.top/gtnntblniz.html

C#:   File.Exists("a.txt")
来源：http://hz.sxryk.cn/gtbfumjyqv.html

[F06] 删除文件
来源：http://hz.ybcxt.top/gtzlpheioo.html

Py:   os.remove("a.txt")
来源：http://hz.fzhhl.top/gthzslwiru.html

PHP:  unlink("a.txt");
来源：http://hz.tianlin.xyz/gtmaxdtlay.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.vqdsnc.cn/gtaexxgatf.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgfzy.top/gtljbvjvkf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.pengpengdd.cyou/gtyzdwuikg.html

Go:   os.Remove("a.txt")
来源：http://hz.dashuyun.cn/gtvtlqcakn.html

Ruby: File.delete("a.txt")
来源：http://hz.shzxlz.cn/gtqfatwmjq.html

C#:   File.Delete("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtthvuuctv.html

[F07] 创建目录（含多级）
来源：http://hz.hammf.cn/gtkwmdyzxf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yj20258.top/gtmkihlvge.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ywan-chungtsiang.top/gtwcmqrfly.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tianlin.xyz/gtujtzytex.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tanke756.top/gtdgmbidpt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shangyingyoupin.top/gtalidydnb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.52xcode.cn/gtybcjwdcq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yuxming.cn/gtggfuyngt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenjidiqi.icu/gtawufxnqh.html

[F08] 遍历目录
来源：http://hz.vqdsnc.cn/gtuawmpfxh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj20258888.top/gtdumvasqd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinqigufen.top/gtbpuoyjuw.html

JS:   fs.readdirSync("dir")
来源：http://hz.fengsongda.top/gtdiajarhu.html

TS:   fs.readdirSync("dir")
来源：http://hz.316326.xyz/gttiswpkqi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.svipenyu.cn/gtdltxwpkf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ehwqpu.com/gtajqdfueb.html

Ruby: Dir.children("dir")
来源：http://hz.xziqi.cn/gtdxlazisn.html

C#:   Directory.GetFiles("dir")
来源：http://hz.52xcode.cn/gtrcrrfwtv.html

[F09] 获取文件大小
来源：http://hz.cashguo.top/gtvfbdfenz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yongpay.top/gtkozjiyey.html

PHP:  filesize("a.txt");
来源：http://hz.yueranfly.top/gtotlcbvid.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hongshengwenyu.top/gtvzpwmxsh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.fzhhl.top/gtujqoxqwe.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.gzhubu.top/gtikttmsaz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.nanxinkj.top/gtfhewhvmf.html

Ruby: File.size("a.txt")
来源：http://hz.ppjwa.cn/gtdbhzaoxh.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cqqwz.cn/gtpnotmzpe.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.316326.xyz/gtbulgfmfj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cashguo.top/gtwxewctqy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yuanzhike.top/gtqlicqhah.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtmjrugncj.html

TS:   path.extname("a.txt")
来源：http://hz.nanxinkj.top/gtttzqrkzi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.guowangkeji.top/gtxqwsuwuz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.tianlin.xyz/gtrcsfrqyb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtodddiocc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.tanke756.top/gtmhuyitlm.html

[F11] 复制与移动文件
来源：http://hz.yangfankeji.com/gtabmwykla.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gtkagrggce.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gzhubu.top/gthohuqent.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtamlsryod.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtgvtuftvv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.iojbl.cn/gtdxoqtzgu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.redwolf501.top/gtfbnfcbhf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gtpltlyptq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xinyue.icu/gthtqpfgum.html

[F12] CSV 读写
来源：http://hz.yongpay.top/gtvtthsvwa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.wangshuangyany.cn/gtuifeeghe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yj20258.top/gtnbicpmjl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj202588.top/gtyssetgik.html

TS:   // 同上
来源：http://hz.yanxiufei.cn/gtvvekayzt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.c1oappe.top/gtknapitgm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.birdmap.top/gtjbzgvnvw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.guannengcc.top/gtzurrfsvs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gotoacloud.top/gtjfxspkyh.html

================================================================================
来源：http://hz.hysaishi.cn/gtwzlwlgox.html

G. 面向对象
来源：http://hz.jinqigfzy.top/gtvmwzayap.html

================================================================================
来源：http://hz.sxryk.cn/gtpsieqilw.html

[G01] 定义类
来源：http://hz.zhiwuduotai.top/gtrjwwforo.html

Py:   class User: pass
来源：http://hz.sweek.top/gtfcjbulxz.html

PHP:  class User {}
来源：http://hz.316326.xyz/gtgsczuevy.html

JS:   class User {}
来源：http://hz.jiagoushi.top/gtzsfpublf.html

TS:   class User { name: string = ""; }
来源：http://hz.yongpay.top/gtcfknqnih.html

Java: class User {}
来源：http://hz.yueranfly.top/gtaxwnodal.html

Go:   type User struct { Name string }
来源：http://hz.yongpay.top/gtuwwjzhue.html

Ruby: class User; end
来源：http://hz.jqgufenzy.top/gtmluqfuws.html

C#:   class User {}
来源：http://hz.zycfv.cn/gtuiveaarl.html

[G02] 构造函数
来源：http://hz.hongshengwenyu.top/gtvgtqekez.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jiagoushi.top/gtwjnjgkio.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.aibaodan.cn/gtpyfezpln.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.52xcode.cn/gtjrgvzykq.html

TS:   constructor(public name: string) {}
来源：http://hz.shanyushiyangtech.top/gtlqnfujyy.html

Java: User(String name) { this.name = name; }
来源：http://hz.yuanzhike.top/gtqhxhptez.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gaohongyu789.top/gtpkryaapx.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenzaomai.com/gtqspnnatg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.svipenyu.cn/gtbwlgavnl.html

[G03] 实例属性
来源：http://hz.hywenlv.cn/gtanlxppaj.html

Py:   self.name = "x"
来源：http://hz.xziqi.cn/gtrdeijzlw.html

PHP:  public string $name = "x";
来源：http://hz.tanke756.top/gtbaaeevvv.html

JS:   this.name = "x";
来源：http://hz.ivvv.top/gtpwghzveg.html

TS:   name: string = "x";
来源：http://hz.tianlin.xyz/gtfhhngqld.html

Java: private String name;
来源：http://hz.zdqjudy.top/gtlbuumsvs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.pengpengdd.cyou/gtvfwxdnre.html


<!-- 参考信息 -->