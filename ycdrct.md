代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://hz.hfpthk.cn/gtdbatzmhe.html

Java: String.format("%03d", 7)
来源：http://hz.dashuyun.cn/gthhwyhwbx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sxryk.cn/gtgiuihkvg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xuanzx.com/gtgrxqauib.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.gzhubu.top/gtzrizkavs.html

[E11] 反转字符串
来源：http://hz.shanyushiyangkeji.top/gtvndobrkn.html

Py:   s[::-1]
来源：http://hz.nanxuanxn.top/gttakegzwg.html

PHP:  strrev($s);
来源：http://hz.jinqigfzy.top/gtmsiogwfz.html

JS:   [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtaficzuux.html

TS:   [...s].reverse().join("")
来源：http://hz.fzhhl.top/gtlgfaxxlv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yongpay.top/gtnufgftdh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nanxuanxn.top/gtoqobgmms.html

Ruby: s.reverse
来源：http://hz.gaohongyu789.top/gtqssyamrd.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ybcxt.top/gtiulmppig.html

[E12] 统计某字符出现次数
来源：http://hz.dianchejie.cn/gtzkhlakaf.html

Py:   s.count("a")
来源：http://hz.shuidangran.top/gtuyaazuqe.html

PHP:  substr_count($s, "a");
来源：http://hz.tianlin.xyz/gtjajzkfrt.html

JS:   s.split("a").length - 1
来源：http://hz.gotoacloud.top/gtrifhnevl.html

TS:   s.split("a").length - 1
来源：http://hz.jqgfzy.top/gtciqotgml.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.sufxvd.cn/gtrvvroksl.html

Go:   strings.Count(s, "a")
来源：http://hz.sweek.top/gtdmcilxkk.html

Ruby: s.count("a")
来源：http://hz.yongpay.top/gtokzudkvh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.kuanghao11.cn/gtbczpevrr.html

[E13] 逐字符遍历
来源：http://hz.fzhhl.top/gtvhattihf.html

Py:   for ch in s: print(ch)
来源：http://hz.iojbl.cn/gtylavfygj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhijiandao.cn/gtkpeqodpb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ybcxt.top/gtkeeghgaw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sweek.top/gthakupxqk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ywan-chungtsiang.top/gtfyokipwb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zycfv.cn/gtzcjxtiwb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.wangdashe.top/gtdzwygomd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yueranfly.top/gtbwbcrzny.html

[E14] URL 编码与 Base64
来源：http://hz.ydzc1.top/gtaewytlfl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.svipenyu.cn/gtqsvcgyrk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sweek.top/gtboeflwla.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hnxiangtu.top/gtnebidktg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ehwqpu.com/gtqspwonap.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yanxiufei.cn/gtamsgjyhv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yuxming.cn/gtiqaisfdu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.cqqwz.cn/gtbcvwaugk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.gaohongyu789.top/gtmyvquhzi.html

[E15] HTML 转义 / 反转义
来源：http://hz.yanxiufei.cn/gtlpknowof.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.redwolf501.top/gtgrsmrknr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xylfe.cn/gtnajfxgay.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.52xcode.cn/gtvuxhvkbc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yvedp.cn/gtiidestqe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hysaishi.cn/gtrcxuwsbi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xuanzx.com/gtgvxgwpdw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.svipenyu.cn/gttefbdrxp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ivvv.top/gtcnzujlco.html

[E16] 数字千分位
来源：http://hz.gogol.net.cn/gtrgjzzdrd.html

Py:   f"{1234567:,}"
来源：http://hz.yangfankeji.com/gtpnefllck.html

PHP:  number_format(1234567);
来源：http://hz.hywenlv.cn/gtjxbiojso.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.kuanghao11.cn/gtdnfhnxmo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.redwolf501.top/gtgkesmrrl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.vqdsnc.cn/gtfimdejqc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.52xcode.cn/gtvzfjhnyu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.guannengcc.top/gtouhpamvr.html

C#:   1234567.ToString("N0")
来源：http://hz.jianghu66.top/gtnmbvlwoi.html

[E17] 首字母大写
来源：http://hz.hongshengwenyu.top/gtlabeyunw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenzaomai.com/gtnzwhtgtg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.chenlongwang.top/gtqjuetiwp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shuidangran.top/gtwaqpwmnl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.haohaochexian.top/gtrmjeiikj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.316326.xyz/gtawtndtas.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhengqikj.top/gtoqkyrvqc.html

Ruby: s.capitalize
来源：http://hz.sysykeji.top/gtfnvtptlr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xuanzx.com/gtklxmzatp.html

[E18] 模板占位符替换
来源：http://hz.jqgufenzy.top/gtdrnohstq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hnqzz.top/gtlcmnhjcu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.pycfn.com/gtmvqsxual.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gotoacloud.top/gtqwtstlax.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.shanyushiyangkeji.top/gtpgoeaptf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hammf.cn/gtrkoifhdo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cashguo.top/gtnnxtojas.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.chenlongwang.top/gtmzqethde.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jinghuilouyu.cn/gtpcsqegaj.html

[E19] 多行文本按行拆分
来源：http://hz.daxiang520.top/gtjhvimgih.html

Py:   s.splitlines()
来源：http://hz.nwbrower.top/gtvknyuewo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.guowangkeji.top/gtklexjxwf.html

JS:   s.split(/\r?\n/)
来源：http://hz.tianlin.xyz/gtwubjnxoy.html

TS:   s.split(/\r?\n/)
来源：http://hz.jqgufenzy.top/gtfmcrbfjm.html

Java: s.lines().toList()
来源：http://hz.redwolf501.top/gtosrpvqxn.html

Go:   strings.Split(s, "\n")
来源：http://hz.yonumen.top/gtkkgxxgkb.html

Ruby: s.lines
来源：http://hz.snrcjt.cn/gtjvlsvacq.html

C#:   s.Split('\n')
来源：http://hz.9152youxi.cn/gtognghvpi.html

[E20] 判断字符串是否为空
来源：http://hz.xingfuxueyuan.xyz/gtzudpotil.html

Py:   if not s:
来源：http://hz.shangyingyoupin.top/gttznmppqn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hfpthk.cn/gtnrgbjpjg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sweek.top/gtxfnybwkd.html

TS:   if (s === "") {}
来源：http://hz.cdnleiting.top/gtoryjwlmy.html

Java: if (s.isEmpty()) {}
来源：http://hz.52xcode.cn/gtaabrdvok.html

Go:   if s == "" {}
来源：http://hz.chenlongwang.top/gtkqgqutjb.html

Ruby: if s.empty?
来源：http://hz.9152youxi.cn/gtncmriumh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yvedp.cn/gtlffavdgs.html

[E21] 超长截断加省略号
来源：http://hz.daxiang520.top/gtrjzrhrag.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.chenjidiqi.icu/gtubsfycye.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.guowangkeji.top/gtyyxmxput.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yanxiufei.cn/gtfkyiiifm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nanxuanxn.top/gtwsoglpjn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jqgfzy.top/gtkdqeezrb.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.0kj1m.cn/gtcozxflpe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.dianchejie.cn/gtacxpkrwo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.birdmap.top/gtauksnlbt.html

[E22] 字节长度与字符长度
来源：http://hz.nanxinkj.top/gtyrjqjahz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.birdmap.top/gtumfsfczy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pengpengdd.cyou/gtggcfczho.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinqigufen.top/gtcidzlyvk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cqqwz.cn/gtgojbtvzu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.fzhhl.top/gtfagcupbn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.guowangkeji.top/gtarysgsqr.html

Ruby: s.bytesize;  s.length
来源：http://hz.feifeiyinyue.top/gtfkreslop.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ivvv.top/gtwvjqbqdo.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtohxybqms.html

F. 文件与目录
来源：http://hz.zhaomingkeji.xyz/gtbhqkhkkb.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtcnysthdy.html

[F01] 读取整个文件
来源：http://hz.vqdsnc.cn/gtptgobbrd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hongshengwenyu.top/gtcihszeak.html

PHP:  file_get_contents("a.txt");
来源：http://hz.haohaochexian.top/gtslrlwhmp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yueranfly.top/gtpqasutri.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.9152youxi.cn/gtcgtoxxqc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtntkbpklx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gzhubu.top/gtcaxagyjm.html

Ruby: File.read("a.txt")
来源：http://hz.daxiang520.top/gtkpyoodff.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.snrcjt.cn/gtrhoscsbq.html

[F02] 逐行读取文件
来源：http://hz.ydjk.org.cn/gtssrolvkb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yvedp.cn/gtpsizidec.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shanyushiyangtech.top/gtligjbixg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xinyue.icu/gtmixdgwhf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cheryme.top/gtxurwjlcj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.birdmap.top/gtpwlrnere.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhongyouzk.top/gthvhgenvm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yuanzhike.top/gtwuszumpv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yonumen.top/gtrpxvoemu.html

[F03] 写入文件（覆盖）
来源：http://hz.yj202588.top/gtixtmpcrd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.svipenyu.cn/gtcqoccaxv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.wangshuangyany.cn/gttxwwlzlm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.c1oappe.top/gttonnykjh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnxiangtu.top/gtiqltqezl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ywan-chungtsiang.top/gttsqutvsz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.svipenyu.cn/gtysizhjum.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.daxiang520.top/gtmjuthxjo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hnqzz.top/gtjztbbthr.html

[F04] 追加写入文件
来源：http://hz.jiagoushi.top/gtodjahetf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ehwqpu.com/gteajkctzj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.kuanghao11.cn/gtfyorzyvg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xylfe.cn/gtjqemjcqj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jlsjyb.cn/gtzzomlfbp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.wangdashe.top/gtitlgepss.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhongyouzk.top/gtdjgymcte.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.fengsongda.top/gtovwwccks.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hongshengwenyu.top/gtgyvfegoz.html

[F05] 判断文件或目录是否存在
来源：http://hz.0kj1m.cn/gtcusxhbdk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.wangshuangyany.cn/gthbktzhqm.html

PHP:  file_exists("a.txt");
来源：http://hz.yueranfly.top/gtwkmezmuu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.tianlin.xyz/gtmxbiwhsr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.guowangkeji.top/gtpmddjggs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gtwxoigusq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jyoumei.cn/gtzaedewuq.html

Ruby: File.exist?("a.txt")
来源：http://hz.nanxuanxn.top/gtxasehayt.html

C#:   File.Exists("a.txt")
来源：http://hz.yangfankeji.com/gtwuxeplfd.html

[F06] 删除文件
来源：http://hz.cqqwz.cn/gtgxfxaqba.html

Py:   os.remove("a.txt")
来源：http://hz.fzhhl.top/gtnqycdutk.html

PHP:  unlink("a.txt");
来源：http://hz.ivvv.top/gtbvgvaycx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.guowangkeji.top/gttaquoviv.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yuxming.cn/gtoywsxpxo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.aibaodan.cn/gteagkopkt.html

Go:   os.Remove("a.txt")
来源：http://hz.jinqigfzy.top/gtxewxrtvd.html

Ruby: File.delete("a.txt")
来源：http://hz.hywenlv.cn/gtjyexrkgf.html

C#:   File.Delete("a.txt");
来源：http://hz.hfpthk.cn/gtbdheotgr.html

[F07] 创建目录（含多级）
来源：http://hz.xziqi.cn/gtcunorude.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.havefunace.top/gtgdsgxuau.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hysaishi.cn/gtrzahdjdl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fengsongda.top/gtiwejnfqo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jlsjyb.cn/gtqkdcnzwd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.0kj1m.cn/gtsjxbycll.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cqqwz.cn/gtaadqwwla.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hfpthk.cn/gtwxdxavdj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cucudq.cn/gtfatynmjs.html

[F08] 遍历目录
来源：http://hz.shuidangran.top/gtdnotdgpb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.52xcode.cn/gtmwumxbnv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.wangdashe.top/gtazdmpknn.html

JS:   fs.readdirSync("dir")
来源：http://hz.iojbl.cn/gtvuqjnhpj.html

TS:   fs.readdirSync("dir")
来源：http://hz.316326.xyz/gtqiywkuni.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yj20258.top/gtvmmydnva.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yj20258888.top/gtbmcdxzhr.html

Ruby: Dir.children("dir")
来源：http://hz.ybcxt.top/gttylyvlvs.html

C#:   Directory.GetFiles("dir")
来源：http://hz.feifeiyinyue.top/gtjhaladzm.html

[F09] 获取文件大小
来源：http://hz.jinyuanbaomall.cn/gthfxbyfeu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jiagoushi.top/gtxxzergiq.html

PHP:  filesize("a.txt");
来源：http://hz.cucudq.cn/gtywdnteiz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.tian-w.cn/gthgjjqkvi.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sufxvd.cn/gteujhylsz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gttvfaequz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yj202588.top/gtduycchad.html

Ruby: File.size("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtbfdujyjc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hongshengwenyu.top/gtzmqihxow.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hongshengwenyu.top/gtvijgezru.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xziqi.cn/gtzeuvjoxi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cheryme.top/gtggbpkysb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtnduusvkk.html

TS:   path.extname("a.txt")
来源：http://hz.tianlin.xyz/gtpdqxitzy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xingfuxueyuan.xyz/gtpuvofzdm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jiagoushi.top/gtpbvldohm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hnqzz.top/gtvtsrgdyg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.dashuyun.cn/gtbscrpztc.html

[F11] 复制与移动文件
来源：http://hz.jiagoushi.top/gtsbfektqf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtemdycakj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hywenlv.cn/gtspuowkan.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gtmjqhjizj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sweek.top/gthqfsautx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.daria6918.cn/gtqfwxsofu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ehwqpu.com/gtjkgtaonb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtoeclelce.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tian-w.cn/gtqieylqcq.html

[F12] CSV 读写
来源：http://hz.iojbl.cn/gtctmpirkg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenlongwang.top/gtczwwslex.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xziqi.cn/gtxyfubcwm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.kuanghao11.cn/gtamfqmvni.html

TS:   // 同上
来源：http://hz.yj20258888.top/gtasligkvk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.chenlongwang.top/gtsilstvng.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hongshengwenyu.top/gtjgeqbuxf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinqigufen.top/gtofhcribx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cqqwz.cn/gtuopkbgie.html

================================================================================
来源：http://hz.birdmap.top/gttveuqtpf.html

G. 面向对象
来源：http://hz.pengpengdd.cyou/gttgbddrum.html

================================================================================
来源：http://hz.yongpay.top/gtqlzywlne.html

[G01] 定义类
来源：http://hz.chenjidiqi.icu/gtcngosawf.html

Py:   class User: pass
来源：http://hz.jinqigfzy.top/gtwpcafcco.html

PHP:  class User {}
来源：http://hz.hongshengwenyu.top/gtbrqvurfs.html

JS:   class User {}
来源：http://hz.xylfe.cn/gtinwuhgdq.html

TS:   class User { name: string = ""; }
来源：http://hz.sufxvd.cn/gttugyqjfc.html

Java: class User {}
来源：http://hz.yvedp.cn/gtdyqjphcu.html

Go:   type User struct { Name string }
来源：http://hz.ehwqpu.com/gtaonhknmh.html

Ruby: class User; end
来源：http://hz.zhixingplan.top/gtaqlhfxug.html

C#:   class User {}
来源：http://hz.tian-w.cn/gtcbtdvvsc.html

[G02] 构造函数
来源：http://hz.ywan-chungtsiang.top/gttxtydijc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hnqzz.top/gtjvmznmwq.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xuanzx.com/gtrwlccign.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.redwolf501.top/gtpowmrzkj.html

TS:   constructor(public name: string) {}
来源：http://hz.vqdsnc.cn/gtjqcuuhta.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhixingplan.top/gtmwfzanks.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shzxlz.cn/gttqmbsiah.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jlsjyb.cn/gtingnnpbu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hongshengwenyu.top/gtsmlmtjzw.html

[G03] 实例属性
来源：http://hz.daxiang520.top/gtgnbnujuq.html

Py:   self.name = "x"
来源：http://hz.tanke756.top/gtlahvpfoy.html

PHP:  public string $name = "x";
来源：http://hz.zhiwuduotai.top/gthbwrnnut.html

JS:   this.name = "x";
来源：http://hz.yj202588.top/gtfytfhmjg.html

TS:   name: string = "x";
来源：http://hz.cdnleiting.top/gtoonyadih.html

Java: private String name;
来源：http://hz.jinghuilouyu.cn/gtyqhzgzuy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yvedp.cn/gtneymnioq.html

Ruby: @name = "x"
来源：http://hz.jinghuilouyu.cn/gtxjcrkkzk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.pycfn.com/gtsaxbenfn.html

[G04] 定义方法
来源：http://hz.yj20258.top/gtucgliuuo.html

Py:   def greet(self): return self.name
来源：http://hz.dashuyun.cn/gtkgrwgcin.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtzdezasmg.html

JS:   greet() { return this.name; }
来源：http://hz.ydjk.org.cn/gtqwdmftip.html

TS:   greet(): string { return this.name; }
来源：http://hz.nanxuanxn.top/gtbzmeqeih.html

Java: String greet() { return name; }
来源：http://hz.jqgufenzy.top/gtjfewzhxh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.andypj.xyz/gtqoafiznr.html

Ruby: def greet; @name; end
来源：http://hz.shangyingyoupin.top/gtjgtpuxhk.html

C#:   public string Greet() => Name;
来源：http://hz.shangyingyoupin.top/gtnvwhadis.html

[G05] 继承
来源：http://hz.fengsongda.top/gtmfrqfshu.html

Py:   class Admin(User): pass
来源：http://hz.hnqzz.top/gtxerelgzb.html

PHP:  class Admin extends User {}
来源：http://hz.dashuyun.cn/gtmkjgptsf.html

JS:   class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtjctlsxce.html

TS:   class Admin extends User {}
来源：http://hz.yongpay.top/gtwcxpkclu.html

Java: class Admin extends User {}
来源：http://hz.ybcxt.top/gtqnyrhmpk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.pycfn.com/gtblkijjod.html

Ruby: class Admin < User; end
来源：http://hz.zhongyouzk.top/gtzxlybguf.html

C#:   class Admin : User {}
来源：http://hz.sufxvd.cn/gtobkzlslt.html

[G06] 重写方法
来源：http://hz.pengpengdd.cyou/gtepfenfom.html

Py:   def greet(self): return "admin"
来源：http://hz.9152youxi.cn/gtcdxvgmpa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.smart0.xyz/gtngzfelyz.html

JS:   greet() { return "admin"; }
来源：http://hz.yuxming.cn/gtmqwhidmo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yj202588.top/gtvwjzzbnu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yuxming.cn/gtbchkhhia.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cucudq.cn/gtaqtpzreb.html

Ruby: def greet; "admin"; end
来源：http://hz.quarkkingdee.top/gtssssvzfo.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhiwuduotai.top/gtqefrppcf.html

[G07] 调用父类方法
来源：http://hz.jqgufenzy.top/gtrkvvsmrd.html

Py:   super().greet()
来源：http://hz.jinqigfzy.top/gttoeaoygy.html

PHP:  parent::greet();
来源：http://hz.gogol.net.cn/gtjnfzqwru.html

JS:   super.greet();
来源：http://hz.shzxlz.cn/gtqzgbqout.html

TS:   super.greet();
来源：http://hz.cqqwz.cn/gtnvupghph.html

Java: super.greet();
来源：http://hz.yuxming.cn/gtmsqlmsfz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.daxiang520.top/gtmqbpylhc.html

Ruby: super
来源：http://hz.kuanghao11.cn/gtlodgxoyh.html

C#:   base.Greet();
来源：http://hz.yongpay.top/gtdpgjknte.html

[G08] 静态方法与属性
来源：http://hz.hammf.cn/gtkxyzvsqr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jiagoushi.top/gtgdvhzcwb.html

PHP:  public static function f() {}
来源：http://hz.ivvv.top/gtbcelrcwh.html

JS:   static f() {}
来源：http://hz.yvedp.cn/gtlosajmxg.html

TS:   static f(): void {}
来源：http://hz.jinghuilouyu.cn/gtmkohonlk.html

Java: static void f() {}
来源：http://hz.zhoulong.xyz/gtqqalvrpy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.daria6918.cn/gtfyezwcdp.html

Ruby: def self.f; end
来源：http://hz.yangfankeji.com/gtthuziqor.html

C#:   public static void F() {}
来源：http://hz.birdmap.top/gtmhmgygjf.html

[G09] 接口 / 抽象类
来源：http://hz.daria6918.cn/gtypdkdyij.html


<!-- 参考信息 -->