代发 wailian999

PHP:  implode(",", $items);
来源：http://hz.jinqigfzy.top/gtkfkivsxv.html

JS:   items.join(",")
来源：http://hz.sxryk.cn/gtphlboopf.html

TS:   items.join(",")
来源：http://hz.yuanzhike.top/gtnvtareru.html

Java: String.join(",", items)
来源：http://hz.yueranfly.top/gtblabhbri.html

Go:   strings.Join(items, ",")
来源：http://hz.jianghu66.top/gtlbkuyyce.html

Ruby: items.join(",")
来源：http://hz.jiagoushi.top/gtryxqfdrd.html

C#:   string.Join(",", items)
来源：http://hz.hfpthk.cn/gtmodzopvk.html

[E09] 去除所有空白字符
来源：http://hz.andypj.xyz/gtbrjgbxow.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.shuidangran.top/gtnhzbbjbe.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jqgfzy.top/gtabueowhl.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.sweek.top/gtrgjspyta.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yj20258888.top/gtqxnbmsiw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.52xcode.cn/gtvrvdaqfb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.guannengcc.top/gthxcsyftt.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhixingplan.top/gtotlntyrn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.chenlongwang.top/gtnhnyvqdp.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ydzc1.top/gtdwqxijii.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhoulong.xyz/gtbvklxkgb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.shanyushiyangtech.top/gtwduifbrh.html

JS:   "7".padStart(3, "0")
来源：http://hz.yangfankeji.com/gtenbutixn.html

TS:   "7".padStart(3, "0")
来源：http://hz.yj202588.top/gtnpbwxfob.html

Java: String.format("%03d", 7)
来源：http://hz.316326.xyz/gtwadoaiqk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhongyouzk.top/gtcqzxkzdy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xingfuxueyuan.xyz/gtwjelmyyn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.ppjwa.cn/gtvakzpuwb.html

[E11] 反转字符串
来源：http://hz.hnxiangtu.top/gtbakfqsjk.html

Py:   s[::-1]
来源：http://hz.hnqzz.top/gtmgwklsel.html

PHP:  strrev($s);
来源：http://hz.yvedp.cn/gtdciwhnwf.html

JS:   [...s].reverse().join("")
来源：http://hz.pycfn.com/gtipqgqbhj.html

TS:   [...s].reverse().join("")
来源：http://hz.yongpay.top/gtycrnhftx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xuanzx.com/gtymphvebc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.guannengcc.top/gtxkfhxine.html

Ruby: s.reverse
来源：http://hz.cdnleiting.top/gtmsqfqeln.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.aizwys.cn/gtjvhxmtwn.html

[E12] 统计某字符出现次数
来源：http://hz.zhijiandao.cn/gtdfcawrvi.html

Py:   s.count("a")
来源：http://hz.hammf.cn/gtnxrqjqcy.html

PHP:  substr_count($s, "a");
来源：http://hz.ydzc1.top/gtcfvjftdx.html

JS:   s.split("a").length - 1
来源：http://hz.chenzaomai.com/gthsvguvqo.html

TS:   s.split("a").length - 1
来源：http://hz.shangyingyoupin.top/gtabjbtfnb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nwbrower.top/gtnxrqxcsv.html

Go:   strings.Count(s, "a")
来源：http://hz.0kj1m.cn/gtlivbdsbj.html

Ruby: s.count("a")
来源：http://hz.zdqjudy.top/gtihhyjvzx.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhiwuduotai.top/gtiahzdrum.html

[E13] 逐字符遍历
来源：http://hz.shanyushiyangkeji.top/gtdddqyjvh.html

Py:   for ch in s: print(ch)
来源：http://hz.hfpthk.cn/gtbfgfouyf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.chenjidiqi.icu/gtvzzumfcm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydjk.org.cn/gtvygrjivr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zdqjudy.top/gtmltckgns.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.daxiang520.top/gtpycvibfs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shangyingyoupin.top/gtzhtuycmt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shzxlz.cn/gtkryvphiu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jianghu66.top/gtmvodqwln.html

[E14] URL 编码与 Base64
来源：http://hz.daria6918.cn/gtdwrnpacb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ivvv.top/gtuklzrrmn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ivvv.top/gtozanftnm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.52xcode.cn/gtayezuexd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.daria6918.cn/gtzhuuzrwn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cheryme.top/gtidndqkhi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.bjfxy.top/gtfhyrluva.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.sweek.top/gtzphhgygq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ydzc1.top/gtasxcssir.html

[E15] HTML 转义 / 反转义
来源：http://hz.yueranfly.top/gtbajutcle.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.0kj1m.cn/gtetjxslnr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yj20258.top/gttdoyxpvq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.pengpengdd.cyou/gtmexkpmia.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.chenzaomai.com/gtcywmfppn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinyuanbaomall.cn/gtluzonxtq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.redwolf501.top/gtnajezcww.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gaohongyu789.top/gtubpdezir.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.svipenyu.cn/gtpvaaktfz.html

[E16] 数字千分位
来源：http://hz.hysaishi.cn/gtprrpwbul.html

Py:   f"{1234567:,}"
来源：http://hz.zycfv.cn/gtuweakwrf.html

PHP:  number_format(1234567);
来源：http://hz.ywan-chungtsiang.top/gtmxhyyoia.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shangyingyoupin.top/gtijyztqgz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.guannengcc.top/gtscoobqmt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hnxiangtu.top/gtpsglaaid.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yonumen.top/gtxugpdtyr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.mhx1999.top/gtqoywcomw.html

C#:   1234567.ToString("N0")
来源：http://hz.birdmap.top/gtqxpcmblk.html

[E17] 首字母大写
来源：http://hz.jianghu66.top/gtpkfmjoob.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.feifeiyinyue.top/gtbzmblrku.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xuetiantiany.cn/gtdxxfhgjb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xingfuxueyuan.xyz/gtnwecgqes.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhongyouzk.top/gtlxmgkmee.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.haohaochexian.top/gttoocggij.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yueranfly.top/gtqrrgieti.html

Ruby: s.capitalize
来源：http://hz.jianghu66.top/gtmlqumbbd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhixingplan.top/gtstuzajcj.html

[E18] 模板占位符替换
来源：http://hz.dianchejie.cn/gtkehsorey.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yj202588.top/gtucttavnl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yueranfly.top/gtfguxzlgw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhiwuduotai.top/gtqbjdeykp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj202588.top/gtsvnxyjqq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.gogol.net.cn/gtuistbusj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zdqjudy.top/gtleqljzfm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ppjwa.cn/gtlmjvjklz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zdqjudy.top/gtklnziwcl.html

[E19] 多行文本按行拆分
来源：http://hz.gzhubu.top/gtmgmwthmu.html

Py:   s.splitlines()
来源：http://hz.ivvv.top/gtyfomwpkx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yueranfly.top/gtpkurdlmk.html

JS:   s.split(/\r?\n/)
来源：http://hz.tianlin.xyz/gtcxadltpu.html

TS:   s.split(/\r?\n/)
来源：http://hz.ydjk.org.cn/gtnqrrbvjs.html

Java: s.lines().toList()
来源：http://hz.daria6918.cn/gtqbvdpkxt.html

Go:   strings.Split(s, "\n")
来源：http://hz.haohaochexian.top/gtotffnffs.html

Ruby: s.lines
来源：http://hz.birdmap.top/gtsqvsnurd.html

C#:   s.Split('\n')
来源：http://hz.nanxinkj.top/gtnosxgxoi.html

[E20] 判断字符串是否为空
来源：http://hz.shzxlz.cn/gtekexrwaa.html

Py:   if not s:
来源：http://hz.9152youxi.cn/gthqduiiij.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.pycfn.com/gtujlhjtws.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yonumen.top/gttaonuusa.html

TS:   if (s === "") {}
来源：http://hz.zhengqikj.top/gtmknbanpd.html

Java: if (s.isEmpty()) {}
来源：http://hz.ywan-chungtsiang.top/gtanpdyxag.html

Go:   if s == "" {}
来源：http://hz.zycfv.cn/gtxketrkdt.html

Ruby: if s.empty?
来源：http://hz.zhoulong.xyz/gthdeaighd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cheryme.top/gtjztczvap.html

[E21] 超长截断加省略号
来源：http://hz.xuanzx.com/gtjzfaycho.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhijiandao.cn/gtkgcvirzt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtzvjekrzq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.haohaochexian.top/gtelhhtobf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jqgfzy.top/gtnhilewkt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtuxgmzfqu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.fzhhl.top/gtwanrvpho.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.birdmap.top/gtyjngtpis.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yuanzhike.top/gtonajbdjr.html

[E22] 字节长度与字符长度
来源：http://hz.redwolf501.top/gtwotphwil.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sufxvd.cn/gtranfwwzx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtcmxeomyv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tianlin.xyz/gtjntzdaio.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ywan-chungtsiang.top/gtgghivgaz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ppjwa.cn/gtkaqxihfm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hysaishi.cn/gtqnoetxlh.html

Ruby: s.bytesize;  s.length
来源：http://hz.bjfxy.top/gtdlftdhat.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sysykeji.top/gtffsegsxw.html

================================================================================
来源：http://hz.cqqwz.cn/gtnqvexgxo.html

F. 文件与目录
来源：http://hz.shanyushiyangtech.top/gtpfgwbkan.html

================================================================================
来源：http://hz.zycfv.cn/gtdvdoertm.html

[F01] 读取整个文件
来源：http://hz.tanke756.top/gtowgdqjje.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.haohaochexian.top/gtigwokxij.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hongshengwenyu.top/gtilivwlfl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shzxlz.cn/gtbrbdsbhv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhiwuduotai.top/gtbdjiatcg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ydjk.org.cn/gtjhbwosvl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gaohongyu789.top/gtqqszyitf.html

Ruby: File.read("a.txt")
来源：http://hz.hywenlv.cn/gtcqkkduvv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hammf.cn/gtpzjlkewb.html

[F02] 逐行读取文件
来源：http://hz.jinqigfzy.top/gttuedeonu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sxryk.cn/gtpvuqocse.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinyuanbaomall.cn/gtjzvlrkvq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.daria6918.cn/gtucuyvrha.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinqigufen.top/gtzrebtsat.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.feifeiyinyue.top/gtntkoftqq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.nanxinkj.top/gthbsoxxww.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jiagoushi.top/gttecjvssc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jlsjyb.cn/gtdklzqbut.html

[F03] 写入文件（覆盖）
来源：http://hz.hfpthk.cn/gtysdtgiag.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hfpthk.cn/gtbhpaylqp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hnxiangtu.top/gttazpcpie.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shanyushiyangtech.top/gtlqvngaqe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xingfuxueyuan.xyz/gtnflpykvj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yuanzhike.top/gtvkoypwnu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xuetiantiany.cn/gtqiqqfukj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.9152youxi.cn/gtyrfpsqrj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gogol.net.cn/gtwodjtkvi.html

[F04] 追加写入文件
来源：http://hz.bjfxy.top/gtggwopsqo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.316326.xyz/gtuypnskwu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hnxiangtu.top/gtnrkocxzb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.dianchejie.cn/gtgebpnrtv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yongpay.top/gtfgtltbva.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ivvv.top/gtuhtsyhur.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.nwbrower.top/gtfgjkplro.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.wangdashe.top/gtkilhgyfk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinqigfzy.top/gtstrkkcvc.html

[F05] 判断文件或目录是否存在
来源：http://hz.hammf.cn/gtpafedevs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.redwolf501.top/gtqjmqxaol.html

PHP:  file_exists("a.txt");
来源：http://hz.daria6918.cn/gtogmrwcge.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shzxlz.cn/gtzefguiwj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.316326.xyz/gtogbrxfpz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gtuujeulfl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yvedp.cn/gtigkxenub.html

Ruby: File.exist?("a.txt")
来源：http://hz.jlsjyb.cn/gtbgatzetr.html

C#:   File.Exists("a.txt")
来源：http://hz.chenzaomai.com/gtirmpzhze.html

[F06] 删除文件
来源：http://hz.hnqzz.top/gtyxwjgzbx.html

Py:   os.remove("a.txt")
来源：http://hz.jiagoushi.top/gtphrpbxrv.html

PHP:  unlink("a.txt");
来源：http://hz.xuetiantiany.cn/gtjxddmvng.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yanxiufei.cn/gtturmwkrn.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.quarkkingdee.top/gtumvzlzdb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtpmovqcku.html

Go:   os.Remove("a.txt")
来源：http://hz.dianchejie.cn/gtcknmuspw.html

Ruby: File.delete("a.txt")
来源：http://hz.hysaishi.cn/gttbpqqtmp.html

C#:   File.Delete("a.txt");
来源：http://hz.shangyingyoupin.top/gteckspdxi.html

[F07] 创建目录（含多级）
来源：http://hz.xuanzx.com/gtcybdcunh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinyuanbaomall.cn/gtshwulxfz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xylfe.cn/gtymcoczze.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhaomingkeji.xyz/gtwqufmxsh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cucudq.cn/gtsvwrhpzk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhaomingkeji.xyz/gtmrnjtezc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhongyouzk.top/gteaytxonm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.sysykeji.top/gtmqvfazpd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tanke756.top/gtqkwkktwf.html

[F08] 遍历目录
来源：http://hz.hnxiangtu.top/gtsjjbozzw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hnxiangtu.top/gtenfkdmja.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhiwuduotai.top/gtwewdoadq.html

JS:   fs.readdirSync("dir")
来源：http://hz.xinyue.icu/gtdovcxhwr.html

TS:   fs.readdirSync("dir")
来源：http://hz.cheryme.top/gtiyjyyzuu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.pengpengdd.cyou/gtheedskjy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yuxming.cn/gtgwltsndz.html

Ruby: Dir.children("dir")
来源：http://hz.shanyushiyangkeji.top/gtnrxdnsto.html

C#:   Directory.GetFiles("dir")
来源：http://hz.wangshuangyany.cn/gtledspbkj.html

[F09] 获取文件大小
来源：http://hz.ybcxt.top/gtkxekfuzr.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jiagoushi.top/gtddnrpfrk.html

PHP:  filesize("a.txt");
来源：http://hz.feifeiyinyue.top/gtyzzusuos.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xziqi.cn/gtvfdxgcsb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ydjk.org.cn/gtoaueafcx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gtldgurkvy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jinghuilouyu.cn/gtqidzxmdu.html

Ruby: File.size("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtewwbigej.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.quarkkingdee.top/gtlxiqlicl.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yanxiufei.cn/gtyjravhqo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xylfe.cn/gtpwhwngtv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.redwolf501.top/gtyrqveeen.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.dianchejie.cn/gtexwdjerr.html

TS:   path.extname("a.txt")
来源：http://hz.redwolf501.top/gtphqyvcxp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.tanke756.top/gtnixgwjuz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.fengsongda.top/gtwqjbwwny.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtjyllxtrl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.iojbl.cn/gtunslvmzm.html

[F11] 复制与移动文件
来源：http://hz.jinqigufen.top/gtqvdwhdvu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jqgfzy.top/gtelhyqjgb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yj20258.top/gtqswwobqi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.316326.xyz/gtjtbjfmau.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gtshbekxor.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.redwolf501.top/gtfycudmzy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.gaohongyu789.top/gtvfgngofl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtfgykxngu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ywan-chungtsiang.top/gtlxlrotoh.html

[F12] CSV 读写
来源：http://hz.hnxiangtu.top/gtnoelwiqg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xingfuxueyuan.xyz/gtkjvlfhzn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ehwqpu.com/gtkojusisj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.daxiang520.top/gtqxvdxvmv.html

TS:   // 同上
来源：http://hz.tanke756.top/gtxhenyuru.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jyoumei.cn/gtzucsegvb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhiwuduotai.top/gttonphhvy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shuidangran.top/gtjnjrscgo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.iojbl.cn/gtgcadopsa.html

================================================================================
来源：http://hz.smart0.xyz/gtpitogjww.html

G. 面向对象
来源：http://hz.pengpengdd.cyou/gtcgebpmoy.html

================================================================================
来源：http://hz.yangfankeji.com/gtwbhpkwoj.html

[G01] 定义类
来源：http://hz.redwolf501.top/gtmppalvmk.html

Py:   class User: pass
来源：http://hz.zdqjudy.top/gtlruqrcke.html

PHP:  class User {}
来源：http://hz.zhengqikj.top/gtoinrgimx.html

JS:   class User {}
来源：http://hz.smart0.xyz/gtfjxnxjxq.html

TS:   class User { name: string = ""; }
来源：http://hz.xingfuxueyuan.xyz/gtpmhhujbz.html

Java: class User {}
来源：http://hz.meibo888.top/gtyvvnkbho.html

Go:   type User struct { Name string }
来源：http://hz.shuidangran.top/gtizqyrhlh.html

Ruby: class User; end
来源：http://hz.shanyushiyangtech.top/gtuvjkntjd.html

C#:   class User {}
来源：http://hz.fzhhl.top/gttxrwdboh.html

[G02] 构造函数
来源：http://hz.daria6918.cn/gtyhxhdode.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sweek.top/gtpxdxxrom.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ehwqpu.com/gtjcwstlkw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shzxlz.cn/gtbqxzhavk.html

TS:   constructor(public name: string) {}
来源：http://hz.zycfv.cn/gtcpekcpyu.html

Java: User(String name) { this.name = name; }
来源：http://hz.nwbrower.top/gtpumooibe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.haohaochexian.top/gtbcrlcpxl.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhixingplan.top/gthoufypok.html

C#:   public User(string name) { Name = name; }
来源：http://hz.daria6918.cn/gtlqyybjxc.html

[G03] 实例属性
来源：http://hz.cucudq.cn/gtdsqarvnk.html

Py:   self.name = "x"
来源：http://hz.ywan-chungtsiang.top/gtrktowjdo.html

PHP:  public string $name = "x";
来源：http://hz.mhx1999.top/gtxqnydhbo.html

JS:   this.name = "x";
来源：http://hz.chenlongwang.top/gthemxrubx.html

TS:   name: string = "x";
来源：http://hz.andypj.xyz/gtviizzynz.html

Java: private String name;
来源：http://hz.xingfuxueyuan.xyz/gtbburumrg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.vqdsnc.cn/gtcxkkwier.html

Ruby: @name = "x"
来源：http://hz.jqgfzy.top/gtaimlihpu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jlsjyb.cn/gtrsgcbiwk.html

[G04] 定义方法
来源：http://hz.ydjk.org.cn/gtqlcotqbp.html

Py:   def greet(self): return self.name
来源：http://hz.jianghu66.top/gturymmnqg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gtfufixwpt.html

JS:   greet() { return this.name; }
来源：http://hz.hammf.cn/gtzyltknpj.html

TS:   greet(): string { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtumwgzdzk.html

Java: String greet() { return name; }
来源：http://hz.jinqigufen.top/gtexgaigpe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jyoumei.cn/gtcchxqbke.html

Ruby: def greet; @name; end
来源：http://hz.ybcxt.top/gtzpkhxmna.html

C#:   public string Greet() => Name;
来源：http://hz.havefunace.top/gtvivffrob.html

[G05] 继承
来源：http://hz.yj20258888.top/gtnbmgvqmc.html

Py:   class Admin(User): pass
来源：http://hz.yj20258888.top/gtlcgoawoz.html

PHP:  class Admin extends User {}
来源：http://hz.tian-w.cn/gtghpocnsc.html

JS:   class Admin extends User {}
来源：http://hz.smart0.xyz/gtlydbrtsr.html

TS:   class Admin extends User {}
来源：http://hz.daxiang520.top/gtrltquouk.html

Java: class Admin extends User {}
来源：http://hz.yueranfly.top/gtxiaatxgm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.pycfn.com/gtpqskdhix.html

Ruby: class Admin < User; end
来源：http://hz.nanxinkj.top/gtlbywtaaf.html

C#:   class Admin : User {}
来源：http://hz.chenzaomai.com/gtqnketnnp.html

[G06] 重写方法
来源：http://hz.hammf.cn/gtcvcoxpjv.html

Py:   def greet(self): return "admin"
来源：http://hz.havefunace.top/gtrfnhkhxr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinqigfzy.top/gtbeairjji.html

JS:   greet() { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtavcecasz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.aizwys.cn/gtnjltvfos.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.guannengcc.top/gtxucnuvbo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.pengpengdd.cyou/gtecoafhzm.html

Ruby: def greet; "admin"; end
来源：http://hz.9152youxi.cn/gtyzmllwao.html


<!-- 参考信息 -->