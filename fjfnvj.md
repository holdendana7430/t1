代发 wailian999

[D19] 按字段分组
来源：http://hz.cucudq.cn/gtnjwuyimp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.daria6918.cn/gtwtiarnsa.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hywenlv.cn/gtwvnodyba.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.gaohongyu789.top/gtjzbgphmr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xziqi.cn/gtueaztkuu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yangfankeji.com/gtoccgyomj.html

Go:   // 手写 map[string][]T
来源：http://hz.cqqwz.cn/gtkbhzevqf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gogol.net.cn/gtehihccja.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gzhubu.top/gteffbhmmf.html

[D20] 统计每个元素出现次数
来源：http://hz.xziqi.cn/gtiovyzaoy.html

Py:   Counter(arr)
来源：http://hz.redwolf501.top/gtlqaopmxb.html

PHP:  array_count_values($arr);
来源：http://hz.sxryk.cn/gtypcfeeic.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gaohongyu789.top/gtahlpldtp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yangfankeji.com/gtobneyoxt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ivvv.top/gtnkhaghnr.html

Go:   // 手写 map[T]int
来源：http://hz.hfpthk.cn/gtywbaslbc.html

Ruby: arr.tally
来源：http://hz.zhaomingkeji.xyz/gtcztotpab.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yuxming.cn/gtjmuwcalr.html

[D21] 判断是否包含某元素
来源：http://hz.ydzc1.top/gtopaibeev.html

Py:   x in arr
来源：http://hz.cdnleiting.top/gthsdzradq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.nanxuanxn.top/gtxywrhkfn.html

JS:   arr.includes(x)
来源：http://hz.jianghu66.top/gtlxtbxqlq.html

TS:   arr.includes(x)
来源：http://hz.cdnleiting.top/gtetddbwyk.html

Java: list.contains(x)
来源：http://hz.zhengqikj.top/gtfxyymxdc.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhiwuduotai.top/gtulyufoiu.html

Ruby: arr.include?(x)
来源：http://hz.gzhubu.top/gtjfchgpht.html

C#:   list.Contains(x)
来源：http://hz.xuanzx.com/gtsadspcdl.html

[D22] 复制数组（避免共享引用）
来源：http://hz.gotoacloud.top/gtygewjgzl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.aizwys.cn/gtjypmcmox.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xuetiantiany.cn/gtqsjyafar.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.nanxinkj.top/gtjbkxkblk.html

TS:   [...arr];
来源：http://hz.jinqigufen.top/gtqbcgidcc.html

Java: new ArrayList<>(list);
来源：http://hz.wangdashe.top/gtbkvylfll.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.chenzaomai.com/gtmbaeloqc.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jiagoushi.top/gtuxeoinmk.html

C#:   new List<int>(list);
来源：http://hz.zhengqikj.top/gtdhtadtfi.html

[D23] reduce 累积计算
来源：http://hz.zhoulong.xyz/gtjgryqomi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.tanke756.top/gtmwklydgf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.shuidangran.top/gtktemhebi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cucudq.cn/gtjkqbeour.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.haohaochexian.top/gtzzbljxfg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zycfv.cn/gttzswcfyg.html

Go:   // 手写循环
来源：http://hz.chenlongwang.top/gtkukgizml.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.dianchejie.cn/gtoiepimab.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cheryme.top/gtyxxdfxpy.html

[D24] 字典 / Map 基本操作
来源：http://hz.ydzc1.top/gtqolqfeho.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hnxiangtu.top/gtpswqglfz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.fzhhl.top/gttfszichv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.guowangkeji.top/gtdfgrgjac.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.tanke756.top/gturfrwffd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nanxuanxn.top/gtwarctlrg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shanyushiyangkeji.top/gtfcbllxyf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.havefunace.top/gtutfxsrty.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xylfe.cn/gtwlffozyp.html

[D25] Set 集合去重与交并差
来源：http://hz.yangfankeji.com/gtcabatpra.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.pycfn.com/gtanjqqpru.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.haohaochexian.top/gtlsorxvdo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.svipenyu.cn/gtaaaxxsio.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hammf.cn/gtnrrkklti.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ehwqpu.com/gtlqclkdqq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ehwqpu.com/gtvdghkkku.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.chenlongwang.top/gtbeooigau.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.mhx1999.top/gtahhsvdfm.html

[D26] 数组转字符串
来源：http://hz.havefunace.top/gtvvfhlrcs.html

Py:   ", ".join(map(str, arr))
来源：http://hz.andypj.xyz/gtbaqvhohy.html

PHP:  implode(", ", $arr);
来源：http://hz.shzxlz.cn/gtpzaqwhov.html

JS:   arr.join(", ")
来源：http://hz.nwbrower.top/gtcxglkeay.html

TS:   arr.join(", ")
来源：http://hz.jianghu66.top/gtoilgkqct.html

Java: String.join(", ", list)
来源：http://hz.cqqwz.cn/gtbwpkoxhd.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhiwuduotai.top/gtbvrgdnpf.html

Ruby: arr.join(", ")
来源：http://hz.yueranfly.top/gtlfktlpgw.html

C#:   string.Join(", ", list)
来源：http://hz.hfpthk.cn/gtbrzamygk.html

================================================================================
来源：http://hz.yuxming.cn/gtuhnrxwts.html

E. 字符串处理
来源：http://hz.jianghu66.top/gtllnlhihx.html

================================================================================
来源：http://hz.redwolf501.top/gtgtsfxezk.html

[E01] 拼接字符串
来源：http://hz.meibo888.top/gtdxmzsmeo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.nwbrower.top/gtnwkzggef.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jinqigufen.top/gtcpghylwl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.iojbl.cn/gtwfkopdfg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guannengcc.top/gtxyjbwfbc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jinqigfzy.top/gtzhqieemj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.nanxuanxn.top/gtjdryqdnd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.andypj.xyz/gtxkhlftmd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hongshengwenyu.top/gtnfmnfwnh.html

[E02] 重复字符串
来源：http://hz.snrcjt.cn/gthlfwguhg.html

Py:   "ab" * 3
来源：http://hz.xinyue.icu/gtwsitatty.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hammf.cn/gtzuqjfepy.html

JS:   "ab".repeat(3)
来源：http://hz.nanxuanxn.top/gtmhqgmsqd.html

TS:   "ab".repeat(3)
来源：http://hz.jinghuilouyu.cn/gtwloptvna.html

Java: "ab".repeat(3)
来源：http://hz.xylfe.cn/gtpdnqhrpr.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xylfe.cn/gtblfmccvd.html

Ruby: "ab" * 3
来源：http://hz.nanxinkj.top/gtgxzeaiya.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.52xcode.cn/gthodekwkz.html

[E03] 截取子串
来源：http://hz.nanxuanxn.top/gtkluyvtxv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zdqjudy.top/gtsdvtmrbp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ydzc1.top/gtzrnovfmm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhengqikj.top/gtpsvxomxm.html

TS:   s.slice(1, 4)
来源：http://hz.jinghuilouyu.cn/gtmcfdniqg.html

Java: s.substring(1, 4)
来源：http://hz.0kj1m.cn/gtlsghdkvr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ywan-chungtsiang.top/gtciecxzzm.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hysaishi.cn/gtsgkszvqs.html

C#:   s.Substring(1, 3)
来源：http://hz.ywan-chungtsiang.top/gtarrwytog.html

[E04] 查找子串位置
来源：http://hz.nwbrower.top/gtlfckyxju.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cashguo.top/gtqkjhmzpx.html

PHP:  strpos($s, "x");
来源：http://hz.ydzc1.top/gtupzfofrk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yj20258888.top/gtmnuqwttx.html

TS:   s.indexOf("x")
来源：http://hz.gotoacloud.top/gtvavpzozi.html

Java: s.indexOf("x")
来源：http://hz.mhx1999.top/gtupkmhbfx.html

Go:   strings.Index(s, "x")
来源：http://hz.yj202588.top/gtpycfowpo.html

Ruby: s.index("x")
来源：http://hz.feifeiyinyue.top/gtvqlilryn.html

C#:   s.IndexOf("x")
来源：http://hz.xingfuxueyuan.xyz/gtkxkxfgcv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yj202588.top/gtbdxmhzns.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.c1oappe.top/gtddcvrdcl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shangyingyoupin.top/gtmtvqreie.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hnqzz.top/gtsszuipzn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.gotoacloud.top/gtgvsxbxdw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shanyushiyangkeji.top/gtrtmnotge.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ivvv.top/gtcvrdebiv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xylfe.cn/gtvoknoccw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.vqdsnc.cn/gtajbzhmep.html

[E06] 替换子串
来源：http://hz.yj202588.top/gtxdryswpv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xylfe.cn/gtgjpceozx.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shanyushiyangtech.top/gtrakigoet.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yuxming.cn/gtfhaawxjj.html

TS:   s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtbqcyoyll.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yuxming.cn/gtnrirbqny.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.kuanghao11.cn/gtdckadjpe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ydzc1.top/gtsperyhql.html

C#:   s.Replace("a", "b")
来源：http://hz.fzhhl.top/gtnffzjneg.html

[E07] 按分隔符拆分
来源：http://hz.meibo888.top/gtjnbttoiv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.tanke756.top/gtaalxziop.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zycfv.cn/gtkbuecout.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhijiandao.cn/gttfulsuiv.html

TS:   s.split(",")
来源：http://hz.zhengqikj.top/gtudpjfyrm.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.daria6918.cn/gtawlmzrow.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ivvv.top/gtildcezqm.html

Ruby: s.split(",");  s.split
来源：http://hz.kuanghao11.cn/gtkjtfxems.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.vqdsnc.cn/gttaxmocwi.html

[E08] 数组按分隔符合并
来源：http://hz.ivvv.top/gthyddddgc.html

Py:   ",".join(items)
来源：http://hz.xingfuxueyuan.xyz/gtigaiuxsa.html

PHP:  implode(",", $items);
来源：http://hz.wangdashe.top/gtdcmuycaq.html

JS:   items.join(",")
来源：http://hz.ivvv.top/gtiyrkzpit.html

TS:   items.join(",")
来源：http://hz.zhengqikj.top/gtwaqzfruj.html

Java: String.join(",", items)
来源：http://hz.chenlongwang.top/gtvhtriuzx.html

Go:   strings.Join(items, ",")
来源：http://hz.mhx1999.top/gtpejmrwkk.html

Ruby: items.join(",")
来源：http://hz.xinyue.icu/gtawuoqnez.html

C#:   string.Join(",", items)
来源：http://hz.cucudq.cn/gthuchpraz.html

[E09] 去除所有空白字符
来源：http://hz.hnxiangtu.top/gtmwfcqgbj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.daxiang520.top/gttfzthawn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.nanxuanxn.top/gtoeyqthcr.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yueranfly.top/gtpmokrcje.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hywenlv.cn/gtfknlvspt.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhixingplan.top/gthqpsqnnm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.gzhubu.top/gtobeeclmf.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yuanzhike.top/gtgkimdtlv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ehwqpu.com/gtappsbeqn.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhaomingkeji.xyz/gtilpwirrs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.iojbl.cn/gtqyuyxqup.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.shuidangran.top/gtrxniyrmt.html

JS:   "7".padStart(3, "0")
来源：http://hz.yonumen.top/gtnytiukbo.html

TS:   "7".padStart(3, "0")
来源：http://hz.ppjwa.cn/gtotwyqgie.html

Java: String.format("%03d", 7)
来源：http://hz.yvedp.cn/gtrbyfnbsw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yueranfly.top/gtkadjkoan.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sxryk.cn/gtxwbzzrew.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cashguo.top/gteemnoyhu.html

[E11] 反转字符串
来源：http://hz.9152youxi.cn/gtbhqflslt.html

Py:   s[::-1]
来源：http://hz.gogol.net.cn/gtjprayhey.html

PHP:  strrev($s);
来源：http://hz.pengpengdd.cyou/gtybgtmhjx.html

JS:   [...s].reverse().join("")
来源：http://hz.xylfe.cn/gtglmcockf.html

TS:   [...s].reverse().join("")
来源：http://hz.yvedp.cn/gtpuopxshs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinqigufen.top/gtmplukzon.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.cashguo.top/gtklfzeyip.html

Ruby: s.reverse
来源：http://hz.gotoacloud.top/gtcrvepkkm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.smart0.xyz/gtkxzpfaza.html

[E12] 统计某字符出现次数
来源：http://hz.pycfn.com/gttcatsrmu.html

Py:   s.count("a")
来源：http://hz.hnxiangtu.top/gtcvyennvu.html

PHP:  substr_count($s, "a");
来源：http://hz.dianchejie.cn/gtpvcossdf.html

JS:   s.split("a").length - 1
来源：http://hz.zhongyouzk.top/gtgidyiyqd.html

TS:   s.split("a").length - 1
来源：http://hz.aizwys.cn/gtlxhpafar.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.52xcode.cn/gtrtdywsbn.html

Go:   strings.Count(s, "a")
来源：http://hz.zhaomingkeji.xyz/gtkcpijugv.html

Ruby: s.count("a")
来源：http://hz.zhixingplan.top/gtlvqzcuhm.html

C#:   s.Count(c => c == 'a')
来源：http://hz.dashuyun.cn/gtfdiblcic.html

[E13] 逐字符遍历
来源：http://hz.yvedp.cn/gtwavpylva.html

Py:   for ch in s: print(ch)
来源：http://hz.chenjidiqi.icu/gtguxcnxmt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ehwqpu.com/gtwafouuwx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.mhx1999.top/gtdbdiknni.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhongyouzk.top/gtcegokxor.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yongpay.top/gtinoqhqsn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.aibaodan.cn/gtrqtcwpzv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.9152youxi.cn/gtgjscseiz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yvedp.cn/gtlhnysuas.html

[E14] URL 编码与 Base64
来源：http://hz.ydzc1.top/gtpqaacdyt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.fzhhl.top/gtovaglcsz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jqgfzy.top/gtnfgaappd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.sufxvd.cn/gtkpfydves.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.c1oappe.top/gtqvbqjcif.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xylfe.cn/gtwhyckqzd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.guannengcc.top/gtkzeaoslj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xuanzx.com/gtdthyluhi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.mhx1999.top/gtzpjpsytq.html

[E15] HTML 转义 / 反转义
来源：http://hz.chenlongwang.top/gtfgehzoop.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shanyushiyangkeji.top/gtzmeatlic.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.dashuyun.cn/gtcevhrfib.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ppjwa.cn/gtqmlrwcam.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cdnleiting.top/gtoyvedhyk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.meibo888.top/gtukvxnmbl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shzxlz.cn/gtqomiiezy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhoulong.xyz/gtilslpdzf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.cheryme.top/gtwiqqwntz.html

[E16] 数字千分位
来源：http://hz.quarkkingdee.top/gtyyjwxake.html

Py:   f"{1234567:,}"
来源：http://hz.shuidangran.top/gtjrwytkty.html

PHP:  number_format(1234567);
来源：http://hz.hammf.cn/gttabjdfqu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sufxvd.cn/gtykjykfwu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnxiangtu.top/gtihekhaxq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shanyushiyangkeji.top/gtryyhpxku.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.bjfxy.top/gtgdypqzps.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gzhubu.top/gtrkuzoryk.html

C#:   1234567.ToString("N0")
来源：http://hz.shanyushiyangtech.top/gtbjkcbkjx.html

[E17] 首字母大写
来源：http://hz.nanxuanxn.top/gtdsdzdgmr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.wangdashe.top/gtutmfyedj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.iojbl.cn/gtmzmxbewo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.snrcjt.cn/gtmnmdaglw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gogol.net.cn/gtrgfahdrm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.quarkkingdee.top/gtbyfgbbqd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ehwqpu.com/gtwgvbexcd.html

Ruby: s.capitalize
来源：http://hz.zhixingplan.top/gthfuvkqtx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yj20258888.top/gtlatxvmlk.html

[E18] 模板占位符替换
来源：http://hz.fengsongda.top/gtcmhmjntv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhoulong.xyz/gtkrsgenqp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yanxiufei.cn/gtusgasdcr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hongshengwenyu.top/gtaqigmhlw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhijiandao.cn/gtyyaxcewk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yvedp.cn/gtyxmyiucu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.nanxuanxn.top/gtxmekdenf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.chenjidiqi.icu/gtdkszmlkj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sxryk.cn/gtazukehcx.html

[E19] 多行文本按行拆分
来源：http://hz.xziqi.cn/gtmrrvjyhy.html

Py:   s.splitlines()
来源：http://hz.xingfuxueyuan.xyz/gtecveadhv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.feifeiyinyue.top/gtncceropj.html

JS:   s.split(/\r?\n/)
来源：http://hz.gaohongyu789.top/gtzpozfjfe.html

TS:   s.split(/\r?\n/)
来源：http://hz.ybcxt.top/gtippjjiuy.html

Java: s.lines().toList()
来源：http://hz.mhx1999.top/gtosovdkxh.html

Go:   strings.Split(s, "\n")
来源：http://hz.xziqi.cn/gtmtdmyzgx.html

Ruby: s.lines
来源：http://hz.jyoumei.cn/gtnycietze.html

C#:   s.Split('\n')
来源：http://hz.nwbrower.top/gtxmuubdej.html

[E20] 判断字符串是否为空
来源：http://hz.snrcjt.cn/gtzarzmirq.html

Py:   if not s:
来源：http://hz.redwolf501.top/gtvhtbxyzq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.nanxinkj.top/gtbmfsucgp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhoulong.xyz/gtthwiaaus.html

TS:   if (s === "") {}
来源：http://hz.sxryk.cn/gtyxdeslaj.html

Java: if (s.isEmpty()) {}
来源：http://hz.zycfv.cn/gtegasfaml.html

Go:   if s == "" {}
来源：http://hz.jinqigufen.top/gtjslekxqc.html

Ruby: if s.empty?
来源：http://hz.jiagoushi.top/gteiuopmfb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.bjfxy.top/gtdhxorgqr.html

[E21] 超长截断加省略号
来源：http://hz.zhixingplan.top/gtgzqqirhk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yueranfly.top/gtumcouexo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.iojbl.cn/gtswnrgmqf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtlbizrfam.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.bjfxy.top/gtovdrvsnx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yongpay.top/gtvjlycwyf.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.chenzaomai.com/gtackueqar.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.sxryk.cn/gtbxbtwech.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jyoumei.cn/gtbholgqmh.html

[E22] 字节长度与字符长度
来源：http://hz.ywan-chungtsiang.top/gtumlxrhsx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hnxiangtu.top/gtfyqnzprd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtchhvtfxb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cucudq.cn/gtvqfgykik.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dashuyun.cn/gtauvmjqis.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.52xcode.cn/gtldtdqdll.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.feifeiyinyue.top/gtqihbscot.html

Ruby: s.bytesize;  s.length
来源：http://hz.guowangkeji.top/gtsxjltzvr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.chenzaomai.com/gtdmtnjxvo.html

================================================================================
来源：http://hz.cheryme.top/gtkdhfejxs.html

F. 文件与目录
来源：http://hz.zhaomingkeji.xyz/gtqoioxjcb.html

================================================================================
来源：http://hz.dianchejie.cn/gtcqvmypgs.html

[F01] 读取整个文件
来源：http://hz.feifeiyinyue.top/gtpymaokuo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.pycfn.com/gtupuxdkkr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.redwolf501.top/gtbaoryekz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jiagoushi.top/gtinenqruz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.cdnleiting.top/gtsrjbtfkb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gtmykqtixy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.9152youxi.cn/gtcafuscpl.html

Ruby: File.read("a.txt")
来源：http://hz.zhixingplan.top/gtncullnus.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.tian-w.cn/gtzxktepvk.html

[F02] 逐行读取文件
来源：http://hz.chenlongwang.top/gtsrugarup.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.wangshuangyany.cn/gtrosjkqyj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhaomingkeji.xyz/gtsopfzhuf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenzaomai.com/gtwhgxkjvd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yanxiufei.cn/gtylhakddu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jyoumei.cn/gtjaemoogv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.chenjidiqi.icu/gtmfqzilqn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.bjfxy.top/gtvnmmwbkn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ydzc1.top/gtocbauuow.html

[F03] 写入文件（覆盖）
来源：http://hz.xingfuxueyuan.xyz/gtjomwoxiu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gotoacloud.top/gtjckoqdjn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.chenjidiqi.icu/gtbzyvbfcu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.dianchejie.cn/gtstdcgeid.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guannengcc.top/gtjrzccrju.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.bjfxy.top/gtapgsgmmh.html


<!-- 参考信息 -->