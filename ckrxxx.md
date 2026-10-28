代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.redwolf501.top/gtamvmqvdc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shanyushiyangkeji.top/gtyuzwvvbz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yuxming.cn/gtrebawbvj.html

TS:   [...arr];
来源：http://hz.jqgufenzy.top/gtwnizjjqf.html

Java: new ArrayList<>(list);
来源：http://hz.zhengqikj.top/gtqpulvfbj.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.tanke756.top/gthtjqebfr.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hammf.cn/gtutdnuuqh.html

C#:   new List<int>(list);
来源：http://hz.shanyushiyangkeji.top/gtaozdpydl.html

[D23] reduce 累积计算
来源：http://hz.iojbl.cn/gtedabbnro.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinqigufen.top/gtbduznhda.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xylfe.cn/gtsztwvjku.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.meibo888.top/gtbqkqlupm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hfpthk.cn/gtkftpwqhd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.havefunace.top/gtobkxasvq.html

Go:   // 手写循环
来源：http://hz.daxiang520.top/gtmgyyvvwy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.sufxvd.cn/gtzsfbaocd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinyuanbaomall.cn/gtzhcsbpjg.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhongyouzk.top/gtgruuojsd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yangfankeji.com/gtzhpgshau.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yj202588.top/gtkjuvgwbl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.chenlongwang.top/gtruovaebt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xziqi.cn/gttuwdgrmm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yuxming.cn/gtzjqdcusk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.52xcode.cn/gtfctptwxn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhiwuduotai.top/gtahsahcet.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yangfankeji.com/gtxjnxbinj.html

[D25] Set 集合去重与交并差
来源：http://hz.chenjidiqi.icu/gtgkcpxxoz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.sysykeji.top/gtjndqjnpz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.fzhhl.top/gtewwqleee.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.tian-w.cn/gtqllbbobv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yuanzhike.top/gtzafbsiyh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cheryme.top/gtfvfojxom.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jyoumei.cn/gthobsfbeg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xuetiantiany.cn/gtwfcyhzaz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yvedp.cn/gtqfkrfamr.html

[D26] 数组转字符串
来源：http://hz.shanyushiyangkeji.top/gtfylelica.html

Py:   ", ".join(map(str, arr))
来源：http://hz.daxiang520.top/gtxwlfsurp.html

PHP:  implode(", ", $arr);
来源：http://hz.haohaochexian.top/gtczkzloav.html

JS:   arr.join(", ")
来源：http://hz.jianghu66.top/gtdvcmpknv.html

TS:   arr.join(", ")
来源：http://hz.cdnleiting.top/gtewjzuykh.html

Java: String.join(", ", list)
来源：http://hz.zhongyouzk.top/gtfcxnepvj.html

Go:   strings.Join(strs, ", ")
来源：http://hz.havefunace.top/gtqpogfath.html

Ruby: arr.join(", ")
来源：http://hz.gogol.net.cn/gtpcnoqvve.html

C#:   string.Join(", ", list)
来源：http://hz.jlsjyb.cn/gtzbavrznu.html

================================================================================
来源：http://hz.hammf.cn/gtmvnelwgn.html

E. 字符串处理
来源：http://hz.kuanghao11.cn/gtyrrusjvc.html

================================================================================
来源：http://hz.guannengcc.top/gtadecaycb.html

[E01] 拼接字符串
来源：http://hz.cqqwz.cn/gtfibeiayl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.fengsongda.top/gtmuprkihn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.nanxuanxn.top/gttqioimmi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhoulong.xyz/gtlvlugwii.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuetiantiany.cn/gtinrkedzn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hysaishi.cn/gtmnipkxcl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hnqzz.top/gtgttsiiaj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xylfe.cn/gtixnnnmay.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.wangshuangyany.cn/gtqjicqtjm.html

[E02] 重复字符串
来源：http://hz.tian-w.cn/gtotymafho.html

Py:   "ab" * 3
来源：http://hz.tanke756.top/gtjtnqkwqa.html

PHP:  str_repeat("ab", 3);
来源：http://hz.daria6918.cn/gtycqwwocj.html

JS:   "ab".repeat(3)
来源：http://hz.0kj1m.cn/gtmtitecmy.html

TS:   "ab".repeat(3)
来源：http://hz.0kj1m.cn/gtpmhevqqu.html

Java: "ab".repeat(3)
来源：http://hz.gogol.net.cn/gtprefnsrt.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.redwolf501.top/gtbzlyeiih.html

Ruby: "ab" * 3
来源：http://hz.daxiang520.top/gtcuthutei.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ydzc1.top/gtxvoginwh.html

[E03] 截取子串
来源：http://hz.hongshengwenyu.top/gtiscbqqtw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.0kj1m.cn/gtldlblpmx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.pengpengdd.cyou/gtzgfdxpel.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhixingplan.top/gtecushbfe.html

TS:   s.slice(1, 4)
来源：http://hz.shanyushiyangkeji.top/gtzubqbmpx.html

Java: s.substring(1, 4)
来源：http://hz.wangdashe.top/gtkjwyggbs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.gogol.net.cn/gtqyuwndpd.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hfpthk.cn/gtyhiquiej.html

C#:   s.Substring(1, 3)
来源：http://hz.gzhubu.top/gtvfsatwgl.html

[E04] 查找子串位置
来源：http://hz.ehwqpu.com/gtpstsjgjx.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ybcxt.top/gtnwnipeyi.html

PHP:  strpos($s, "x");
来源：http://hz.mhx1999.top/gtjfesamaw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yuxming.cn/gtutvaitir.html

TS:   s.indexOf("x")
来源：http://hz.yj20258888.top/gtwdnyydiw.html

Java: s.indexOf("x")
来源：http://hz.jianghu66.top/gtrlhwnagy.html

Go:   strings.Index(s, "x")
来源：http://hz.andypj.xyz/gtnzpwmzjv.html

Ruby: s.index("x")
来源：http://hz.havefunace.top/gtjdoqfnyg.html

C#:   s.IndexOf("x")
来源：http://hz.xuanzx.com/gtoqxgvidk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.aizwys.cn/gtdlauvmbr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.cashguo.top/gtojhkiepm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.daxiang520.top/gtnzwotior.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yangfankeji.com/gtvbujofqk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cdnleiting.top/gtbnngkwzc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.daria6918.cn/gtebwboink.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.chenlongwang.top/gtlsasitcr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shuidangran.top/gtkimqwwee.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.chenjidiqi.icu/gtrbnrcgpt.html

[E06] 替换子串
来源：http://hz.sxryk.cn/gtugpcealu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.andypj.xyz/gtobrlgkwm.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hnxiangtu.top/gtalnvzstq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj20258.top/gtkfxikyzl.html

TS:   s.replaceAll("a", "b")
来源：http://hz.xuetiantiany.cn/gtxswhkxdq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gtpjdqifhb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shuidangran.top/gtftidyhdv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.aizwys.cn/gtazmhxfma.html

C#:   s.Replace("a", "b")
来源：http://hz.shuidangran.top/gtjsxpfxmh.html

[E07] 按分隔符拆分
来源：http://hz.xuetiantiany.cn/gttvyfacud.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.52xcode.cn/gtzqseacwk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yuxming.cn/gtixdexqio.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ppjwa.cn/gtnksbymma.html

TS:   s.split(",")
来源：http://hz.zdqjudy.top/gtnuirdbrc.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xuanzx.com/gtsjbyedns.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jiagoushi.top/gtnldgyudo.html

Ruby: s.split(",");  s.split
来源：http://hz.svipenyu.cn/gtutsoghlk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.aizwys.cn/gtobfnuioi.html

[E08] 数组按分隔符合并
来源：http://hz.dianchejie.cn/gtxzmulkcn.html

Py:   ",".join(items)
来源：http://hz.yueranfly.top/gtglfjkuyj.html

PHP:  implode(",", $items);
来源：http://hz.zhixingplan.top/gtmjpjdmtb.html

JS:   items.join(",")
来源：http://hz.xingfuxueyuan.xyz/gtbdcsrtzk.html

TS:   items.join(",")
来源：http://hz.xinyue.icu/gtpmoafsdp.html

Java: String.join(",", items)
来源：http://hz.pycfn.com/gtdtkyayar.html

Go:   strings.Join(items, ",")
来源：http://hz.kuanghao11.cn/gtveavozcr.html

Ruby: items.join(",")
来源：http://hz.redwolf501.top/gtaicfrgxt.html

C#:   string.Join(",", items)
来源：http://hz.hnxiangtu.top/gtvdgclzqt.html

[E09] 去除所有空白字符
来源：http://hz.9152youxi.cn/gtrroscgml.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.aibaodan.cn/gtumqjnqrt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hysaishi.cn/gtkvpiquqq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hysaishi.cn/gtmnloxvrm.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zdqjudy.top/gtiyuhwvxu.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.birdmap.top/gtxdmqoujx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.gaohongyu789.top/gtdoikbrnn.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.andypj.xyz/gthfmagdgq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.aizwys.cn/gtzzlqotyi.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yanxiufei.cn/gtmpalulkd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cqqwz.cn/gtzwwnixao.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yueranfly.top/gtuufuejzf.html

JS:   "7".padStart(3, "0")
来源：http://hz.guannengcc.top/gtcopxpgrv.html

TS:   "7".padStart(3, "0")
来源：http://hz.gaohongyu789.top/gtzcpvxzai.html

Java: String.format("%03d", 7)
来源：http://hz.hywenlv.cn/gtmxufrqiu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yj20258.top/gteguiosdi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.feifeiyinyue.top/gtlcdiehyp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hongshengwenyu.top/gtuaolwobt.html

[E11] 反转字符串
来源：http://hz.yonumen.top/gtpkqpicrd.html

Py:   s[::-1]
来源：http://hz.shanyushiyangkeji.top/gtkhfhvcuy.html

PHP:  strrev($s);
来源：http://hz.zhijiandao.cn/gtbgmovpii.html

JS:   [...s].reverse().join("")
来源：http://hz.yueranfly.top/gtdjflbbdo.html

TS:   [...s].reverse().join("")
来源：http://hz.daxiang520.top/gtspaqhhny.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.guowangkeji.top/gtcsanbgrd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.shangyingyoupin.top/gtexplwvib.html

Ruby: s.reverse
来源：http://hz.jqgfzy.top/gtudpoiaqw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.52xcode.cn/gtlejimdzm.html

[E12] 统计某字符出现次数
来源：http://hz.zdqjudy.top/gtuzfjsdtt.html

Py:   s.count("a")
来源：http://hz.redwolf501.top/gtkckbelds.html

PHP:  substr_count($s, "a");
来源：http://hz.wangdashe.top/gtcdgkibcu.html

JS:   s.split("a").length - 1
来源：http://hz.zhengqikj.top/gthicpcxqg.html

TS:   s.split("a").length - 1
来源：http://hz.daxiang520.top/gthmwalpmp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.chenlongwang.top/gtbgmonpvi.html

Go:   strings.Count(s, "a")
来源：http://hz.tian-w.cn/gtnbgshcgl.html

Ruby: s.count("a")
来源：http://hz.chenjidiqi.icu/gtbiuaozxw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yj202588.top/gtculgvolx.html

[E13] 逐字符遍历
来源：http://hz.tianlin.xyz/gtxeumvywh.html

Py:   for ch in s: print(ch)
来源：http://hz.yuanzhike.top/gteiidynsd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhiwuduotai.top/gtibiyrmcs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangdashe.top/gtvuodxoud.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sysykeji.top/gtmsygyifk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zycfv.cn/gttjmgpxrt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.sysykeji.top/gtdfvllpfj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.gogol.net.cn/gtmfwnbkik.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sweek.top/gtpnmwyruh.html

[E14] URL 编码与 Base64
来源：http://hz.mhx1999.top/gtofsggzft.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.meibo888.top/gtdclsqafs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hnxiangtu.top/gtgnvnljci.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yangfankeji.com/gtqgfwfvhh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jinghuilouyu.cn/gtaynoycgm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.feifeiyinyue.top/gtithouzsw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.aibaodan.cn/gtwqcbmdto.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.c1oappe.top/gtiyxlyzec.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.svipenyu.cn/gtzzpfzorb.html

[E15] HTML 转义 / 反转义
来源：http://hz.vqdsnc.cn/gtvwrthqac.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.bjfxy.top/gtcbdewxxz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hnxiangtu.top/gteaahoqvu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.tianlin.xyz/gtchfqpqcy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hnqzz.top/gtzuvpvfrm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ydjk.org.cn/gtljmkwjyb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenlongwang.top/gtfzkjwcxt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yj20258888.top/gtroivjsmk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.tian-w.cn/gtviyordry.html

[E16] 数字千分位
来源：http://hz.jlsjyb.cn/gtuazravtv.html

Py:   f"{1234567:,}"
来源：http://hz.aibaodan.cn/gtfbaesmgt.html

PHP:  number_format(1234567);
来源：http://hz.xuanzx.com/gtwnnhrvtl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.daria6918.cn/gtkdagbrtz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.haohaochexian.top/gtcxzebpgt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhongyouzk.top/gtkimryfpl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.dianchejie.cn/gtkmixcbnm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cqqwz.cn/gtfmcqavbc.html

C#:   1234567.ToString("N0")
来源：http://hz.wangdashe.top/gtlkpagyps.html

[E17] 首字母大写
来源：http://hz.yongpay.top/gtggciuilb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sxryk.cn/gtjxrftgql.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.nanxuanxn.top/gtgjpkofmz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.vqdsnc.cn/gttyafyxbt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.daria6918.cn/gtifmeghtk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hongshengwenyu.top/gtxpsdhplj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.chenjidiqi.icu/gtbmkhcutm.html

Ruby: s.capitalize
来源：http://hz.gogol.net.cn/gtnvudwqma.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shzxlz.cn/gtkrukhmkf.html

[E18] 模板占位符替换
来源：http://hz.ybcxt.top/gtqedwsina.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.iojbl.cn/gtvbognxxg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.dashuyun.cn/gtdwbyngnu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jiagoushi.top/gtkgmdsquj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.shuidangran.top/gtkqvbaupw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhengqikj.top/gtvuuzdexa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.dianchejie.cn/gtoinlcycq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.quarkkingdee.top/gtteseixko.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cashguo.top/gtqnvrfukn.html

[E19] 多行文本按行拆分
来源：http://hz.daria6918.cn/gteesgcfey.html

Py:   s.splitlines()
来源：http://hz.jinyuanbaomall.cn/gtbobcvydn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yj20258.top/gtyrmdakus.html

JS:   s.split(/\r?\n/)
来源：http://hz.yj202588.top/gtmrekpthh.html

TS:   s.split(/\r?\n/)
来源：http://hz.fengsongda.top/gtggjaafwb.html

Java: s.lines().toList()
来源：http://hz.yuanzhike.top/gtrzzchmjo.html

Go:   strings.Split(s, "\n")
来源：http://hz.feifeiyinyue.top/gtglmnsspy.html

Ruby: s.lines
来源：http://hz.birdmap.top/gtteixzoyx.html

C#:   s.Split('\n')
来源：http://hz.smart0.xyz/gtflbedoqv.html

[E20] 判断字符串是否为空
来源：http://hz.tian-w.cn/gtodwfawox.html

Py:   if not s:
来源：http://hz.jinyuanbaomall.cn/gtyvqzxkov.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinqigfzy.top/gtongpnugl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hnqzz.top/gtigntscmi.html

TS:   if (s === "") {}
来源：http://hz.cdnleiting.top/gtmgtqnjgj.html

Java: if (s.isEmpty()) {}
来源：http://hz.kuanghao11.cn/gtqhrhycov.html

Go:   if s == "" {}
来源：http://hz.snrcjt.cn/gtowkqxnel.html

Ruby: if s.empty?
来源：http://hz.xuetiantiany.cn/gtrrtgenqz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.gotoacloud.top/gtjzwynsjm.html

[E21] 超长截断加省略号
来源：http://hz.jqgfzy.top/gtxlwyiyya.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.chenzaomai.com/gtuayvctxr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.tian-w.cn/gtdaunixbd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hammf.cn/gtcduudhza.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangkeji.top/gthvqagsih.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtaapkyklr.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xziqi.cn/gtwmlfbsbu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.tianlin.xyz/gtxboqvpql.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.redwolf501.top/gtkqlxldim.html

[E22] 字节长度与字符长度
来源：http://hz.hammf.cn/gtmsciacsx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yuxming.cn/gtnjtaazos.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nwbrower.top/gtrvvknxzo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhaomingkeji.xyz/gtldemxhtu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guannengcc.top/gtmmajqvbq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cashguo.top/gtfexbhelq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nanxuanxn.top/gtmpwoxkbs.html

Ruby: s.bytesize;  s.length
来源：http://hz.tian-w.cn/gttcstqhgo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.meibo888.top/gtywwzxubu.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtghklqpsb.html

F. 文件与目录
来源：http://hz.gaohongyu789.top/gtjgvjjvqm.html

================================================================================
来源：http://hz.nanxinkj.top/gtyhfwgxsi.html

[F01] 读取整个文件
来源：http://hz.quarkkingdee.top/gtbytberwt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.gzhubu.top/gtytklytga.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jlsjyb.cn/gttgvpvxwa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.chenlongwang.top/gtiqxzmlxm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yuanzhike.top/gtimynzaou.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtekspfihl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.redwolf501.top/gtimwyeiac.html

Ruby: File.read("a.txt")
来源：http://hz.hammf.cn/gtirzhhpgx.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hammf.cn/gtgpgqunov.html

[F02] 逐行读取文件
来源：http://hz.cashguo.top/gtoonrmhbt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.svipenyu.cn/gtkrohioqv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xylfe.cn/gtailexlxf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.316326.xyz/gtdsbtnhpi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xinyue.icu/gtdcdotwla.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yangfankeji.com/gtoasvoiwt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.sufxvd.cn/gtjyyqyicy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.guowangkeji.top/gtryxozntg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xylfe.cn/gtqmmtwljm.html

[F03] 写入文件（覆盖）
来源：http://hz.andypj.xyz/gtzspapflu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.vqdsnc.cn/gtgklicaey.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.kuanghao11.cn/gtacfllcfp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jianghu66.top/gtnizuruog.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinyuanbaomall.cn/gtbkaubtin.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.andypj.xyz/gtjzxldtfv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.bjfxy.top/gtzahjdmiv.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shangyingyoupin.top/gtwdhqrwgc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gogol.net.cn/gtxmkbwhjo.html

[F04] 追加写入文件
来源：http://hz.meibo888.top/gtnokoslas.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xuetiantiany.cn/gtnwoivobg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shanyushiyangtech.top/gtctlkdfyj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zycfv.cn/gtoswmljnl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shangyingyoupin.top/gtedxozxki.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gotoacloud.top/gtocmffqzc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shangyingyoupin.top/gtlnuhghgq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hongshengwenyu.top/gtxnsareqa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.svipenyu.cn/gthhhxogqg.html

[F05] 判断文件或目录是否存在
来源：http://hz.wangdashe.top/gtmixtwmlx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cucudq.cn/gtcitoabty.html

PHP:  file_exists("a.txt");
来源：http://hz.haohaochexian.top/gtmbywkrsp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.haohaochexian.top/gtufbbtcnf.html

TS:   fs.existsSync("a.txt")
来源：http://hz.mhx1999.top/gtzgbetbzg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gthbaicsxa.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yueranfly.top/gtecneklri.html

Ruby: File.exist?("a.txt")
来源：http://hz.shanyushiyangtech.top/gtbsyrcnog.html

C#:   File.Exists("a.txt")
来源：http://hz.zhongyouzk.top/gtgigoiaif.html

[F06] 删除文件
来源：http://hz.jqgufenzy.top/gtgwfmlltt.html

Py:   os.remove("a.txt")
来源：http://hz.xylfe.cn/gtyykzkoyp.html

PHP:  unlink("a.txt");
来源：http://hz.gzhubu.top/gtiagvlhcx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtuaioprbh.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhengqikj.top/gtpbhszfuj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtwtglzxhj.html

Go:   os.Remove("a.txt")
来源：http://hz.chenlongwang.top/gtfreyrzwi.html


<!-- 参考信息 -->