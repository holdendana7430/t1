代发 wailian999

[E02] 重复字符串
来源：http://hz.wangshuangyany.cn/gtotawshrn.html

Py:   "ab" * 3
来源：http://hz.xuanzx.com/gtpaagmaoj.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jyoumei.cn/gtlgmpngqb.html

JS:   "ab".repeat(3)
来源：http://hz.shanyushiyangkeji.top/gtbqscbpsl.html

TS:   "ab".repeat(3)
来源：http://hz.hywenlv.cn/gtwfhpwtny.html

Java: "ab".repeat(3)
来源：http://hz.nanxinkj.top/gtilkhismc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.wangdashe.top/gtmmrvrgdq.html

Ruby: "ab" * 3
来源：http://hz.feifeiyinyue.top/gtlutzowww.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.fengsongda.top/gtunudaafh.html

[E03] 截取子串
来源：http://hz.meibo888.top/gtyefuagix.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sufxvd.cn/gtjjrqkbvh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.vqdsnc.cn/gtzrswjgod.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.9152youxi.cn/gtdlucidhv.html

TS:   s.slice(1, 4)
来源：http://hz.guannengcc.top/gtpellkzbb.html

Java: s.substring(1, 4)
来源：http://hz.xingfuxueyuan.xyz/gtqkduxbgj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.haohaochexian.top/gtoxcftewo.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.guannengcc.top/gtefylaakv.html

C#:   s.Substring(1, 3)
来源：http://hz.xuanzx.com/gtkgsdbrkq.html

[E04] 查找子串位置
来源：http://hz.cqqwz.cn/gtovuvreps.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cheryme.top/gtblbdbmpv.html

PHP:  strpos($s, "x");
来源：http://hz.havefunace.top/gtgvmertng.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jinghuilouyu.cn/gtmcpenrgn.html

TS:   s.indexOf("x")
来源：http://hz.ivvv.top/gtkkhhwpjv.html

Java: s.indexOf("x")
来源：http://hz.xinyue.icu/gtixbuogar.html

Go:   strings.Index(s, "x")
来源：http://hz.sweek.top/gtjuhqhuqh.html

Ruby: s.index("x")
来源：http://hz.snrcjt.cn/gtyucugpbg.html

C#:   s.IndexOf("x")
来源：http://hz.pengpengdd.cyou/gtitkjzgcc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ywan-chungtsiang.top/gtmkxzjwor.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.nanxuanxn.top/gtojylojdf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.c1oappe.top/gtrzbmvaze.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.kuanghao11.cn/gtszwdozak.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zdqjudy.top/gtbrfoqvwg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.pycfn.com/gtibykxmmk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.nanxinkj.top/gtjczjiycy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.meibo888.top/gtldqeudvv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ivvv.top/gtykyhofve.html

[E06] 替换子串
来源：http://hz.chenjidiqi.icu/gtujmjcngm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.svipenyu.cn/gtcalmrhru.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.cqqwz.cn/gtvfhpwqax.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sxryk.cn/gtrfwlgacu.html

TS:   s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtokqkldze.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jianghu66.top/gtsnhmdqky.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ybcxt.top/gtumkkfxqn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hammf.cn/gtkzfwnuic.html

C#:   s.Replace("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtbnpwtpqj.html

[E07] 按分隔符拆分
来源：http://hz.gogol.net.cn/gtcqlbjclx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.quarkkingdee.top/gtyjljdnfw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jiagoushi.top/gtgubkpwce.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jqgfzy.top/gttnfmdyzk.html

TS:   s.split(",")
来源：http://hz.smart0.xyz/gtolittqvv.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.aibaodan.cn/gtwbkpwngi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ivvv.top/gtxgrgckcv.html

Ruby: s.split(",");  s.split
来源：http://hz.hywenlv.cn/gttzwxqarl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cdnleiting.top/gtwyiqdfxa.html

[E08] 数组按分隔符合并
来源：http://hz.nanxuanxn.top/gtdgekzxwp.html

Py:   ",".join(items)
来源：http://hz.ppjwa.cn/gtnxqeufiz.html

PHP:  implode(",", $items);
来源：http://hz.yj20258.top/gtgelgdfpr.html

JS:   items.join(",")
来源：http://hz.nwbrower.top/gtjsyccvge.html

TS:   items.join(",")
来源：http://hz.hnqzz.top/gtqstrmltf.html

Java: String.join(",", items)
来源：http://hz.chenzaomai.com/gtnmgpykvl.html

Go:   strings.Join(items, ",")
来源：http://hz.yuanzhike.top/gtdvizgqwe.html

Ruby: items.join(",")
来源：http://hz.sufxvd.cn/gttzyoyckt.html

C#:   string.Join(",", items)
来源：http://hz.tianlin.xyz/gtyansasxw.html

[E09] 去除所有空白字符
来源：http://hz.jinyuanbaomall.cn/gthptjujew.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yanxiufei.cn/gtgicwtbzo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.gzhubu.top/gtbhqlhwty.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenlongwang.top/gtvptufgnb.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.snrcjt.cn/gtfyogbpqd.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yuxming.cn/gtjtjokeqm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yonumen.top/gttmizangb.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shanyushiyangtech.top/gtxlxvuwta.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.fengsongda.top/gtwplkqxew.html

[E10] 左侧补零 / 定长填充
来源：http://hz.tanke756.top/gtiprdomfd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.daxiang520.top/gtgmqivssw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ydjk.org.cn/gtipdqnpkv.html

JS:   "7".padStart(3, "0")
来源：http://hz.redwolf501.top/gtdbpkyozn.html

TS:   "7".padStart(3, "0")
来源：http://hz.jyoumei.cn/gtbfyemtfx.html

Java: String.format("%03d", 7)
来源：http://hz.pengpengdd.cyou/gtgdmcyqko.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cashguo.top/gthcbghnxg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.smart0.xyz/gttopllyfl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.nanxinkj.top/gtsnayrkuz.html

[E11] 反转字符串
来源：http://hz.birdmap.top/gtsmrhkrcg.html

Py:   s[::-1]
来源：http://hz.hongshengwenyu.top/gtdvnqprcl.html

PHP:  strrev($s);
来源：http://hz.jlsjyb.cn/gtgvwloutu.html

JS:   [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtnmnzofvt.html

TS:   [...s].reverse().join("")
来源：http://hz.guowangkeji.top/gtaldyuoct.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.fzhhl.top/gtxktdntih.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sweek.top/gtfoggmcit.html

Ruby: s.reverse
来源：http://hz.zhijiandao.cn/gtwborfmdo.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jinqigfzy.top/gtxvijamzg.html

[E12] 统计某字符出现次数
来源：http://hz.zhengqikj.top/gtcdyofcua.html

Py:   s.count("a")
来源：http://hz.aibaodan.cn/gttdpiqthj.html

PHP:  substr_count($s, "a");
来源：http://hz.yonumen.top/gthpqvgadb.html

JS:   s.split("a").length - 1
来源：http://hz.cashguo.top/gtgfsfnbnw.html

TS:   s.split("a").length - 1
来源：http://hz.gogol.net.cn/gtayfapjnu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.wangshuangyany.cn/gtlgetdjyx.html

Go:   strings.Count(s, "a")
来源：http://hz.jlsjyb.cn/gthzfesbya.html

Ruby: s.count("a")
来源：http://hz.mhx1999.top/gtvsavotnl.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sufxvd.cn/gtwoglfufq.html

[E13] 逐字符遍历
来源：http://hz.zhoulong.xyz/gtneprutkm.html

Py:   for ch in s: print(ch)
来源：http://hz.gogol.net.cn/gtjybezzlb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yonumen.top/gtfpmfskos.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sxryk.cn/gtzlwjfrcu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sysykeji.top/gtrxjgiury.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhoulong.xyz/gtfucrjiyw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.feifeiyinyue.top/gtdfvqgnvt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jinqigfzy.top/gtadjdqaoe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhijiandao.cn/gtfeqliugi.html

[E14] URL 编码与 Base64
来源：http://hz.kuanghao11.cn/gtcphikxwz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.52xcode.cn/gtyyrvedws.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.chenjidiqi.icu/gtsbfsfuok.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.snrcjt.cn/gtrjzombzn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhaomingkeji.xyz/gthnibplpg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yuanzhike.top/gtbpmphswd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jyoumei.cn/gtniyvyubv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.kuanghao11.cn/gtzhkbisjc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhengqikj.top/gtifdbdrmu.html

[E15] HTML 转义 / 反转义
来源：http://hz.tian-w.cn/gteliyrjdq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.guannengcc.top/gtksksqvox.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yangfankeji.com/gttpbhkitb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.iojbl.cn/gtkxxgmizg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yj20258888.top/gtvecywers.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhaomingkeji.xyz/gtgwpjqbss.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.nanxuanxn.top/gtupbwjjjw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yuxming.cn/gtlodhncuw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shanyushiyangkeji.top/gtfkzndgqh.html

[E16] 数字千分位
来源：http://hz.nanxinkj.top/gtxymqffll.html

Py:   f"{1234567:,}"
来源：http://hz.dianchejie.cn/gtgdxuakpk.html

PHP:  number_format(1234567);
来源：http://hz.quarkkingdee.top/gtxmdgpjbm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.smart0.xyz/gtihvzzorz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jiagoushi.top/gthpliuiln.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinyuanbaomall.cn/gtusoezvwt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.svipenyu.cn/gtwqacyaaa.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ppjwa.cn/gtitlducvz.html

C#:   1234567.ToString("N0")
来源：http://hz.hammf.cn/gtjvdxlgvw.html

[E17] 首字母大写
来源：http://hz.guowangkeji.top/gtogrijyln.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shanyushiyangkeji.top/gtzlehexjb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.daxiang520.top/gtkgivxfva.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.daxiang520.top/gtxutbubgq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinyuanbaomall.cn/gtleqvgnzb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.redwolf501.top/gtrgmhqwwt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jqgfzy.top/gtgwigntoi.html

Ruby: s.capitalize
来源：http://hz.quarkkingdee.top/gtwvmpfzoe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhongyouzk.top/gtejnexaqc.html

[E18] 模板占位符替换
来源：http://hz.jinyuanbaomall.cn/gtkqsedbhy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.svipenyu.cn/gtzudsrkkp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.316326.xyz/gtfxvqfrzb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ehwqpu.com/gtsncbyfan.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenlongwang.top/gtvrygtrrj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hywenlv.cn/gtrhaalqss.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.9152youxi.cn/gtqhgzlahe.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.gotoacloud.top/gtdqzxyvot.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cheryme.top/gtolfduyxv.html

[E19] 多行文本按行拆分
来源：http://hz.ywan-chungtsiang.top/gtqwuffltx.html

Py:   s.splitlines()
来源：http://hz.jianghu66.top/gtkxtsjuys.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yangfankeji.com/gtrcyugsts.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhongyouzk.top/gtzdufyvto.html

TS:   s.split(/\r?\n/)
来源：http://hz.zycfv.cn/gtqjkeowsq.html

Java: s.lines().toList()
来源：http://hz.yueranfly.top/gtegmrbslr.html

Go:   strings.Split(s, "\n")
来源：http://hz.xylfe.cn/gtqzcfzolx.html

Ruby: s.lines
来源：http://hz.jiagoushi.top/gtgeojajaa.html

C#:   s.Split('\n')
来源：http://hz.meibo888.top/gtdvzponzs.html

[E20] 判断字符串是否为空
来源：http://hz.gzhubu.top/gtpbegdaeh.html

Py:   if not s:
来源：http://hz.zhixingplan.top/gtfkgfthcc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.daria6918.cn/gtjntnyjkf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.aizwys.cn/gtmxbjmkaz.html

TS:   if (s === "") {}
来源：http://hz.guannengcc.top/gtidripxvq.html

Java: if (s.isEmpty()) {}
来源：http://hz.yuanzhike.top/gtqcufylvu.html

Go:   if s == "" {}
来源：http://hz.jinyuanbaomall.cn/gtmpzgqrjj.html

Ruby: if s.empty?
来源：http://hz.tian-w.cn/gtpusbmlxp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.iojbl.cn/gtvybzerdb.html

[E21] 超长截断加省略号
来源：http://hz.cdnleiting.top/gtujwftgty.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shanyushiyangtech.top/gtxdijfrlg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.gzhubu.top/gtrwkcskjb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hnxiangtu.top/gtkffegqjl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sysykeji.top/gturndfpxg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.havefunace.top/gtmuvymupv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cdnleiting.top/gteivgpkzh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.birdmap.top/gtcyfxrdjm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.quarkkingdee.top/gtxhflkqdo.html

[E22] 字节长度与字符长度
来源：http://hz.svipenyu.cn/gtvjvbfmuz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xziqi.cn/gtcyqeljrl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtdimgfxyy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cqqwz.cn/gtrelhklhv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sysykeji.top/gtpibqcbkd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ehwqpu.com/gtmgruvyhz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.sysykeji.top/gtqjzrtfer.html

Ruby: s.bytesize;  s.length
来源：http://hz.wangdashe.top/gtvrfidizo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.9152youxi.cn/gtmivgeiju.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtpfjtmcye.html

F. 文件与目录
来源：http://hz.sysykeji.top/gtyheyvxwm.html

================================================================================
来源：http://hz.cdnleiting.top/gtetmmxvdw.html

[F01] 读取整个文件
来源：http://hz.daria6918.cn/gtpqxtgefi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.fengsongda.top/gtcnxyyyox.html

PHP:  file_get_contents("a.txt");
来源：http://hz.aizwys.cn/gtjlbqdpzc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yj20258888.top/gtrynnhlfj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hnxiangtu.top/gtxmfhzwny.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gtuoeupskh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cashguo.top/gtwigoppjn.html

Ruby: File.read("a.txt")
来源：http://hz.fengsongda.top/gtnbhurpdd.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yuxming.cn/gtieblroyz.html

[F02] 逐行读取文件
来源：http://hz.xziqi.cn/gtnsajzmre.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xuetiantiany.cn/gtjbcdicqf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jianghu66.top/gtmpnimwqz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gaohongyu789.top/gtxtlscuwp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.c1oappe.top/gtlazvuuck.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhiwuduotai.top/gtxvfplxiw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.feifeiyinyue.top/gtovdipjbb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ivvv.top/gtoelesyqd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shanyushiyangtech.top/gtzfygaszr.html

[F03] 写入文件（覆盖）
来源：http://hz.andypj.xyz/gtoimfgzgy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ppjwa.cn/gtgfjlgtvn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cheryme.top/gtqqzcjskp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.pengpengdd.cyou/gtqbqlypoa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.iojbl.cn/gtvsiwwnkl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shanyushiyangkeji.top/gtwtwmprhw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yj20258888.top/gtmzccihsw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhoulong.xyz/gtlaccsoyf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yj20258888.top/gtkgjdglyi.html

[F04] 追加写入文件
来源：http://hz.yanxiufei.cn/gtdrrbacjv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.guannengcc.top/gtxoofbgcb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tanke756.top/gtrtskynto.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.snrcjt.cn/gtxfksvdbj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aibaodan.cn/gtwrkrjrxo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.redwolf501.top/gtabeatoxa.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jinqigfzy.top/gtezocmnbf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jqgfzy.top/gtjqvrzijx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.redwolf501.top/gtskykrinj.html

[F05] 判断文件或目录是否存在
来源：http://hz.9152youxi.cn/gtniqmusom.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shangyingyoupin.top/gtmvhglufm.html

PHP:  file_exists("a.txt");
来源：http://hz.birdmap.top/gtmbkdomfh.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtfzggvxjd.html

TS:   fs.existsSync("a.txt")
来源：http://hz.guannengcc.top/gtrmhyhdwz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtlcjljwti.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhaomingkeji.xyz/gtzyqewgxz.html

Ruby: File.exist?("a.txt")
来源：http://hz.yvedp.cn/gtgdmqbahy.html

C#:   File.Exists("a.txt")
来源：http://hz.jqgfzy.top/gtewbpkiyw.html

[F06] 删除文件
来源：http://hz.birdmap.top/gtkwxnkroh.html

Py:   os.remove("a.txt")
来源：http://hz.chenjidiqi.icu/gtdxibxtke.html

PHP:  unlink("a.txt");
来源：http://hz.xinyue.icu/gtrvbxytue.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.pycfn.com/gtleqbxxdx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.pycfn.com/gtwvtrmjyh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtiefoqknc.html

Go:   os.Remove("a.txt")
来源：http://hz.feifeiyinyue.top/gtkumcemrp.html

Ruby: File.delete("a.txt")
来源：http://hz.sxryk.cn/gtipzyyqyp.html

C#:   File.Delete("a.txt");
来源：http://hz.sufxvd.cn/gtzltukaxw.html

[F07] 创建目录（含多级）
来源：http://hz.feifeiyinyue.top/gtxgncrlja.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.iojbl.cn/gtpoqsogza.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jianghu66.top/gtqbsacsqc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.meibo888.top/gtghiekphv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zycfv.cn/gtmbviylip.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhixingplan.top/gtellddqty.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhengqikj.top/gtsfyrtlze.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.sxryk.cn/gtprgltsox.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zdqjudy.top/gtlyyaqwkq.html

[F08] 遍历目录
来源：http://hz.yueranfly.top/gtofksxeyq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hnxiangtu.top/gtpnohgiwi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cashguo.top/gtnozxuvrx.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhijiandao.cn/gtikciilvz.html

TS:   fs.readdirSync("dir")
来源：http://hz.yj20258888.top/gthtqlmgvi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jinqigfzy.top/gtrdvhftqu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cheryme.top/gtswdfgycg.html

Ruby: Dir.children("dir")
来源：http://hz.kuanghao11.cn/gtkfvybppl.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nanxuanxn.top/gthhicfrtp.html

[F09] 获取文件大小
来源：http://hz.aibaodan.cn/gthbexkmys.html

Py:   os.path.getsize("a.txt")
来源：http://hz.havefunace.top/gthproaxmm.html

PHP:  filesize("a.txt");
来源：http://hz.sufxvd.cn/gtcfjxvijf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yonumen.top/gtjmezpmtn.html

TS:   fs.statSync("a.txt").size
来源：http://hz.wangdashe.top/gtfatcrflw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jlsjyb.cn/gtdyqvldoy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yj20258888.top/gtgnylrkxy.html

Ruby: File.size("a.txt")
来源：http://hz.dashuyun.cn/gttqepummi.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shanyushiyangkeji.top/gtmnkltefh.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hysaishi.cn/gtthhmtmel.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hysaishi.cn/gtfuzspjiu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jlsjyb.cn/gtoqjpqinf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtkrpdeemp.html

TS:   path.extname("a.txt")
来源：http://hz.zhijiandao.cn/gtocsiznms.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.aibaodan.cn/gtmqtkdaav.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.fengsongda.top/gtutqapaip.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cdnleiting.top/gtrurehqep.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtpfqlzoib.html

[F11] 复制与移动文件
来源：http://hz.aibaodan.cn/gtmilmpsah.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtgmspjuvx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jianghu66.top/gtohvlsqiz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtukfvofcu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtaphvnxwq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.meibo888.top/gtjjlbugyg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xylfe.cn/gtxbbgglla.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtlggvurhw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.dianchejie.cn/gtevxboifs.html

[F12] CSV 读写
来源：http://hz.shzxlz.cn/gtkkwnngml.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.iojbl.cn/gtdrugiluo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zycfv.cn/gtzpvwbube.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yvedp.cn/gtbjvahtcb.html

TS:   // 同上
来源：http://hz.wangdashe.top/gtrqbctkir.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.mhx1999.top/gtllafbfpx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.snrcjt.cn/gtlpbpedqi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.cheryme.top/gtoldgslcd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.svipenyu.cn/gthlycasoi.html


<!-- 参考信息 -->