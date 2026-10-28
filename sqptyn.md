代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhixingplan.top/gtcnwylvfi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.aizwys.cn/gtizmnascm.html

Go:   // 手写 map[string][]T
来源：http://hz.yonumen.top/gtsxwsjfbr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shanyushiyangtech.top/gtknhdfsxh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hywenlv.cn/gtlwynyadb.html

[D20] 统计每个元素出现次数
来源：http://hz.cqqwz.cn/gtqlmeeyxb.html

Py:   Counter(arr)
来源：http://hz.zhiwuduotai.top/gtrekmrpsg.html

PHP:  array_count_values($arr);
来源：http://hz.jqgufenzy.top/gtzhowpmwf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dashuyun.cn/gtagvkkrmf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.316326.xyz/gtgxacwkcr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.dashuyun.cn/gtbwzdyfun.html

Go:   // 手写 map[T]int
来源：http://hz.quarkkingdee.top/gthoebvnqh.html

Ruby: arr.tally
来源：http://hz.nwbrower.top/gtvmtamylp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zycfv.cn/gtvuvynfhq.html

[D21] 判断是否包含某元素
来源：http://hz.pycfn.com/gttumsbbqd.html

Py:   x in arr
来源：http://hz.hnxiangtu.top/gtiniremyp.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gotoacloud.top/gtypxorhlf.html

JS:   arr.includes(x)
来源：http://hz.andypj.xyz/gtvtjzbjhh.html

TS:   arr.includes(x)
来源：http://hz.cashguo.top/gtihpmsdhy.html

Java: list.contains(x)
来源：http://hz.dianchejie.cn/gtmbmlekso.html

Go:   slices.Contains(arr, x)
来源：http://hz.jinghuilouyu.cn/gtjclzewcy.html

Ruby: arr.include?(x)
来源：http://hz.xingfuxueyuan.xyz/gtbedpnltc.html

C#:   list.Contains(x)
来源：http://hz.fengsongda.top/gtpmrqdoib.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zycfv.cn/gtopwcatjh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xylfe.cn/gtwjqvnnsv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.nanxinkj.top/gtvrcdsuty.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jiagoushi.top/gtilsjnqem.html

TS:   [...arr];
来源：http://hz.yangfankeji.com/gtctrvmxyt.html

Java: new ArrayList<>(list);
来源：http://hz.zhengqikj.top/gtaigezwjc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.daxiang520.top/gtuytwgwmg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.bjfxy.top/gtcttzltrt.html

C#:   new List<int>(list);
来源：http://hz.tianlin.xyz/gtvzowjljs.html

[D23] reduce 累积计算
来源：http://hz.jlsjyb.cn/gtuektmmck.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yvedp.cn/gtzgmowoeo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhijiandao.cn/gtzxcglfsc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cqqwz.cn/gtqhfqpqbw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guowangkeji.top/gtiivntepl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hammf.cn/gtcfnyqfcl.html

Go:   // 手写循环
来源：http://hz.sufxvd.cn/gtcfsosdwr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.fzhhl.top/gtqzrtmgyw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.birdmap.top/gtlpfbjgxj.html

[D24] 字典 / Map 基本操作
来源：http://hz.gzhubu.top/gtpzuxenri.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.quarkkingdee.top/gtctcctuib.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.havefunace.top/gtsmuuynjw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.kuanghao11.cn/gtlsivzvrv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sxryk.cn/gtgeljhjwj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nanxinkj.top/gtlyuchpuu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.chenjidiqi.icu/gtzicakyql.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sxryk.cn/gttvbforwk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.chenlongwang.top/gtpzhhzxap.html

[D25] Set 集合去重与交并差
来源：http://hz.guannengcc.top/gtwvvjhaqa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jyoumei.cn/gtlnjozsrl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.9152youxi.cn/gtprecznsp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jlsjyb.cn/gtziqgcuon.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhixingplan.top/gtlxvzgdxx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.dianchejie.cn/gtrzipxlez.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yj202588.top/gtdwcfxomb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.wangdashe.top/gtuhdrymgm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shangyingyoupin.top/gtxmxzbvpt.html

[D26] 数组转字符串
来源：http://hz.chenlongwang.top/gtsojtttuf.html

Py:   ", ".join(map(str, arr))
来源：http://hz.52xcode.cn/gtgiefmvxu.html

PHP:  implode(", ", $arr);
来源：http://hz.shuidangran.top/gtynkbbcnk.html

JS:   arr.join(", ")
来源：http://hz.cqqwz.cn/gtqznovvie.html

TS:   arr.join(", ")
来源：http://hz.zhiwuduotai.top/gtohhoitxz.html

Java: String.join(", ", list)
来源：http://hz.hongshengwenyu.top/gtlishjbvh.html

Go:   strings.Join(strs, ", ")
来源：http://hz.daria6918.cn/gttrwiuivf.html

Ruby: arr.join(", ")
来源：http://hz.jianghu66.top/gtzkrnhjxj.html

C#:   string.Join(", ", list)
来源：http://hz.wangdashe.top/gtwqaogbur.html

================================================================================
来源：http://hz.dashuyun.cn/gtzoefxplg.html

E. 字符串处理
来源：http://hz.yj20258.top/gtbccqoqcj.html

================================================================================
来源：http://hz.yongpay.top/gtscqgellt.html

[E01] 拼接字符串
来源：http://hz.zycfv.cn/gtvksrbgtj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ywan-chungtsiang.top/gtxnydpvwt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.smart0.xyz/gtnigqzmct.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sysykeji.top/gtswmvbklu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jiagoushi.top/gtcuugmxqz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.mhx1999.top/gtqclosarr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ydjk.org.cn/gtlefdwunh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.tianlin.xyz/gtmxftrgxe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hysaishi.cn/gtvukeoneo.html

[E02] 重复字符串
来源：http://hz.jinyuanbaomall.cn/gttgytyjkg.html

Py:   "ab" * 3
来源：http://hz.yj202588.top/gtukkzqvts.html

PHP:  str_repeat("ab", 3);
来源：http://hz.iojbl.cn/gtclphpqyq.html

JS:   "ab".repeat(3)
来源：http://hz.fengsongda.top/gtmrknwlxo.html

TS:   "ab".repeat(3)
来源：http://hz.ivvv.top/gtrxnllwud.html

Java: "ab".repeat(3)
来源：http://hz.zhongyouzk.top/gtcpjlyaen.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.pycfn.com/gtjciitiuj.html

Ruby: "ab" * 3
来源：http://hz.dianchejie.cn/gtcurlatzy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xziqi.cn/gtoydxaauv.html

[E03] 截取子串
来源：http://hz.fengsongda.top/gtprvgvabz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yj20258.top/gtpguwpyqn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yvedp.cn/gtfakqxdht.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.c1oappe.top/gtmxqwazka.html

TS:   s.slice(1, 4)
来源：http://hz.andypj.xyz/gtdscldwmx.html

Java: s.substring(1, 4)
来源：http://hz.sysykeji.top/gtnlmfttnf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hywenlv.cn/gtffaaxrhb.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ppjwa.cn/gtigiivuwi.html

C#:   s.Substring(1, 3)
来源：http://hz.wangshuangyany.cn/gtbviygufk.html

[E04] 查找子串位置
来源：http://hz.yj20258888.top/gtyxboxfkt.html

Py:   s.find("x");  s.index("x")
来源：http://hz.nanxuanxn.top/gtfesbdqgc.html

PHP:  strpos($s, "x");
来源：http://hz.zhiwuduotai.top/gtbgzebetg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xziqi.cn/gtmukcxhvq.html

TS:   s.indexOf("x")
来源：http://hz.cdnleiting.top/gtsafhqbjj.html

Java: s.indexOf("x")
来源：http://hz.hywenlv.cn/gtruqdkyvy.html

Go:   strings.Index(s, "x")
来源：http://hz.fengsongda.top/gtimeynpvr.html

Ruby: s.index("x")
来源：http://hz.kuanghao11.cn/gtswbsmwse.html

C#:   s.IndexOf("x")
来源：http://hz.gaohongyu789.top/gtjggiqfpy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.shangyingyoupin.top/gtuukbbzvy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ywan-chungtsiang.top/gtwuknsyje.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.fzhhl.top/gtqumecgvl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.mhx1999.top/gtoxifnlmb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.quarkkingdee.top/gtiooejwsy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenjidiqi.icu/gtfbhbhiel.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hongshengwenyu.top/gtugdmujbi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gaohongyu789.top/gtgmxjedmq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xingfuxueyuan.xyz/gtgeuhabdd.html

[E06] 替换子串
来源：http://hz.shanyushiyangtech.top/gtitgwpari.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yuxming.cn/gtzzbudsmv.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ehwqpu.com/gtbkcqpuus.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ppjwa.cn/gttexuqxxy.html

TS:   s.replaceAll("a", "b")
来源：http://hz.nwbrower.top/gtignyanpp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhongyouzk.top/gtugirgomy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.dashuyun.cn/gtrttimvnv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.haohaochexian.top/gtwvhjiiuy.html

C#:   s.Replace("a", "b")
来源：http://hz.hnxiangtu.top/gtekvfwxrn.html

[E07] 按分隔符拆分
来源：http://hz.guannengcc.top/gtcqoehlfv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhongyouzk.top/gtijxqzudm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ywan-chungtsiang.top/gtrttglcwt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.nanxinkj.top/gtusbrcdoa.html

TS:   s.split(",")
来源：http://hz.yj20258888.top/gtlerwudxs.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.bjfxy.top/gtvazfttou.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhoulong.xyz/gtjnkektxt.html

Ruby: s.split(",");  s.split
来源：http://hz.nanxuanxn.top/gthllpizxq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.kuanghao11.cn/gtsvhhmhic.html

[E08] 数组按分隔符合并
来源：http://hz.yongpay.top/gtwvldjpnt.html

Py:   ",".join(items)
来源：http://hz.quarkkingdee.top/gtfoemryuy.html

PHP:  implode(",", $items);
来源：http://hz.havefunace.top/gteenlwtvb.html

JS:   items.join(",")
来源：http://hz.vqdsnc.cn/gtruclbxzw.html

TS:   items.join(",")
来源：http://hz.snrcjt.cn/gtvclgiwyc.html

Java: String.join(",", items)
来源：http://hz.iojbl.cn/gtnlxrmnpg.html

Go:   strings.Join(items, ",")
来源：http://hz.chenzaomai.com/gtlrnygqbg.html

Ruby: items.join(",")
来源：http://hz.yj202588.top/gtfhhtswuy.html

C#:   string.Join(",", items)
来源：http://hz.0kj1m.cn/gtolhcjuwr.html

[E09] 去除所有空白字符
来源：http://hz.zhixingplan.top/gteojhgypo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.wangdashe.top/gtzaknvtvs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yueranfly.top/gtewsoaokx.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cqqwz.cn/gtyhzpyyfi.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ydzc1.top/gtcalqsltp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hysaishi.cn/gtavhhpfpj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sweek.top/gtqfgrftsm.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.meibo888.top/gtzftekjpl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.shanyushiyangkeji.top/gtvlmnqmuw.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cheryme.top/gtqpaxecij.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhixingplan.top/gtjdxmkpqn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jianghu66.top/gtnkbyieto.html

JS:   "7".padStart(3, "0")
来源：http://hz.cdnleiting.top/gtsmhrohvj.html

TS:   "7".padStart(3, "0")
来源：http://hz.dianchejie.cn/gtoclhvcos.html

Java: String.format("%03d", 7)
来源：http://hz.shuidangran.top/gtwrvngidk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shuidangran.top/gtnclqjjrt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yuxming.cn/gtgqxrbtrc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhoulong.xyz/gtfqerjdpq.html

[E11] 反转字符串
来源：http://hz.yongpay.top/gtxxoznisp.html

Py:   s[::-1]
来源：http://hz.sweek.top/gtnbkgyphn.html

PHP:  strrev($s);
来源：http://hz.aizwys.cn/gtaxfjcxpd.html

JS:   [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtawusywkv.html

TS:   [...s].reverse().join("")
来源：http://hz.shuidangran.top/gtrvbfserb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.sufxvd.cn/gtfnplgjjt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yuanzhike.top/gtysfzquwi.html

Ruby: s.reverse
来源：http://hz.zycfv.cn/gtzrjrkjas.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yanxiufei.cn/gtgofuzcdo.html

[E12] 统计某字符出现次数
来源：http://hz.sysykeji.top/gtizujfvtj.html

Py:   s.count("a")
来源：http://hz.cdnleiting.top/gtpvhxofbm.html

PHP:  substr_count($s, "a");
来源：http://hz.gotoacloud.top/gtgncunjko.html

JS:   s.split("a").length - 1
来源：http://hz.hnxiangtu.top/gthxjofokc.html

TS:   s.split("a").length - 1
来源：http://hz.zhoulong.xyz/gtjkhtpdsf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.dashuyun.cn/gtcstritgp.html

Go:   strings.Count(s, "a")
来源：http://hz.smart0.xyz/gtcdmpmhgi.html

Ruby: s.count("a")
来源：http://hz.ydjk.org.cn/gtqftzkubd.html

C#:   s.Count(c => c == 'a')
来源：http://hz.mhx1999.top/gtzdxyzytl.html

[E13] 逐字符遍历
来源：http://hz.hysaishi.cn/gtyhfdxshc.html

Py:   for ch in s: print(ch)
来源：http://hz.jqgfzy.top/gtjdhgfghz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shangyingyoupin.top/gtkzuobfnv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuxming.cn/gtaxfpeuoj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangshuangyany.cn/gtfijmwqvo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.wangshuangyany.cn/gtlhaftmvc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.daria6918.cn/gtpssgwddk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xuanzx.com/gtemlsroyq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.0kj1m.cn/gtdzoyawqx.html

[E14] URL 编码与 Base64
来源：http://hz.havefunace.top/gtupotunzp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.chenlongwang.top/gtlmwxtdbu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.c1oappe.top/gtiabgauqz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shzxlz.cn/gtgcbrxjvx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yj20258888.top/gtjtjilexu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ppjwa.cn/gtuocfjist.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hongshengwenyu.top/gtstwgcbfw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ywan-chungtsiang.top/gtdjjsfudp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ivvv.top/gtensvkpfe.html

[E15] HTML 转义 / 反转义
来源：http://hz.aizwys.cn/gtkwkxgwzc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.52xcode.cn/gtdvkxuprt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sweek.top/gtgwamizwi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.9152youxi.cn/gtbuojqwnh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cdnleiting.top/gttncxivzc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.wangdashe.top/gtvnwnttkk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shzxlz.cn/gtjnozskge.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ivvv.top/gtmzjevyde.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.mhx1999.top/gtuptreuvu.html

[E16] 数字千分位
来源：http://hz.shanyushiyangkeji.top/gtjeufofnt.html

Py:   f"{1234567:,}"
来源：http://hz.zhixingplan.top/gtrlzaxguz.html

PHP:  number_format(1234567);
来源：http://hz.cqqwz.cn/gtjdltthqt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuanzhike.top/gtpxikwvgb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cheryme.top/gtqzvxpmos.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.haohaochexian.top/gthfnsmnqb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cucudq.cn/gtsmscypzc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jqgufenzy.top/gtoqkbsqfc.html

C#:   1234567.ToString("N0")
来源：http://hz.zhengqikj.top/gtbgpixprg.html

[E17] 首字母大写
来源：http://hz.chenjidiqi.icu/gtatmslple.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenlongwang.top/gtleiqflwg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xziqi.cn/gtobiaspni.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tianlin.xyz/gtglcfignq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258888.top/gtcutphkse.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sweek.top/gtisitvrll.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.daxiang520.top/gtvjqaxugr.html

Ruby: s.capitalize
来源：http://hz.shanyushiyangtech.top/gtpcduqgfo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yuanzhike.top/gtpwydjwcv.html

[E18] 模板占位符替换
来源：http://hz.xuetiantiany.cn/gtpiuyrfhy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jqgfzy.top/gttwxxiwkk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ybcxt.top/gtdgpwwjfe.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.pengpengdd.cyou/gtppkyyetd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zycfv.cn/gtijfyhzcw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yueranfly.top/gtjbwfrlwr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.9152youxi.cn/gtvpdipojt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.pycfn.com/gtjefqxjve.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.fengsongda.top/gtmaylqxxr.html

[E19] 多行文本按行拆分
来源：http://hz.shzxlz.cn/gtthkosdlz.html

Py:   s.splitlines()
来源：http://hz.c1oappe.top/gthltrxsjc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.guannengcc.top/gtultnbwjb.html

JS:   s.split(/\r?\n/)
来源：http://hz.hysaishi.cn/gtctcttfxh.html

TS:   s.split(/\r?\n/)
来源：http://hz.nwbrower.top/gtxgqmqbsh.html

Java: s.lines().toList()
来源：http://hz.jyoumei.cn/gthvclrjdo.html

Go:   strings.Split(s, "\n")
来源：http://hz.haohaochexian.top/gtfwmvlyfn.html

Ruby: s.lines
来源：http://hz.yvedp.cn/gtezqwozeh.html

C#:   s.Split('\n')
来源：http://hz.nwbrower.top/gtkfrvueiw.html

[E20] 判断字符串是否为空
来源：http://hz.316326.xyz/gtsafhplcq.html

Py:   if not s:
来源：http://hz.wangdashe.top/gthekxymtl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.chenlongwang.top/gtvqpeomps.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.havefunace.top/gtfmfuygvt.html

TS:   if (s === "") {}
来源：http://hz.yanxiufei.cn/gthkodqhtc.html

Java: if (s.isEmpty()) {}
来源：http://hz.yuanzhike.top/gtxrhqnfpt.html

Go:   if s == "" {}
来源：http://hz.chenjidiqi.icu/gtfwekuovc.html

Ruby: if s.empty?
来源：http://hz.zhixingplan.top/gtsgdtkhah.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jiagoushi.top/gtpdvlqboz.html

[E21] 超长截断加省略号
来源：http://hz.yj20258.top/gtcodpwori.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sysykeji.top/gtrjigbyiq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cashguo.top/gtbofyyiqc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.vqdsnc.cn/gtqhvtzpev.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jlsjyb.cn/gtpbjhmabl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinghuilouyu.cn/gthgnibsna.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.sufxvd.cn/gtwhkswmyk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtlxwvhkbf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.chenjidiqi.icu/gtxynvdeit.html

[E22] 字节长度与字符长度
来源：http://hz.hywenlv.cn/gtcivncaql.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.andypj.xyz/gtntnyizri.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hywenlv.cn/gtavnmhzua.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shangyingyoupin.top/gtsoxylski.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.bjfxy.top/gtzdjbflmh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ehwqpu.com/gtqzdrywiu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xziqi.cn/gtppssvqug.html

Ruby: s.bytesize;  s.length
来源：http://hz.svipenyu.cn/gtvrkmsndy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hnqzz.top/gtvybcnieh.html

================================================================================
来源：http://hz.yj202588.top/gtdllhgatu.html

F. 文件与目录
来源：http://hz.hongshengwenyu.top/gtdqblumlu.html

================================================================================
来源：http://hz.gzhubu.top/gtprfhsnlc.html

[F01] 读取整个文件
来源：http://hz.jinghuilouyu.cn/gtxkaavfpk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj20258888.top/gtyvplnlll.html

PHP:  file_get_contents("a.txt");
来源：http://hz.redwolf501.top/gtyjeytaoy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ybcxt.top/gtczhgmwfe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.bjfxy.top/gtnjqqogca.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.kuanghao11.cn/gtxcnrzphn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jqgufenzy.top/gtuoqsqrkk.html

Ruby: File.read("a.txt")
来源：http://hz.zhiwuduotai.top/gtqgprupev.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.guowangkeji.top/gtpwshsdng.html

[F02] 逐行读取文件
来源：http://hz.hongshengwenyu.top/gtzfgqcxyx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yangfankeji.com/gtyceejoyu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shanyushiyangkeji.top/gtsmpgayzt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yvedp.cn/gtoygjqyxf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.andypj.xyz/gtfnoahapw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xylfe.cn/gtxsdafpgp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.pengpengdd.cyou/gtwneziihb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.havefunace.top/gthbdzywmu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.316326.xyz/gtkpxhajcb.html

[F03] 写入文件（覆盖）
来源：http://hz.yuanzhike.top/gtzbiugywn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gotoacloud.top/gtspohltcx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shuidangran.top/gtuopmrmsi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.wangshuangyany.cn/gtomclxklj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinghuilouyu.cn/gtvdipnejz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.wangshuangyany.cn/gtpmoihfkz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shuidangran.top/gtzpjwqfmo.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cqqwz.cn/gtlnibpilm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.chenzaomai.com/gtxmeusfnx.html

[F04] 追加写入文件
来源：http://hz.zhijiandao.cn/gtmjstshgx.html


<!-- 参考信息 -->