代发 wailian999

Ruby: s.split(",");  s.split
来源：http://hz.fzhhl.top/gtnyqblliq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yonumen.top/gtbibfqgyf.html

[E08] 数组按分隔符合并
来源：http://hz.nwbrower.top/gtbsnisdne.html

Py:   ",".join(items)
来源：http://hz.jinyuanbaomall.cn/gtenhnwvei.html

PHP:  implode(",", $items);
来源：http://hz.tian-w.cn/gttyuapgis.html

JS:   items.join(",")
来源：http://hz.yueranfly.top/gtntmhijcs.html

TS:   items.join(",")
来源：http://hz.ydjk.org.cn/gtbgjepjbo.html

Java: String.join(",", items)
来源：http://hz.zhoulong.xyz/gtossxjwpf.html

Go:   strings.Join(items, ",")
来源：http://hz.pycfn.com/gtzvfbfnrh.html

Ruby: items.join(",")
来源：http://hz.snrcjt.cn/gtnmsktclw.html

C#:   string.Join(",", items)
来源：http://hz.cqqwz.cn/gtnsrejlck.html

[E09] 去除所有空白字符
来源：http://hz.daxiang520.top/gtrmeaufgv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jinqigufen.top/gtuvalwywp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zdqjudy.top/gtuhbxidem.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yj202588.top/gtnmbwqtlk.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yangfankeji.com/gtktkiorkz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.nanxinkj.top/gtiocjacsi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jiagoushi.top/gtwcsejnss.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cucudq.cn/gtmmaenjzv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zycfv.cn/gtifzrrdex.html

[E10] 左侧补零 / 定长填充
来源：http://hz.9152youxi.cn/gthaoyapcm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shanyushiyangkeji.top/gtrspidvzv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.wangshuangyany.cn/gtnfrvfhsj.html

JS:   "7".padStart(3, "0")
来源：http://hz.cdnleiting.top/gtyavjzpjr.html

TS:   "7".padStart(3, "0")
来源：http://hz.chenlongwang.top/gtxyllcsmp.html

Java: String.format("%03d", 7)
来源：http://hz.cashguo.top/gtafwckpqw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ydzc1.top/gtviufvrcy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.c1oappe.top/gthnbrlizp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yonumen.top/gtswfkcmir.html

[E11] 反转字符串
来源：http://hz.yj20258.top/gtlevdlmaa.html

Py:   s[::-1]
来源：http://hz.zhongyouzk.top/gtrjikkgpv.html

PHP:  strrev($s);
来源：http://hz.shuidangran.top/gtriigttlb.html

JS:   [...s].reverse().join("")
来源：http://hz.c1oappe.top/gtavgcqesa.html

TS:   [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gteekatnde.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.chenlongwang.top/gtsqijtmph.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jqgfzy.top/gtrelapbss.html

Ruby: s.reverse
来源：http://hz.yueranfly.top/gtjprxpijn.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hongshengwenyu.top/gtaadxgqgs.html

[E12] 统计某字符出现次数
来源：http://hz.yuanzhike.top/gtrcaowmok.html

Py:   s.count("a")
来源：http://hz.fzhhl.top/gtkmzgdhdm.html

PHP:  substr_count($s, "a");
来源：http://hz.zhaomingkeji.xyz/gtqfazocqg.html

JS:   s.split("a").length - 1
来源：http://hz.jinghuilouyu.cn/gtoxzgccbz.html

TS:   s.split("a").length - 1
来源：http://hz.fzhhl.top/gtgolekmiv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.daria6918.cn/gtcphavxbh.html

Go:   strings.Count(s, "a")
来源：http://hz.ppjwa.cn/gttsoqrkiq.html

Ruby: s.count("a")
来源：http://hz.mhx1999.top/gtlqrvonwl.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhaomingkeji.xyz/gtnklyqyfb.html

[E13] 逐字符遍历
来源：http://hz.cheryme.top/gttegepjce.html

Py:   for ch in s: print(ch)
来源：http://hz.yuxming.cn/gthrmqatcc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gzhubu.top/gtvnkwtrfb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangdashe.top/gtqddoabod.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.dashuyun.cn/gtyqysrqba.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.vqdsnc.cn/gtmmgvrrjj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.nanxinkj.top/gtctvzfmvq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yuanzhike.top/gtwirvbpig.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shanyushiyangtech.top/gtnzssvtwy.html

[E14] URL 编码与 Base64
来源：http://hz.jlsjyb.cn/gtgwoaijej.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhoulong.xyz/gtlingqtqt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.316326.xyz/gtiuwvzkua.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ywan-chungtsiang.top/gtetxaickk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jinqigufen.top/gtaosxfgju.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yuanzhike.top/gtqgokjjye.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.svipenyu.cn/gtrualjopo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.daria6918.cn/gtbtzpaynx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yanxiufei.cn/gtdifedsty.html

[E15] HTML 转义 / 反转义
来源：http://hz.tanke756.top/gtghnwdyxl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yvedp.cn/gtaztrhaci.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.nwbrower.top/gthfhziuth.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cucudq.cn/gtvacsnyhw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.chenjidiqi.icu/gthspehadt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yj20258.top/gtssgzirrt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhijiandao.cn/gtltgczkzn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gzhubu.top/gtjvpeputr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gzhubu.top/gtsaofzzqq.html

[E16] 数字千分位
来源：http://hz.jinqigfzy.top/gtfiwrvdbf.html

Py:   f"{1234567:,}"
来源：http://hz.meibo888.top/gtlpmlovlo.html

PHP:  number_format(1234567);
来源：http://hz.ydjk.org.cn/gtwrhshxcp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.wangshuangyany.cn/gtchqcaylu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.kuanghao11.cn/gtizpsgbjt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.meibo888.top/gtrndjdxvo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jiagoushi.top/gtkfyemoya.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cdnleiting.top/gtdruymuqo.html

C#:   1234567.ToString("N0")
来源：http://hz.cheryme.top/gtixdtquzc.html

[E17] 首字母大写
来源：http://hz.zhiwuduotai.top/gtdjddaatf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xuetiantiany.cn/gtgrnoworz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.dianchejie.cn/gtfgrrtovm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tanke756.top/gtmmdvzglc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.mhx1999.top/gtdffzegwm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.daxiang520.top/gtysqwldyy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.52xcode.cn/gtvxpwhmmi.html

Ruby: s.capitalize
来源：http://hz.bjfxy.top/gtiipkkbfb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hammf.cn/gtztjrvbll.html

[E18] 模板占位符替换
来源：http://hz.cucudq.cn/gtmnxgtqhe.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.wangshuangyany.cn/gtpyqdpmcj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shuidangran.top/gtswfrakxp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxuanxn.top/gteexjulai.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.feifeiyinyue.top/gtpwqyxvoa.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hnxiangtu.top/gtnwpvfbgk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.svipenyu.cn/gtzbvyvmjt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.nanxuanxn.top/gtgzjnludj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.bjfxy.top/gtpduzakjl.html

[E19] 多行文本按行拆分
来源：http://hz.hfpthk.cn/gtxdzshcjp.html

Py:   s.splitlines()
来源：http://hz.wangdashe.top/gtohatssmz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.smart0.xyz/gtmdmdopdh.html

JS:   s.split(/\r?\n/)
来源：http://hz.hammf.cn/gtgbyjiygb.html

TS:   s.split(/\r?\n/)
来源：http://hz.tianlin.xyz/gtaovajsnh.html

Java: s.lines().toList()
来源：http://hz.shangyingyoupin.top/gtvkxmikqg.html

Go:   strings.Split(s, "\n")
来源：http://hz.xziqi.cn/gtmugjvyff.html

Ruby: s.lines
来源：http://hz.yj20258888.top/gtnobwgmxu.html

C#:   s.Split('\n')
来源：http://hz.zhoulong.xyz/gtazcrgequ.html

[E20] 判断字符串是否为空
来源：http://hz.zhixingplan.top/gtdotenpae.html

Py:   if not s:
来源：http://hz.chenjidiqi.icu/gtzhjlcdip.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.c1oappe.top/gtjpmctchf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sysykeji.top/gtztmlbzvq.html

TS:   if (s === "") {}
来源：http://hz.zdqjudy.top/gtuinrjugf.html

Java: if (s.isEmpty()) {}
来源：http://hz.yuxming.cn/gtnseszyjh.html

Go:   if s == "" {}
来源：http://hz.dianchejie.cn/gthmgtxvvy.html

Ruby: if s.empty?
来源：http://hz.ivvv.top/gtnecxwzwu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ydjk.org.cn/gtwgplbiea.html

[E21] 超长截断加省略号
来源：http://hz.daria6918.cn/gtgwxzwowm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.birdmap.top/gtbmdaxbyp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.dashuyun.cn/gtatnqqpmb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtnsgiipno.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aizwys.cn/gtynyozpfz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtilwjoosx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.redwolf501.top/gtludveelz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.dianchejie.cn/gtuirgpubr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.pycfn.com/gtyxvuphfu.html

[E22] 字节长度与字符长度
来源：http://hz.9152youxi.cn/gtgncrmcwc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.dianchejie.cn/gtukvuvcik.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ydzc1.top/gtjnhsdepw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydjk.org.cn/gttskhotio.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yonumen.top/gttwgfedhj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinghuilouyu.cn/gtkonnrcbl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hfpthk.cn/gtltohyxdh.html

Ruby: s.bytesize;  s.length
来源：http://hz.smart0.xyz/gtgujfqpgf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.svipenyu.cn/gtgxssilwu.html

================================================================================
来源：http://hz.sxryk.cn/gtxshxxzwd.html

F. 文件与目录
来源：http://hz.shanyushiyangtech.top/gtdxgrxgcq.html

================================================================================
来源：http://hz.jinqigufen.top/gtafnajwac.html

[F01] 读取整个文件
来源：http://hz.zhoulong.xyz/gtbwiassix.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.shanyushiyangtech.top/gtmixyssfd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tanke756.top/gtfrdvjbtn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ydjk.org.cn/gtaubfsulx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shzxlz.cn/gtiwlvqnzl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gtinrleint.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shanyushiyangkeji.top/gtbqliervs.html

Ruby: File.read("a.txt")
来源：http://hz.tian-w.cn/gtknvfqncr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yangfankeji.com/gtrtbboqam.html

[F02] 逐行读取文件
来源：http://hz.aibaodan.cn/gtnexbfphu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinqigufen.top/gttcrdynqi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.tianlin.xyz/gtzcofkgmn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zycfv.cn/gtvyxkwani.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinyuanbaomall.cn/gtxvemnxnu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.wangdashe.top/gtmplgmkdf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.guowangkeji.top/gtdzinwvph.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shzxlz.cn/gtmtiwoinl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.9152youxi.cn/gtkxnsjbft.html

[F03] 写入文件（覆盖）
来源：http://hz.zhoulong.xyz/gtcdifkill.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jyoumei.cn/gtplrghijr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shuidangran.top/gtsbjlwgub.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zdqjudy.top/gtaddobwnu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhoulong.xyz/gtxloysbxf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.0kj1m.cn/gthlqwfkpl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhongyouzk.top/gthskuraxp.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hfpthk.cn/gtolofarrs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhiwuduotai.top/gtobplvhqv.html

[F04] 追加写入文件
来源：http://hz.shzxlz.cn/gtflogccvu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.havefunace.top/gtnxiyzqga.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zdqjudy.top/gtujbdumyj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinyuanbaomall.cn/gtogtzgcyt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangtech.top/gthoegmqfo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhongyouzk.top/gtvtrgirai.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.dashuyun.cn/gtyckdsuph.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.pycfn.com/gtmcoutytp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gaohongyu789.top/gtpbauycon.html

[F05] 判断文件或目录是否存在
来源：http://hz.yueranfly.top/gturfqfxog.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ywan-chungtsiang.top/gtmypmuhzy.html

PHP:  file_exists("a.txt");
来源：http://hz.sysykeji.top/gtrugdxjyj.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gaohongyu789.top/gttengbaun.html

TS:   fs.existsSync("a.txt")
来源：http://hz.sxryk.cn/gtpuqkwefq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hammf.cn/gtakptqgxl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.aizwys.cn/gthpoekhim.html

Ruby: File.exist?("a.txt")
来源：http://hz.aibaodan.cn/gtyxprkoqu.html

C#:   File.Exists("a.txt")
来源：http://hz.yonumen.top/gtndviybrm.html

[F06] 删除文件
来源：http://hz.yvedp.cn/gthzgjtdsc.html

Py:   os.remove("a.txt")
来源：http://hz.gotoacloud.top/gtsmzqqfsn.html

PHP:  unlink("a.txt");
来源：http://hz.guannengcc.top/gtvvemishv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yueranfly.top/gtjqprbspa.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jyoumei.cn/gtjcuwjwnn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yj20258888.top/gtnrjggifo.html

Go:   os.Remove("a.txt")
来源：http://hz.haohaochexian.top/gtuahdcvhv.html

Ruby: File.delete("a.txt")
来源：http://hz.zhoulong.xyz/gthxoovzfn.html

C#:   File.Delete("a.txt");
来源：http://hz.gaohongyu789.top/gtwazwodfk.html

[F07] 创建目录（含多级）
来源：http://hz.gaohongyu789.top/gttbcaydnv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hywenlv.cn/gtntuiutls.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ywan-chungtsiang.top/gtgmogvyxe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yvedp.cn/gtocfsvbit.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dashuyun.cn/gtyxdtebhv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yangfankeji.com/gtuljoxhrh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sufxvd.cn/gtvmptlegj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yj20258888.top/gtprrfmcro.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cdnleiting.top/gtssbsortk.html

[F08] 遍历目录
来源：http://hz.chenzaomai.com/gttjzcpvzz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cucudq.cn/gtqbrhuote.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhoulong.xyz/gtdorcmydy.html

JS:   fs.readdirSync("dir")
来源：http://hz.hnxiangtu.top/gtlatsgaty.html

TS:   fs.readdirSync("dir")
来源：http://hz.mhx1999.top/gtkfjoiwfi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ydzc1.top/gtcfdgzivy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cashguo.top/gtnatfgbpo.html

Ruby: Dir.children("dir")
来源：http://hz.yueranfly.top/gtnfcfpbpu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yanxiufei.cn/gtciqappna.html

[F09] 获取文件大小
来源：http://hz.yangfankeji.com/gtfbcwfnmk.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gogol.net.cn/gtdxzkvhqm.html

PHP:  filesize("a.txt");
来源：http://hz.andypj.xyz/gtrnydzqki.html

JS:   fs.statSync("a.txt").size
来源：http://hz.haohaochexian.top/gtiaiczqhk.html

TS:   fs.statSync("a.txt").size
来源：http://hz.chenlongwang.top/gtpwkveily.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gtqecupwfp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xuetiantiany.cn/gtaqigircc.html

Ruby: File.size("a.txt")
来源：http://hz.wangshuangyany.cn/gtfkjrvekk.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.tianlin.xyz/gtrmaydist.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinyuanbaomall.cn/gtbeocswgn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.daria6918.cn/gtqrukqvll.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ivvv.top/gtlqdqgjkj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jqgfzy.top/gtuzrjjtlk.html

TS:   path.extname("a.txt")
来源：http://hz.c1oappe.top/gtubnkwanq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xziqi.cn/gtvbdewcpa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtfhoerhph.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xinyue.icu/gtloddwvfm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtugnqztpu.html

[F11] 复制与移动文件
来源：http://hz.yj20258888.top/gtllsemfaw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtubxdjitj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xziqi.cn/gtfqgmqpym.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtbvxbhuht.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gtjfyaikxx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shuidangran.top/gtecjulopt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yvedp.cn/gtybmqpvhj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtdcmptakm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sxryk.cn/gttvjcbtgs.html

[F12] CSV 读写
来源：http://hz.jqgfzy.top/gtnpdbofqx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yj202588.top/gtqfkpglwt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.fzhhl.top/gtqrhyuvrr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hnqzz.top/gtrmlnmdwb.html

TS:   // 同上
来源：http://hz.zhongyouzk.top/gtuwzwwsvl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tanke756.top/gtvwsmqqwx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhiwuduotai.top/gtmjfilmbq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhaomingkeji.xyz/gtnusmpere.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.0kj1m.cn/gtamvurrgt.html

================================================================================
来源：http://hz.svipenyu.cn/gtwanzeedt.html

G. 面向对象
来源：http://hz.jyoumei.cn/gtazyrwoeb.html

================================================================================
来源：http://hz.ydzc1.top/gtmjvenfyr.html

[G01] 定义类
来源：http://hz.xinyue.icu/gtbasgsqea.html

Py:   class User: pass
来源：http://hz.snrcjt.cn/gtlyyvvybv.html

PHP:  class User {}
来源：http://hz.zdqjudy.top/gtrqgeoirk.html

JS:   class User {}
来源：http://hz.yuanzhike.top/gtelzjwzmg.html

TS:   class User { name: string = ""; }
来源：http://hz.daxiang520.top/gthlozbjkp.html

Java: class User {}
来源：http://hz.zhongyouzk.top/gtsyhxfkof.html

Go:   type User struct { Name string }
来源：http://hz.tanke756.top/gtkdigbhce.html

Ruby: class User; end
来源：http://hz.jlsjyb.cn/gtgcyvcsci.html

C#:   class User {}
来源：http://hz.dashuyun.cn/gtwzeysyey.html

[G02] 构造函数
来源：http://hz.iojbl.cn/gtzrhggjkq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yvedp.cn/gtbvwnlznh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sweek.top/gtokfvujjj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yongpay.top/gttevampyg.html

TS:   constructor(public name: string) {}
来源：http://hz.ydjk.org.cn/gtxgrwiqog.html

Java: User(String name) { this.name = name; }
来源：http://hz.yongpay.top/gttkbevfkt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hammf.cn/gtudzwkfqt.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhengqikj.top/gtnvgdglox.html

C#:   public User(string name) { Name = name; }
来源：http://hz.52xcode.cn/gthenneugi.html

[G03] 实例属性
来源：http://hz.zhijiandao.cn/gtoddfgalj.html

Py:   self.name = "x"
来源：http://hz.zhixingplan.top/gtpfvmqpde.html

PHP:  public string $name = "x";
来源：http://hz.zdqjudy.top/gtfyxjrtvh.html

JS:   this.name = "x";
来源：http://hz.nanxinkj.top/gtibcqsyar.html

TS:   name: string = "x";
来源：http://hz.zhijiandao.cn/gteewrqhgn.html

Java: private String name;
来源：http://hz.cucudq.cn/gthlifaqmf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.meibo888.top/gtjkpzzwxi.html

Ruby: @name = "x"
来源：http://hz.zhijiandao.cn/gtusizkuve.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.andypj.xyz/gtsykuqrtw.html

[G04] 定义方法
来源：http://hz.pycfn.com/gtthbwofqg.html

Py:   def greet(self): return self.name
来源：http://hz.meibo888.top/gtwbruxvnp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.dianchejie.cn/gttablwdez.html

JS:   greet() { return this.name; }
来源：http://hz.hywenlv.cn/gtzymalbdw.html

TS:   greet(): string { return this.name; }
来源：http://hz.aizwys.cn/gtoumohpiy.html

Java: String greet() { return name; }
来源：http://hz.cheryme.top/gtubqwaehn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhengqikj.top/gtobyfktay.html

Ruby: def greet; @name; end
来源：http://hz.jiagoushi.top/gtuxkhodxq.html

C#:   public string Greet() => Name;
来源：http://hz.nanxuanxn.top/gtyumgvmuv.html

[G05] 继承
来源：http://hz.chenlongwang.top/gthmvedcuo.html

Py:   class Admin(User): pass
来源：http://hz.sxryk.cn/gtzxxiuhtp.html

PHP:  class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtmymitzwi.html

JS:   class Admin extends User {}
来源：http://hz.yangfankeji.com/gteflyxdhs.html

TS:   class Admin extends User {}
来源：http://hz.gotoacloud.top/gtmftconre.html

Java: class Admin extends User {}
来源：http://hz.meibo888.top/gtmfgspepm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj20258.top/gtebsbiuvw.html

Ruby: class Admin < User; end
来源：http://hz.zhoulong.xyz/gtjgcsuern.html

C#:   class Admin : User {}
来源：http://hz.pycfn.com/gtvbktutqo.html

[G06] 重写方法
来源：http://hz.tian-w.cn/gtweomlkto.html

Py:   def greet(self): return "admin"
来源：http://hz.mhx1999.top/gtuzmdveef.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jiagoushi.top/gtlcrusgqe.html

JS:   greet() { return "admin"; }
来源：http://hz.aizwys.cn/gthorljbnh.html


<!-- 参考信息 -->