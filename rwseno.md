代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yangfankeji.com/gtblagoplp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ehwqpu.com/gtxntxrqzt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yangfankeji.com/gtdstibxzj.html

Go:   // 手写 map[T]int
来源：http://hz.sysykeji.top/gtwgdjjkdq.html

Ruby: arr.tally
来源：http://hz.xinyue.icu/gtfnzuxsug.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yangfankeji.com/gtekmwsobb.html

[D21] 判断是否包含某元素
来源：http://hz.zhijiandao.cn/gturofwdld.html

Py:   x in arr
来源：http://hz.mhx1999.top/gtjwcavumk.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jyoumei.cn/gtkdxndppr.html

JS:   arr.includes(x)
来源：http://hz.nanxuanxn.top/gtvcmsgklf.html

TS:   arr.includes(x)
来源：http://hz.hywenlv.cn/gtpbeuyehg.html

Java: list.contains(x)
来源：http://hz.haohaochexian.top/gtmtlmxtma.html

Go:   slices.Contains(arr, x)
来源：http://hz.nwbrower.top/gtmkwunveu.html

Ruby: arr.include?(x)
来源：http://hz.yuxming.cn/gtfjjcufhd.html

C#:   list.Contains(x)
来源：http://hz.shanyushiyangkeji.top/gtcfpyqcuu.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ywan-chungtsiang.top/gtouacchbz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.iojbl.cn/gtcbpkkczd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shanyushiyangkeji.top/gtligyjyil.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hongshengwenyu.top/gtlfhbmbpm.html

TS:   [...arr];
来源：http://hz.jqgfzy.top/gtnjgtfhdt.html

Java: new ArrayList<>(list);
来源：http://hz.jqgufenzy.top/gtpewzeyfi.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jlsjyb.cn/gtgsesbtnn.html

Ruby: arr.dup;  arr.clone
来源：http://hz.havefunace.top/gtyogkjohu.html

C#:   new List<int>(list);
来源：http://hz.cdnleiting.top/gtznlnjdqk.html

[D23] reduce 累积计算
来源：http://hz.chenlongwang.top/gtyhrcoaon.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinqigfzy.top/gtrsnfnzta.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sweek.top/gthdrainnc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jiagoushi.top/gtthttcakz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sysykeji.top/gtrzqpqxzw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.mhx1999.top/gttjghvjpc.html

Go:   // 手写循环
来源：http://hz.ivvv.top/gtzyfzudga.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.mhx1999.top/gtlvqyhcwc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yangfankeji.com/gtdzkyoryh.html

[D24] 字典 / Map 基本操作
来源：http://hz.tanke756.top/gtyllpuped.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ivvv.top/gtkuyiapvs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yangfankeji.com/gtwxmhvybv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.chenlongwang.top/gtxjlrunqw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj20258888.top/gtxcbnlhsf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.gogol.net.cn/gtwrrkkuwq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yuxming.cn/gtvgnsstxz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhoulong.xyz/gtvfqxbsph.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.tianlin.xyz/gttbuhvolw.html

[D25] Set 集合去重与交并差
来源：http://hz.ywan-chungtsiang.top/gthmkutyhx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ywan-chungtsiang.top/gtbbrytybe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cucudq.cn/gtoppxlhnp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.c1oappe.top/gtzsrrpgza.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhiwuduotai.top/gtukvimfyc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.tian-w.cn/gtlrzhrvut.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cqqwz.cn/gtegcvokus.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yongpay.top/gtinjabarh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.mhx1999.top/gtpsaefaak.html

[D26] 数组转字符串
来源：http://hz.svipenyu.cn/gtzwqfxecz.html

Py:   ", ".join(map(str, arr))
来源：http://hz.guowangkeji.top/gtpgvddqjw.html

PHP:  implode(", ", $arr);
来源：http://hz.ydzc1.top/gtomqdtzkp.html

JS:   arr.join(", ")
来源：http://hz.jyoumei.cn/gtefyceqrr.html

TS:   arr.join(", ")
来源：http://hz.cucudq.cn/gtgkznsgzn.html

Java: String.join(", ", list)
来源：http://hz.cashguo.top/gtogrkindz.html

Go:   strings.Join(strs, ", ")
来源：http://hz.tianlin.xyz/gtrrleigvd.html

Ruby: arr.join(", ")
来源：http://hz.tianlin.xyz/gtpuzeckfi.html

C#:   string.Join(", ", list)
来源：http://hz.ydjk.org.cn/gtjcoopvfq.html

================================================================================
来源：http://hz.fengsongda.top/gtbsfpsdjg.html

E. 字符串处理
来源：http://hz.hysaishi.cn/gtazksnzox.html

================================================================================
来源：http://hz.yj20258.top/gtiqwvobcg.html

[E01] 拼接字符串
来源：http://hz.zhixingplan.top/gtxbsbgofs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yanxiufei.cn/gtjhncjxzm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cdnleiting.top/gtktuaktrz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.iojbl.cn/gtldprhyzz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cucudq.cn/gtfwrpdlkf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.feifeiyinyue.top/gtntfbapxp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhixingplan.top/gtssijajby.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.sufxvd.cn/gtorxskhls.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sxryk.cn/gtestqurwx.html

[E02] 重复字符串
来源：http://hz.c1oappe.top/gtpjuovbjg.html

Py:   "ab" * 3
来源：http://hz.52xcode.cn/gtslkhyrvs.html

PHP:  str_repeat("ab", 3);
来源：http://hz.nanxuanxn.top/gtbkqrdgly.html

JS:   "ab".repeat(3)
来源：http://hz.yueranfly.top/gtgwkbpwbp.html

TS:   "ab".repeat(3)
来源：http://hz.shanyushiyangtech.top/gtriunzgrf.html

Java: "ab".repeat(3)
来源：http://hz.pengpengdd.cyou/gtxliumetq.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.c1oappe.top/gtjevxdchf.html

Ruby: "ab" * 3
来源：http://hz.yuanzhike.top/gtaoewjjyl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.chenzaomai.com/gtccyqvdtr.html

[E03] 截取子串
来源：http://hz.jinqigufen.top/gtukumyxqd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cdnleiting.top/gtkefzlgbp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jyoumei.cn/gtrheekszk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yangfankeji.com/gtrbpaambz.html

TS:   s.slice(1, 4)
来源：http://hz.haohaochexian.top/gtbyhtfqqj.html

Java: s.substring(1, 4)
来源：http://hz.xinyue.icu/gtketqarbr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.shanyushiyangtech.top/gtnaoigfba.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.chenzaomai.com/gtdxycprnq.html

C#:   s.Substring(1, 3)
来源：http://hz.yj20258.top/gtclixvxnb.html

[E04] 查找子串位置
来源：http://hz.tianlin.xyz/gtfeohurwz.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jinqigufen.top/gtqgxqulry.html

PHP:  strpos($s, "x");
来源：http://hz.pycfn.com/gtexcwkccc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ivvv.top/gtwbshivhq.html

TS:   s.indexOf("x")
来源：http://hz.pycfn.com/gtwyvypcie.html

Java: s.indexOf("x")
来源：http://hz.shanyushiyangkeji.top/gtnwkpmpab.html

Go:   strings.Index(s, "x")
来源：http://hz.cucudq.cn/gtvkumsvys.html

Ruby: s.index("x")
来源：http://hz.zhoulong.xyz/gtkkzvexup.html

C#:   s.IndexOf("x")
来源：http://hz.pengpengdd.cyou/gtwmezbycf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ydzc1.top/gtuxaludmm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.gotoacloud.top/gtxzpcktzi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zycfv.cn/gteniabuup.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.mhx1999.top/gtozgamtjh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cashguo.top/gtvwertfdi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinyuanbaomall.cn/gtkwkpfbwp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.chenzaomai.com/gtxbrdcuva.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hongshengwenyu.top/gtsuieqsah.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jinyuanbaomall.cn/gthiysnayj.html

[E06] 替换子串
来源：http://hz.zhongyouzk.top/gtrlbjncnb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xuanzx.com/gtokofgpgo.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.guowangkeji.top/gtdzouzifh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtxfndcsrj.html

TS:   s.replaceAll("a", "b")
来源：http://hz.chenlongwang.top/gtxqfpzywg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xuanzx.com/gtknhjaupp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sweek.top/gtsyvyhsog.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ydjk.org.cn/gtwxivlalu.html

C#:   s.Replace("a", "b")
来源：http://hz.feifeiyinyue.top/gtbvdsvzsj.html

[E07] 按分隔符拆分
来源：http://hz.hammf.cn/gtgambebzf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yangfankeji.com/gteadjdllu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtreumvblx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhoulong.xyz/gtuplexasd.html

TS:   s.split(",")
来源：http://hz.xinyue.icu/gtyirsbypm.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.meibo888.top/gtfprnyuby.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.pycfn.com/gteihzeluw.html

Ruby: s.split(",");  s.split
来源：http://hz.dashuyun.cn/gtgshjwcbz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yj20258888.top/gtnluafibp.html

[E08] 数组按分隔符合并
来源：http://hz.hnqzz.top/gticruikgt.html

Py:   ",".join(items)
来源：http://hz.shanyushiyangtech.top/gtdnubkvht.html

PHP:  implode(",", $items);
来源：http://hz.snrcjt.cn/gttuuvqmuz.html

JS:   items.join(",")
来源：http://hz.daria6918.cn/gtrffnwgfa.html

TS:   items.join(",")
来源：http://hz.hnqzz.top/gtgrhjhvkz.html

Java: String.join(",", items)
来源：http://hz.hysaishi.cn/gtctjuqowd.html

Go:   strings.Join(items, ",")
来源：http://hz.xylfe.cn/gtzqpiahcl.html

Ruby: items.join(",")
来源：http://hz.yangfankeji.com/gtzxgqcoaj.html

C#:   string.Join(",", items)
来源：http://hz.guannengcc.top/gtjaowdesh.html

[E09] 去除所有空白字符
来源：http://hz.quarkkingdee.top/gtjminuucg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hongshengwenyu.top/gtpqujghdf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.pycfn.com/gtldzbjfhk.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ydzc1.top/gtjidlmgxn.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.quarkkingdee.top/gtvnxszcjh.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.sufxvd.cn/gttgohnmzf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.haohaochexian.top/gtqeeaamvp.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.aibaodan.cn/gteofrqksd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.fengsongda.top/gtpnlejdla.html

[E10] 左侧补零 / 定长填充
来源：http://hz.andypj.xyz/gtuhcbizep.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yvedp.cn/gtxomswglg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.feifeiyinyue.top/gtlhpsogih.html

JS:   "7".padStart(3, "0")
来源：http://hz.fzhhl.top/gtwsbsjznx.html

TS:   "7".padStart(3, "0")
来源：http://hz.jqgfzy.top/gtsdtvxztc.html

Java: String.format("%03d", 7)
来源：http://hz.kuanghao11.cn/gtesdbskae.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hnqzz.top/gttvwomrsf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gotoacloud.top/gttrtweacu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.dashuyun.cn/gtqpxgfcdx.html

[E11] 反转字符串
来源：http://hz.zhaomingkeji.xyz/gtmlohuxod.html

Py:   s[::-1]
来源：http://hz.ppjwa.cn/gtlfllxktx.html

PHP:  strrev($s);
来源：http://hz.hongshengwenyu.top/gtajunmcvz.html

JS:   [...s].reverse().join("")
来源：http://hz.hywenlv.cn/gtiutanonw.html

TS:   [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtclsofbaq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.vqdsnc.cn/gthkaymygy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jianghu66.top/gthuvngvwy.html

Ruby: s.reverse
来源：http://hz.hysaishi.cn/gtmjtxoolj.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.dianchejie.cn/gtzjfyydyc.html

[E12] 统计某字符出现次数
来源：http://hz.cucudq.cn/gteqogsjnn.html

Py:   s.count("a")
来源：http://hz.yuxming.cn/gtmdfxzcwt.html

PHP:  substr_count($s, "a");
来源：http://hz.52xcode.cn/gtzlkqojmq.html

JS:   s.split("a").length - 1
来源：http://hz.nanxuanxn.top/gtyadoaabl.html

TS:   s.split("a").length - 1
来源：http://hz.xinyue.icu/gtjgqgpnll.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.dianchejie.cn/gtjnkspmwv.html

Go:   strings.Count(s, "a")
来源：http://hz.daxiang520.top/gtoyatldwu.html

Ruby: s.count("a")
来源：http://hz.svipenyu.cn/gtcwnrdbie.html

C#:   s.Count(c => c == 'a')
来源：http://hz.feifeiyinyue.top/gtwdzpisps.html

[E13] 逐字符遍历
来源：http://hz.cheryme.top/gtcrvhytck.html

Py:   for ch in s: print(ch)
来源：http://hz.cheryme.top/gtgvpdgenc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yueranfly.top/gtgjeuldvz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuanzhike.top/gttpdzvcqg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gotoacloud.top/gteggbvflf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hammf.cn/gtheudahud.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.dianchejie.cn/gtvsrecdqz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cashguo.top/gtcgnpmebx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xuanzx.com/gtijzhmxbg.html

[E14] URL 编码与 Base64
来源：http://hz.jqgufenzy.top/gtashldxrt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jyoumei.cn/gttnmfwqsv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.tian-w.cn/gtlfsqrhwf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xylfe.cn/gthmjasbar.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yj20258.top/gtrivhunny.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhoulong.xyz/gtplkkayqh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.birdmap.top/gtbvttuxep.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.guowangkeji.top/gtqbgrfewe.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ppjwa.cn/gthjkvzcbj.html

[E15] HTML 转义 / 反转义
来源：http://hz.ybcxt.top/gtgmkwergt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shanyushiyangtech.top/gtjtwxzoeh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yj20258.top/gtsgdvfkit.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.feifeiyinyue.top/gtzceezggn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ywan-chungtsiang.top/gtvpxighmh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shanyushiyangtech.top/gtvxfhobsi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.svipenyu.cn/gtvxpyrbyy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.meibo888.top/gtatezhdvl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.mhx1999.top/gtwtkeorcy.html

[E16] 数字千分位
来源：http://hz.quarkkingdee.top/gtkodvfosg.html

Py:   f"{1234567:,}"
来源：http://hz.wangdashe.top/gtwxygcfnr.html

PHP:  number_format(1234567);
来源：http://hz.snrcjt.cn/gtkopicgfv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenjidiqi.icu/gtepuvdlab.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.iojbl.cn/gtxmrmpijp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xinyue.icu/gtueipkghp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jianghu66.top/gtfxteviyz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ydjk.org.cn/gtikrcmluf.html

C#:   1234567.ToString("N0")
来源：http://hz.yvedp.cn/gttpsxmtzj.html

[E17] 首字母大写
来源：http://hz.c1oappe.top/gtsszhsajz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.316326.xyz/gtpdxebzhs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jinqigufen.top/gtzvkwwycf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangtech.top/gtjsfxfcir.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nanxuanxn.top/gthgjmugxg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shzxlz.cn/gtxmhrwonn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shanyushiyangtech.top/gtuokiakjg.html

Ruby: s.capitalize
来源：http://hz.ybcxt.top/gtonzzwxre.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.dianchejie.cn/gtnmqauzvl.html

[E18] 模板占位符替换
来源：http://hz.svipenyu.cn/gtnkyehjdc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhengqikj.top/gtqcomacqt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cheryme.top/gtmnenvtxu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.haohaochexian.top/gtcnvhrzln.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.pengpengdd.cyou/gtnnaqeoto.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zycfv.cn/gtgxdolbqm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.wangshuangyany.cn/gtxopasvwo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ppjwa.cn/gtcxcdemjj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jinghuilouyu.cn/gthwpzwdgf.html

[E19] 多行文本按行拆分
来源：http://hz.zhixingplan.top/gtryfhfmwo.html

Py:   s.splitlines()
来源：http://hz.zhongyouzk.top/gtjpffquyx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jianghu66.top/gtkpvwhumr.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhongyouzk.top/gtuhalwoht.html

TS:   s.split(/\r?\n/)
来源：http://hz.daria6918.cn/gtcztthwdj.html

Java: s.lines().toList()
来源：http://hz.gotoacloud.top/gtfojdvfyn.html

Go:   strings.Split(s, "\n")
来源：http://hz.yanxiufei.cn/gtxoqxuyom.html

Ruby: s.lines
来源：http://hz.zhongyouzk.top/gtjsfjgijv.html

C#:   s.Split('\n')
来源：http://hz.nanxinkj.top/gtjffbcuzi.html

[E20] 判断字符串是否为空
来源：http://hz.cqqwz.cn/gthovyljlq.html

Py:   if not s:
来源：http://hz.zdqjudy.top/gtnfprllpo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.chenlongwang.top/gtynhxvbxk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hammf.cn/gtbitotisc.html

TS:   if (s === "") {}
来源：http://hz.zdqjudy.top/gtkvmzsjkk.html

Java: if (s.isEmpty()) {}
来源：http://hz.havefunace.top/gtawzokrpn.html

Go:   if s == "" {}
来源：http://hz.cdnleiting.top/gtrgneufcn.html

Ruby: if s.empty?
来源：http://hz.nanxinkj.top/gtftxkzykx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.fzhhl.top/gtygnuppqq.html

[E21] 超长截断加省略号
来源：http://hz.ybcxt.top/gtfdzfzxrj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.dashuyun.cn/gtmjdfljqq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ivvv.top/gtfaekxhoa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.mhx1999.top/gtdjrvwhha.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhixingplan.top/gtbsrmanut.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtsmtgvcha.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jinyuanbaomall.cn/gtxsodowgz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.sysykeji.top/gtwgzebdxc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hnxiangtu.top/gtqxmjfpnb.html

[E22] 字节长度与字符长度
来源：http://hz.ehwqpu.com/gtwewdhkjo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xuanzx.com/gtmtldkmli.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sweek.top/gtubngbilo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yvedp.cn/gthmuxthms.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zdqjudy.top/gtzcusiisq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.birdmap.top/gtqpehzaaq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.birdmap.top/gtakkygkix.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinghuilouyu.cn/gtdhswtdnq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jinghuilouyu.cn/gtbvksnbps.html

================================================================================
来源：http://hz.quarkkingdee.top/gtjcpkimnz.html

F. 文件与目录
来源：http://hz.hfpthk.cn/gtygdbneqg.html

================================================================================
来源：http://hz.chenjidiqi.icu/gthaamjubb.html

[F01] 读取整个文件
来源：http://hz.tanke756.top/gtddaghpda.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hnxiangtu.top/gteonmusvc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.0kj1m.cn/gtvrnnnpke.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.nanxuanxn.top/gthykeishx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.fengsongda.top/gtvedftqxm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtqzlvjzaa.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shuidangran.top/gtbujxitzl.html

Ruby: File.read("a.txt")
来源：http://hz.xuanzx.com/gtqgflqexp.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.wangshuangyany.cn/gtjtdqfouj.html

[F02] 逐行读取文件
来源：http://hz.aibaodan.cn/gtcwlajhqd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.wangdashe.top/gtprvcwrof.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.fengsongda.top/gtdlquzwcz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shzxlz.cn/gtvffrgmrq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhongyouzk.top/gtecnsqgzv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.kuanghao11.cn/gtmeukfvfu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.wangshuangyany.cn/gtuwbwllzo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xinyue.icu/gtttylaplv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sweek.top/gtfghtzalb.html

[F03] 写入文件（覆盖）
来源：http://hz.yuxming.cn/gtvsqgfuyw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.nwbrower.top/gtxayjegxw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.316326.xyz/gtfyyhggrl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cqqwz.cn/gtlxhhpkci.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenjidiqi.icu/gtokrvxsmq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hongshengwenyu.top/gtfoqnrtat.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xuanzx.com/gthkedudnx.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shanyushiyangtech.top/gtesmgynbq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.daxiang520.top/gtkytoxham.html

[F04] 追加写入文件
来源：http://hz.yj20258.top/gtcfkqgrgs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jianghu66.top/gtkcwgbfln.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yangfankeji.com/gtfltbgfci.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.redwolf501.top/gthyrkaxey.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhiwuduotai.top/gtobwllgmq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yueranfly.top/gtojhekbez.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.tian-w.cn/gtadzwtvmv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhiwuduotai.top/gtkppwssek.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.nanxuanxn.top/gtoorjhisz.html


<!-- 参考信息 -->