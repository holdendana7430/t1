代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xylfe.cn/gtjldyskpx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xylfe.cn/gtilagarot.html

Go:   // 手写循环
来源：http://hz.yvedp.cn/gtbdidmrfv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cheryme.top/gttejmhtub.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhijiandao.cn/gtwhlxnzmk.html

[D24] 字典 / Map 基本操作
来源：http://hz.gotoacloud.top/gtrkpqtkqd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.gogol.net.cn/gtotiwrjvm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hywenlv.cn/gtohhkrtqg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.snrcjt.cn/gtworkbpot.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.snrcjt.cn/gtvjxkmzeg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yongpay.top/gttcavpzjs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hongshengwenyu.top/gtwqvzozji.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ydjk.org.cn/gtpxoyngka.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.tian-w.cn/gtfioghdfu.html

[D25] Set 集合去重与交并差
来源：http://hz.guowangkeji.top/gthtzhjijd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.sxryk.cn/gtegtzwdfd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yj20258.top/gtnycskrqn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yangfankeji.com/gtfxtcjmdq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yangfankeji.com/gtsrgpmtnp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jianghu66.top/gtgwpgsole.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hysaishi.cn/gtjolmerwh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.daxiang520.top/gtulsilzzi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.aibaodan.cn/gtfnbmyjvb.html

[D26] 数组转字符串
来源：http://hz.tanke756.top/gtldvbyjnp.html

Py:   ", ".join(map(str, arr))
来源：http://hz.tian-w.cn/gtoegxzoky.html

PHP:  implode(", ", $arr);
来源：http://hz.shuidangran.top/gtklieyvci.html

JS:   arr.join(", ")
来源：http://hz.tanke756.top/gtiorotgfc.html

TS:   arr.join(", ")
来源：http://hz.tian-w.cn/gtigmkxfws.html

Java: String.join(", ", list)
来源：http://hz.yuxming.cn/gtocacdowc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ywan-chungtsiang.top/gtfmddgpyk.html

Ruby: arr.join(", ")
来源：http://hz.jinqigfzy.top/gtngnatdhn.html

C#:   string.Join(", ", list)
来源：http://hz.0kj1m.cn/gtbovtyofy.html

================================================================================
来源：http://hz.haohaochexian.top/gtaqncraxf.html

E. 字符串处理
来源：http://hz.cashguo.top/gtkrevejxw.html

================================================================================
来源：http://hz.yuxming.cn/gtbwzlevuz.html

[E01] 拼接字符串
来源：http://hz.nanxuanxn.top/gtoiiabwxn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinghuilouyu.cn/gtcmeqwsnb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yj202588.top/gttzhnthjb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hywenlv.cn/gtefaybqhl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhongyouzk.top/gtsshemrdx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.fzhhl.top/gtxyxltpzh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yonumen.top/gtluaplygy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jinqigufen.top/gtoyktceax.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.iojbl.cn/gtticchnam.html

[E02] 重复字符串
来源：http://hz.shzxlz.cn/gtbejspgep.html

Py:   "ab" * 3
来源：http://hz.wangshuangyany.cn/gtlqztslfh.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yuanzhike.top/gtjrngiair.html

JS:   "ab".repeat(3)
来源：http://hz.xinyue.icu/gtxmbgupys.html

TS:   "ab".repeat(3)
来源：http://hz.ppjwa.cn/gtudcttcjp.html

Java: "ab".repeat(3)
来源：http://hz.hnqzz.top/gtgpiovnsw.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yj20258.top/gtfjhxpxdh.html

Ruby: "ab" * 3
来源：http://hz.ppjwa.cn/gtyrtlqybq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yanxiufei.cn/gtuhsrozch.html

[E03] 截取子串
来源：http://hz.ybcxt.top/gtnbiebvdp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yuxming.cn/gtslrenxvu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cucudq.cn/gtbvcphzqk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hammf.cn/gtthmuunfm.html

TS:   s.slice(1, 4)
来源：http://hz.gogol.net.cn/gtmfgwqbtu.html

Java: s.substring(1, 4)
来源：http://hz.hfpthk.cn/gtkpdouhmu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.pengpengdd.cyou/gtjtdsstik.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ehwqpu.com/gtsptxclqr.html

C#:   s.Substring(1, 3)
来源：http://hz.daria6918.cn/gtwzrkogeu.html

[E04] 查找子串位置
来源：http://hz.sweek.top/gtimrzbdtj.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cqqwz.cn/gtwtcdoynt.html

PHP:  strpos($s, "x");
来源：http://hz.shanyushiyangkeji.top/gthlixbqcc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ydjk.org.cn/gtinogznpi.html

TS:   s.indexOf("x")
来源：http://hz.hammf.cn/gtqqiyrzuy.html

Java: s.indexOf("x")
来源：http://hz.jinghuilouyu.cn/gtcjouakan.html

Go:   strings.Index(s, "x")
来源：http://hz.yj20258.top/gtonfzydri.html

Ruby: s.index("x")
来源：http://hz.zdqjudy.top/gtwbbjktco.html

C#:   s.IndexOf("x")
来源：http://hz.shanyushiyangkeji.top/gtjbusfzpm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.mhx1999.top/gtkfbykyzf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shanyushiyangtech.top/gthwdgxdrr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.andypj.xyz/gtxbqahxys.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.andypj.xyz/gtqbpbqovj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhiwuduotai.top/gtbvtqefzk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhaomingkeji.xyz/gtczlpvpdv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hywenlv.cn/gtouarcovx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gotoacloud.top/gtlbaowfjw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jinghuilouyu.cn/gtabokvjqe.html

[E06] 替换子串
来源：http://hz.aizwys.cn/gtnjilfzgh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.9152youxi.cn/gtbvbyugrn.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.aizwys.cn/gthodihqni.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.c1oappe.top/gtcszljdrr.html

TS:   s.replaceAll("a", "b")
来源：http://hz.chenjidiqi.icu/gtogybjcfm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.daria6918.cn/gtylyttxis.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.haohaochexian.top/gtctsrowhe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xylfe.cn/gtxjswphxc.html

C#:   s.Replace("a", "b")
来源：http://hz.c1oappe.top/gtzzfdxwjw.html

[E07] 按分隔符拆分
来源：http://hz.yuxming.cn/gtaaiyeybx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.wangshuangyany.cn/gtjpaqzvkf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.smart0.xyz/gtgrgiwtyf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.52xcode.cn/gtrolkvgif.html

TS:   s.split(",")
来源：http://hz.hammf.cn/gtttaomznw.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.guowangkeji.top/gtyvlxmnkd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xingfuxueyuan.xyz/gtkkfiickt.html

Ruby: s.split(",");  s.split
来源：http://hz.daria6918.cn/gtngexdjdw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hammf.cn/gtxaophkcb.html

[E08] 数组按分隔符合并
来源：http://hz.yuxming.cn/gtraamizua.html

Py:   ",".join(items)
来源：http://hz.smart0.xyz/gtbjvrvkqs.html

PHP:  implode(",", $items);
来源：http://hz.wangshuangyany.cn/gtviiaihsi.html

JS:   items.join(",")
来源：http://hz.hnqzz.top/gtdsptbptr.html

TS:   items.join(",")
来源：http://hz.gzhubu.top/gtkzopvzpe.html

Java: String.join(",", items)
来源：http://hz.xylfe.cn/gthqadzlkz.html

Go:   strings.Join(items, ",")
来源：http://hz.jyoumei.cn/gtvglenvah.html

Ruby: items.join(",")
来源：http://hz.c1oappe.top/gtttoxhesm.html

C#:   string.Join(",", items)
来源：http://hz.smart0.xyz/gtqrlhgjcy.html

[E09] 去除所有空白字符
来源：http://hz.ywan-chungtsiang.top/gtynabgzxi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hnqzz.top/gtjrwaunda.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.feifeiyinyue.top/gteotwfyak.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenjidiqi.icu/gtrlxdrbqu.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yvedp.cn/gtkikomynj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.feifeiyinyue.top/gtnkdiupql.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shanyushiyangkeji.top/gtdctoepil.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jqgufenzy.top/gtbxfkujny.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hongshengwenyu.top/gtthavuwlw.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cheryme.top/gtugrwpzlo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.guannengcc.top/gthscbkzge.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hnxiangtu.top/gtnisajwkg.html

JS:   "7".padStart(3, "0")
来源：http://hz.tanke756.top/gtdpmomuvl.html

TS:   "7".padStart(3, "0")
来源：http://hz.c1oappe.top/gtzycvbcbi.html

Java: String.format("%03d", 7)
来源：http://hz.daria6918.cn/gtwzkpltdl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.havefunace.top/gtrnyyjncd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yj20258.top/gtfdblimrr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.andypj.xyz/gtodogqcyh.html

[E11] 反转字符串
来源：http://hz.andypj.xyz/gtdtzzpzvn.html

Py:   s[::-1]
来源：http://hz.sysykeji.top/gtkmfctycl.html

PHP:  strrev($s);
来源：http://hz.xylfe.cn/gtnhfrunea.html

JS:   [...s].reverse().join("")
来源：http://hz.hfpthk.cn/gtvsasjfwq.html

TS:   [...s].reverse().join("")
来源：http://hz.52xcode.cn/gtlbrrhclg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.daria6918.cn/gtyoilyamq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhoulong.xyz/gtqgjrksvy.html

Ruby: s.reverse
来源：http://hz.jinghuilouyu.cn/gttqhzabwp.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.andypj.xyz/gtinreknit.html

[E12] 统计某字符出现次数
来源：http://hz.yongpay.top/gtxpvbdiie.html

Py:   s.count("a")
来源：http://hz.xylfe.cn/gtxlsdhxcs.html

PHP:  substr_count($s, "a");
来源：http://hz.hongshengwenyu.top/gtrpbxympe.html

JS:   s.split("a").length - 1
来源：http://hz.xziqi.cn/gtaxyrmsna.html

TS:   s.split("a").length - 1
来源：http://hz.pengpengdd.cyou/gtrcocxfqn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ybcxt.top/gthtztwdtj.html

Go:   strings.Count(s, "a")
来源：http://hz.yueranfly.top/gtuyywnvkq.html

Ruby: s.count("a")
来源：http://hz.redwolf501.top/gtpiryxlqn.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sysykeji.top/gtsdpnesiu.html

[E13] 逐字符遍历
来源：http://hz.pycfn.com/gtatsyhlbf.html

Py:   for ch in s: print(ch)
来源：http://hz.birdmap.top/gtdkvrfnqg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ehwqpu.com/gtgahoeixj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtemlmjzld.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jqgufenzy.top/gthdkepfkw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xuetiantiany.cn/gtckzjybky.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yj20258.top/gtmfmxidjb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.sufxvd.cn/gtsxxklhed.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shangyingyoupin.top/gtqvzywymv.html

[E14] URL 编码与 Base64
来源：http://hz.ydjk.org.cn/gtsbuxgzwh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.cashguo.top/gthmyvsjvd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinqigfzy.top/gtcmwocdmj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jyoumei.cn/gtwymwsvni.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shanyushiyangkeji.top/gthrnxgrdb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yj202588.top/gtxnpgcajs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shanyushiyangkeji.top/gtixkomzmh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.cdnleiting.top/gtjwnaeyuj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.gzhubu.top/gtsxyiudkd.html

[E15] HTML 转义 / 反转义
来源：http://hz.tian-w.cn/gtyspgmsxl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yj20258888.top/gthynzmoay.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hfpthk.cn/gtjnvfybds.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jinqigufen.top/gtarhdhrjp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jinyuanbaomall.cn/gtkfyzytqn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinqigufen.top/gtmydofiep.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zycfv.cn/gtevixisub.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shanyushiyangtech.top/gttgaadsgy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.andypj.xyz/gtnlvcfvyk.html

[E16] 数字千分位
来源：http://hz.ehwqpu.com/gtggqecmvv.html

Py:   f"{1234567:,}"
来源：http://hz.jqgufenzy.top/gtcptqnmdy.html

PHP:  number_format(1234567);
来源：http://hz.ydzc1.top/gtiksixncm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuetiantiany.cn/gtxcynmzvw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.pengpengdd.cyou/gtlaxmabhn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gaohongyu789.top/gtvhhdjxuz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.daria6918.cn/gtwjlpysnu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.sysykeji.top/gtaoqbivsq.html

C#:   1234567.ToString("N0")
来源：http://hz.quarkkingdee.top/gthcuinnja.html

[E17] 首字母大写
来源：http://hz.yvedp.cn/gtbpzodsib.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.birdmap.top/gtiktikmlx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yj20258888.top/gtiznvmnfb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nanxuanxn.top/gthoisjgol.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yuanzhike.top/gtahpuhsxw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hongshengwenyu.top/gtsatrzves.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.iojbl.cn/gtergwgwui.html

Ruby: s.capitalize
来源：http://hz.sufxvd.cn/gtrargtcyu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sysykeji.top/gtuavedyil.html

[E18] 模板占位符替换
来源：http://hz.jyoumei.cn/gtrkkqnzje.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xylfe.cn/gtoumhptjj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xziqi.cn/gttpahylhn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shanyushiyangtech.top/gtfnncwsve.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnxiangtu.top/gtspemwjjk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xingfuxueyuan.xyz/gtmotaokks.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yvedp.cn/gthvfysvmo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ppjwa.cn/gtizdajuwe.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.shuidangran.top/gtuskvurev.html

[E19] 多行文本按行拆分
来源：http://hz.chenzaomai.com/gtqyqtfrfk.html

Py:   s.splitlines()
来源：http://hz.tanke756.top/gtcfwxvqxd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.daria6918.cn/gtofusyarn.html

JS:   s.split(/\r?\n/)
来源：http://hz.shanyushiyangkeji.top/gtqdygktoj.html

TS:   s.split(/\r?\n/)
来源：http://hz.9152youxi.cn/gtoxezqjhk.html

Java: s.lines().toList()
来源：http://hz.kuanghao11.cn/gtnpzmufke.html

Go:   strings.Split(s, "\n")
来源：http://hz.daxiang520.top/gthgrhoybk.html

Ruby: s.lines
来源：http://hz.pycfn.com/gtrxqgjuov.html

C#:   s.Split('\n')
来源：http://hz.yanxiufei.cn/gtnwasquul.html

[E20] 判断字符串是否为空
来源：http://hz.tanke756.top/gtezskkwcs.html

Py:   if not s:
来源：http://hz.sysykeji.top/gtkuocuivr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shanyushiyangtech.top/gtqilbuuza.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.haohaochexian.top/gtekesdtoy.html

TS:   if (s === "") {}
来源：http://hz.yuxming.cn/gtrgsfyleh.html

Java: if (s.isEmpty()) {}
来源：http://hz.hywenlv.cn/gtezjbvekh.html

Go:   if s == "" {}
来源：http://hz.yj202588.top/gtxchncopf.html

Ruby: if s.empty?
来源：http://hz.jqgufenzy.top/gtfonawcob.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jqgufenzy.top/gtqvukoomi.html

[E21] 超长截断加省略号
来源：http://hz.ydjk.org.cn/gtcgafmdfb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gaohongyu789.top/gtnvmxgunt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yonumen.top/gtnxytygci.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtnfyjeadr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zycfv.cn/gtufyvfyji.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.bjfxy.top/gthfeiqtve.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tianlin.xyz/gtqyeiqfdm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.sysykeji.top/gtmaymwsaa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hfpthk.cn/gtxdahvxki.html

[E22] 字节长度与字符长度
来源：http://hz.chenlongwang.top/gtincjqbmh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.smart0.xyz/gtmhgmxucn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.havefunace.top/gtovxkajcg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hammf.cn/gtvgtpoifx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuetiantiany.cn/gtohebsmhx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yanxiufei.cn/gtfkzzbsyt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhaomingkeji.xyz/gtxqbudumx.html

Ruby: s.bytesize;  s.length
来源：http://hz.sysykeji.top/gtonqoclbo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yanxiufei.cn/gtfrnyriln.html

================================================================================
来源：http://hz.zhijiandao.cn/gtpxumzuyc.html

F. 文件与目录
来源：http://hz.svipenyu.cn/gtsulyvird.html

================================================================================
来源：http://hz.zdqjudy.top/gtmldoywps.html

[F01] 读取整个文件
来源：http://hz.birdmap.top/gtitijkthp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.havefunace.top/gtllxrayqv.html

PHP:  file_get_contents("a.txt");
来源：http://hz.smart0.xyz/gtywcxmlul.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.9152youxi.cn/gtanyeybmi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xuetiantiany.cn/gtdaqgfwri.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gtsoecaaqt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jqgfzy.top/gthjiolaqc.html

Ruby: File.read("a.txt")
来源：http://hz.xziqi.cn/gttinwuegk.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.fengsongda.top/gtjvgefmgb.html

[F02] 逐行读取文件
来源：http://hz.ivvv.top/gttwwjwapt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jqgfzy.top/gtxmmukvso.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.redwolf501.top/gtoqtirxux.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.bjfxy.top/gttapjshhh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ppjwa.cn/gttnfzomgp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hnxiangtu.top/gtpschnrnk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhongyouzk.top/gtzbkofzmv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.mhx1999.top/gtfpznmsih.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hongshengwenyu.top/gtthmhewuo.html

[F03] 写入文件（覆盖）
来源：http://hz.xylfe.cn/gtgomloyrz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sufxvd.cn/gttgaxcqvj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hywenlv.cn/gttiqqbwcd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.pycfn.com/gtzbsbpixt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnxiangtu.top/gtkdykksgc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.c1oappe.top/gtkfpzhzcl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cqqwz.cn/gtpqqclnfi.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shanyushiyangkeji.top/gtxjlzrdfc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.shanyushiyangtech.top/gtectoszml.html

[F04] 追加写入文件
来源：http://hz.guowangkeji.top/gtrrrvsqow.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.wangshuangyany.cn/gthjtlioku.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yueranfly.top/gtycdlqljx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinqigfzy.top/gtrhrwxnwu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hnxiangtu.top/gtqxftzgsw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gaohongyu789.top/gtygidnead.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xylfe.cn/gtakceecue.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cdnleiting.top/gtmxqyorjk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.snrcjt.cn/gtdmxtdkal.html

[F05] 判断文件或目录是否存在
来源：http://hz.smart0.xyz/gttruwackr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shzxlz.cn/gtxbshbvis.html

PHP:  file_exists("a.txt");
来源：http://hz.316326.xyz/gtblyyazuc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yuxming.cn/gtsiqfhsrs.html

TS:   fs.existsSync("a.txt")
来源：http://hz.guannengcc.top/gthjrawezl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yj20258.top/gtpiiqxots.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hywenlv.cn/gtjzezwmjv.html

Ruby: File.exist?("a.txt")
来源：http://hz.cdnleiting.top/gtvhkcbzoz.html

C#:   File.Exists("a.txt")
来源：http://hz.dashuyun.cn/gtmikuiumd.html

[F06] 删除文件
来源：http://hz.hysaishi.cn/gtbsucxjhz.html

Py:   os.remove("a.txt")
来源：http://hz.havefunace.top/gtelcgrgvv.html

PHP:  unlink("a.txt");
来源：http://hz.ppjwa.cn/gttmhssgxb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.vqdsnc.cn/gtnnfppfhu.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sufxvd.cn/gtbazdtnuu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yj20258.top/gtgchofwtc.html

Go:   os.Remove("a.txt")
来源：http://hz.yangfankeji.com/gtitrsodda.html

Ruby: File.delete("a.txt")
来源：http://hz.smart0.xyz/gtisjfihbg.html

C#:   File.Delete("a.txt");
来源：http://hz.aizwys.cn/gtrezuhkwq.html

[F07] 创建目录（含多级）
来源：http://hz.yonumen.top/gtzeyicudh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yonumen.top/gtycclwaaw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.wangshuangyany.cn/gthfhzdevr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xinyue.icu/gtlzrxhumt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yonumen.top/gtflalqprk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sufxvd.cn/gtdzeqwzou.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hongshengwenyu.top/gtfetbsceg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.smart0.xyz/gthhnkhfpa.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhongyouzk.top/gterlbifdf.html

[F08] 遍历目录
来源：http://hz.dianchejie.cn/gtarczoblq.html


<!-- 参考信息 -->