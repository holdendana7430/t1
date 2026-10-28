代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ywan-chungtsiang.top/gtdlckddfx.html

C#:   list.Sum();  list.Average()
来源：http://hz.cashguo.top/gtjxktutng.html

[D17] 最大值与最小值
来源：http://hz.dashuyun.cn/gtpcpbwodd.html

Py:   max(arr);  min(arr)
来源：http://hz.andypj.xyz/gtgrdyexjg.html

PHP:  max($arr);  min($arr);
来源：http://hz.wangshuangyany.cn/gtvofpbwfg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.iojbl.cn/gtzfixzgro.html

TS:   Math.max(...arr);
来源：http://hz.sufxvd.cn/gtidcffyxt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.havefunace.top/gtrlvqbdyp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhaomingkeji.xyz/gtsandfeqa.html

Ruby: arr.max;  arr.min
来源：http://hz.guannengcc.top/gtsmvanwkv.html

C#:   list.Max();  list.Min()
来源：http://hz.sysykeji.top/gtokafbzsd.html

[D18] 扁平化嵌套数组
来源：http://hz.yongpay.top/gtmjokdzat.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jqgufenzy.top/gtkakvhzwt.html

PHP:  array_merge(...$nested);
来源：http://hz.yanxiufei.cn/gtqvwmeeci.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.bjfxy.top/gthzoszqho.html

TS:   nested.flat();
来源：http://hz.xuetiantiany.cn/gtnihznody.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.feifeiyinyue.top/gtpzlkysmv.html

Go:   // 手写双层循环
来源：http://hz.jlsjyb.cn/gtubjmesro.html

Ruby: nested.flatten
来源：http://hz.shuidangran.top/gtyfdlygdf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yvedp.cn/gtpziknuoz.html

[D19] 按字段分组
来源：http://hz.xuetiantiany.cn/gtjirxlwxw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ywan-chungtsiang.top/gthapkjgdz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yonumen.top/gtvkjwfnhh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hnxiangtu.top/gtenamgmcj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gaohongyu789.top/gtbblszrcy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.dianchejie.cn/gtbewgnoxi.html

Go:   // 手写 map[string][]T
来源：http://hz.tianlin.xyz/gtfvbvkzcs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.mhx1999.top/gtwkgygxvm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gzhubu.top/gtycwkgqus.html

[D20] 统计每个元素出现次数
来源：http://hz.yj20258888.top/gtbniswqkm.html

Py:   Counter(arr)
来源：http://hz.jinqigufen.top/gtxprqgbvy.html

PHP:  array_count_values($arr);
来源：http://hz.yueranfly.top/gtktpueryd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fzhhl.top/gtselhvkyp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenzaomai.com/gtjjmdfjrj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zycfv.cn/gtdmyziqqo.html

Go:   // 手写 map[T]int
来源：http://hz.cdnleiting.top/gtggjcbmom.html

Ruby: arr.tally
来源：http://hz.sweek.top/gtrezkqidz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.bjfxy.top/gtbqrwnuil.html

[D21] 判断是否包含某元素
来源：http://hz.jqgfzy.top/gtgvhebfti.html

Py:   x in arr
来源：http://hz.guannengcc.top/gtmcthqgrx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jinqigfzy.top/gtyyjnryyf.html

JS:   arr.includes(x)
来源：http://hz.hysaishi.cn/gtdmdjrdzg.html

TS:   arr.includes(x)
来源：http://hz.guannengcc.top/gtwoihxkkt.html

Java: list.contains(x)
来源：http://hz.guowangkeji.top/gtvztzjvpy.html

Go:   slices.Contains(arr, x)
来源：http://hz.tian-w.cn/gttjylzxqk.html

Ruby: arr.include?(x)
来源：http://hz.ywan-chungtsiang.top/gtnyextlpz.html

C#:   list.Contains(x)
来源：http://hz.yuxming.cn/gtnhzwpggw.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shangyingyoupin.top/gtftkubjaw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.kuanghao11.cn/gtrjxjnioo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhongyouzk.top/gtehnjuffo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xuanzx.com/gtjlhrlilw.html

TS:   [...arr];
来源：http://hz.hnqzz.top/gtfzgnkmkk.html

Java: new ArrayList<>(list);
来源：http://hz.shanyushiyangtech.top/gtdwsrudsk.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hfpthk.cn/gtpmicfuuy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sysykeji.top/gtbrunpryb.html

C#:   new List<int>(list);
来源：http://hz.dashuyun.cn/gtsydyszny.html

[D23] reduce 累积计算
来源：http://hz.kuanghao11.cn/gtqgxgdylm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.gotoacloud.top/gtjfalpjpj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhijiandao.cn/gtashmwofy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jyoumei.cn/gttjffcdpd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ywan-chungtsiang.top/gtdrbhzarw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.52xcode.cn/gtnvcfshqk.html

Go:   // 手写循环
来源：http://hz.cucudq.cn/gtgywwzshh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.daxiang520.top/gtezmdhgfu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yuxming.cn/gtlgohdpag.html

[D24] 字典 / Map 基本操作
来源：http://hz.yj20258888.top/gtqgejtgnw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.chenjidiqi.icu/gtweegwgir.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.kuanghao11.cn/gttztehjdq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.wangshuangyany.cn/gtstjigrlz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.wangdashe.top/gtsnrmfvkl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yvedp.cn/gtsmvsuqsx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xinyue.icu/gtqyaubkue.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.fzhhl.top/gtctvigsrs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.pengpengdd.cyou/gtwmrgasep.html

[D25] Set 集合去重与交并差
来源：http://hz.tanke756.top/gtsdexijhz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yj202588.top/gtwlualahy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.0kj1m.cn/gtjqfkxnvs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.316326.xyz/gtkfckkjfv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhijiandao.cn/gtbxfdjebf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.smart0.xyz/gtvbmwoxzh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yueranfly.top/gtumymaeaf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ivvv.top/gtwcqgwejk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.wangshuangyany.cn/gtyokhdjjz.html

[D26] 数组转字符串
来源：http://hz.kuanghao11.cn/gtqeddzjwg.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xziqi.cn/gtaosipdzg.html

PHP:  implode(", ", $arr);
来源：http://hz.pycfn.com/gtkrqhneaa.html

JS:   arr.join(", ")
来源：http://hz.birdmap.top/gtlsiyinsj.html

TS:   arr.join(", ")
来源：http://hz.sxryk.cn/gtwfbuthmp.html

Java: String.join(", ", list)
来源：http://hz.zhijiandao.cn/gtcouizrmh.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yuanzhike.top/gttswedxxy.html

Ruby: arr.join(", ")
来源：http://hz.aizwys.cn/gtocbrkswn.html

C#:   string.Join(", ", list)
来源：http://hz.xinyue.icu/gtxyjykyfx.html

================================================================================
来源：http://hz.nanxinkj.top/gtdawaqwqi.html

E. 字符串处理
来源：http://hz.shangyingyoupin.top/gtpyhullzv.html

================================================================================
来源：http://hz.zhongyouzk.top/gtomtfypsd.html

[E01] 拼接字符串
来源：http://hz.yonumen.top/gtzlveviyq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cheryme.top/gtezgmrgsf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.gogol.net.cn/gtevezkjtz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhixingplan.top/gtqgpwavtp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuxming.cn/gtuxuoygit.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ehwqpu.com/gtkdfghwqj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenjidiqi.icu/gtnrrjvvmx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.daria6918.cn/gtjkrueafa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cashguo.top/gtlccviwjt.html

[E02] 重复字符串
来源：http://hz.jiagoushi.top/gtqpimhpyo.html

Py:   "ab" * 3
来源：http://hz.shzxlz.cn/gtmoiskdlv.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yj20258888.top/gtbbtgrzea.html

JS:   "ab".repeat(3)
来源：http://hz.yangfankeji.com/gtmbkaddow.html

TS:   "ab".repeat(3)
来源：http://hz.ehwqpu.com/gtdpintdnj.html

Java: "ab".repeat(3)
来源：http://hz.0kj1m.cn/gtipciatwf.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cashguo.top/gtikixqayo.html

Ruby: "ab" * 3
来源：http://hz.wangshuangyany.cn/gtekwgwbto.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yuanzhike.top/gtukxmhfey.html

[E03] 截取子串
来源：http://hz.wangdashe.top/gtfbkkipwm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.tianlin.xyz/gtlldqlgso.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xinyue.icu/gtgwlgcmzh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cheryme.top/gtzjhnbodt.html

TS:   s.slice(1, 4)
来源：http://hz.ybcxt.top/gthwtdtqoz.html

Java: s.substring(1, 4)
来源：http://hz.xuanzx.com/gtsravafrd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yonumen.top/gtuftykzao.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jinyuanbaomall.cn/gthhsfulyd.html

C#:   s.Substring(1, 3)
来源：http://hz.yuanzhike.top/gtdqkulxxm.html

[E04] 查找子串位置
来源：http://hz.cucudq.cn/gtfywoprjo.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xylfe.cn/gtxarnxjvn.html

PHP:  strpos($s, "x");
来源：http://hz.gzhubu.top/gtxuzvnbxz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.vqdsnc.cn/gtiqjvnwub.html

TS:   s.indexOf("x")
来源：http://hz.shuidangran.top/gtdzjabjku.html

Java: s.indexOf("x")
来源：http://hz.shanyushiyangkeji.top/gtflznmnsl.html

Go:   strings.Index(s, "x")
来源：http://hz.cashguo.top/gtmecsdbxd.html

Ruby: s.index("x")
来源：http://hz.aibaodan.cn/gtkwavqcnb.html

C#:   s.IndexOf("x")
来源：http://hz.jqgufenzy.top/gtxteuuwdq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yvedp.cn/gtjsgyfqxq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shangyingyoupin.top/gtatfpipyw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.svipenyu.cn/gtnwqdspiq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jianghu66.top/gtxtsxawcd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yueranfly.top/gtqqlfiges.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yangfankeji.com/gtvzgovxxc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hnqzz.top/gtzzejghzk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.birdmap.top/gtdxtncwot.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jlsjyb.cn/gtnunkowxu.html

[E06] 替换子串
来源：http://hz.sysykeji.top/gtgacwipeu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ivvv.top/gtxfnvbput.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yongpay.top/gtlpwhxigb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hysaishi.cn/gtokbzbvnc.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cashguo.top/gtqcnclppn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sysykeji.top/gtsotjoxit.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.guowangkeji.top/gtsupclfpu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.aibaodan.cn/gtvuhogbtf.html

C#:   s.Replace("a", "b")
来源：http://hz.iojbl.cn/gtdiluroun.html

[E07] 按分隔符拆分
来源：http://hz.haohaochexian.top/gtmsvreyyf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.cucudq.cn/gteylkmsrw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.gogol.net.cn/gteeaxkliw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xinyue.icu/gtujxehrvr.html

TS:   s.split(",")
来源：http://hz.meibo888.top/gtonfsfxce.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.c1oappe.top/gtvlpnnijq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jinyuanbaomall.cn/gtczdsqgnr.html

Ruby: s.split(",");  s.split
来源：http://hz.zhengqikj.top/gtctzaiatl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.0kj1m.cn/gtfodtmpiz.html

[E08] 数组按分隔符合并
来源：http://hz.zhengqikj.top/gtarwistch.html

Py:   ",".join(items)
来源：http://hz.jianghu66.top/gtnlkbkvkb.html

PHP:  implode(",", $items);
来源：http://hz.shanyushiyangtech.top/gtogukbyze.html

JS:   items.join(",")
来源：http://hz.yueranfly.top/gtnwgrgwuo.html

TS:   items.join(",")
来源：http://hz.52xcode.cn/gtomwhbubb.html

Java: String.join(",", items)
来源：http://hz.gzhubu.top/gtkjkcuacp.html

Go:   strings.Join(items, ",")
来源：http://hz.yuxming.cn/gtguyluobm.html

Ruby: items.join(",")
来源：http://hz.feifeiyinyue.top/gtodboggoz.html

C#:   string.Join(",", items)
来源：http://hz.iojbl.cn/gtqonhwdof.html

[E09] 去除所有空白字符
来源：http://hz.jiagoushi.top/gttuuotbmw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.sweek.top/gtijggfesm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yvedp.cn/gtyiwnlzqj.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.guannengcc.top/gtdvbehwck.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yj20258.top/gtsqbhobzn.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.feifeiyinyue.top/gttnrxdwry.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.gogol.net.cn/gtyajuixqm.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hnxiangtu.top/gtzyabmbwh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cdnleiting.top/gtrqkxkpwh.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jqgufenzy.top/gtivkbdrah.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.pengpengdd.cyou/gteuinoffp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.haohaochexian.top/gtinqyxrks.html

JS:   "7".padStart(3, "0")
来源：http://hz.cheryme.top/gtpbpktrwu.html

TS:   "7".padStart(3, "0")
来源：http://hz.yj20258.top/gtlwawxfmh.html

Java: String.format("%03d", 7)
来源：http://hz.chenlongwang.top/gtdbpdwjrv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.9152youxi.cn/gtxeeodxgs.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ydzc1.top/gtzyitzkyk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenlongwang.top/gtpkuplike.html

[E11] 反转字符串
来源：http://hz.dashuyun.cn/gtgndoswzg.html

Py:   s[::-1]
来源：http://hz.yangfankeji.com/gtqvdafwnt.html

PHP:  strrev($s);
来源：http://hz.nanxuanxn.top/gtwvtuwpcs.html

JS:   [...s].reverse().join("")
来源：http://hz.tanke756.top/gtkyvklbut.html

TS:   [...s].reverse().join("")
来源：http://hz.yj202588.top/gtvrwogtjq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ydjk.org.cn/gtqlzxtuty.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sufxvd.cn/gtbxirkdrr.html

Ruby: s.reverse
来源：http://hz.zhongyouzk.top/gtumwwybsn.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cqqwz.cn/gtlshunrrc.html

[E12] 统计某字符出现次数
来源：http://hz.ybcxt.top/gtrccqhhtj.html

Py:   s.count("a")
来源：http://hz.nanxuanxn.top/gtscaygpah.html

PHP:  substr_count($s, "a");
来源：http://hz.ydjk.org.cn/gtenvqlcsd.html

JS:   s.split("a").length - 1
来源：http://hz.cucudq.cn/gtjgwgaged.html

TS:   s.split("a").length - 1
来源：http://hz.aizwys.cn/gtvtujnlys.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhoulong.xyz/gtabmuxuvm.html

Go:   strings.Count(s, "a")
来源：http://hz.sufxvd.cn/gtesxcxoaq.html

Ruby: s.count("a")
来源：http://hz.jinqigfzy.top/gtfakusltx.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hywenlv.cn/gtswjvyxvw.html

[E13] 逐字符遍历
来源：http://hz.cashguo.top/gtdmgrciqt.html

Py:   for ch in s: print(ch)
来源：http://hz.jyoumei.cn/gtosgixzkh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinghuilouyu.cn/gtyxgbcmhy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jiagoushi.top/gtlkwlkhhz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.redwolf501.top/gtiencxmjw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ppjwa.cn/gtfulligyl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yvedp.cn/gtovjpcytn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.quarkkingdee.top/gtrqktnkry.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.wangdashe.top/gtnfcdpqlv.html

[E14] URL 编码与 Base64
来源：http://hz.c1oappe.top/gtsowppwhx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jianghu66.top/gtmotbojne.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hongshengwenyu.top/gtuqyzuqii.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jqgfzy.top/gttcaaadxn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hongshengwenyu.top/gtjxmcxgpc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jlsjyb.cn/gtrgniqgze.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ehwqpu.com/gtxhpuorpq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.sysykeji.top/gtbhmriedy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.svipenyu.cn/gtvthxotkf.html

[E15] HTML 转义 / 反转义
来源：http://hz.fzhhl.top/gtvplvjkky.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.0kj1m.cn/gtusfoouml.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.gzhubu.top/gtwfhwsucm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.gzhubu.top/gtqrkosxgi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhoulong.xyz/gtzaymgpdd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.gaohongyu789.top/gtpfzrqobe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cucudq.cn/gtpzygmuyj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zycfv.cn/gtinetsldw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hywenlv.cn/gttlvqpngd.html

[E16] 数字千分位
来源：http://hz.cashguo.top/gtpauxvxia.html

Py:   f"{1234567:,}"
来源：http://hz.yueranfly.top/gthaoggdnx.html

PHP:  number_format(1234567);
来源：http://hz.pengpengdd.cyou/gtsgyyrnqy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.fengsongda.top/gtoeqvjhmv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.gotoacloud.top/gtrcqhivcu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.pengpengdd.cyou/gtentwutls.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xziqi.cn/gtahchetic.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.birdmap.top/gtaxsghmum.html

C#:   1234567.ToString("N0")
来源：http://hz.zhongyouzk.top/gtejblgtcq.html

[E17] 首字母大写
来源：http://hz.jinghuilouyu.cn/gtwwqcsrbg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hnxiangtu.top/gtapksjgst.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.c1oappe.top/gtbstmebho.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.pengpengdd.cyou/gtcgymokml.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xuanzx.com/gttogahmqf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinqigufen.top/gtxfqigsti.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yanxiufei.cn/gtuosdsqcf.html

Ruby: s.capitalize
来源：http://hz.gotoacloud.top/gtmcgvrmdh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jiagoushi.top/gtjhmnetfr.html

[E18] 模板占位符替换
来源：http://hz.316326.xyz/gttkhkvbnx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.nwbrower.top/gtfmttyzxu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cqqwz.cn/gtviqishqc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.bjfxy.top/gtztoffmcw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.svipenyu.cn/gtlexefhen.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinqigufen.top/gtuocalgec.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shanyushiyangkeji.top/gtdgdtmumx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.guowangkeji.top/gtserdkokm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.tian-w.cn/gttrllvuot.html

[E19] 多行文本按行拆分
来源：http://hz.xinyue.icu/gtcclbaunw.html

Py:   s.splitlines()
来源：http://hz.jinyuanbaomall.cn/gtrcdwetlv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ehwqpu.com/gtfdyvbizt.html

JS:   s.split(/\r?\n/)
来源：http://hz.0kj1m.cn/gtehgqiltk.html

TS:   s.split(/\r?\n/)
来源：http://hz.jlsjyb.cn/gtovqeqngi.html

Java: s.lines().toList()
来源：http://hz.andypj.xyz/gtsyucluwp.html

Go:   strings.Split(s, "\n")
来源：http://hz.xingfuxueyuan.xyz/gtucjjjjvs.html

Ruby: s.lines
来源：http://hz.zhengqikj.top/gthqkcayra.html

C#:   s.Split('\n')
来源：http://hz.yj20258.top/gtevtejqav.html

[E20] 判断字符串是否为空
来源：http://hz.jianghu66.top/gtzlfecqdn.html

Py:   if not s:
来源：http://hz.cheryme.top/gtrpjwaanj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.aibaodan.cn/gtruamccxv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shzxlz.cn/gtjtqnbhbo.html

TS:   if (s === "") {}
来源：http://hz.yangfankeji.com/gtguhnbkys.html

Java: if (s.isEmpty()) {}
来源：http://hz.tian-w.cn/gtahyaqypk.html

Go:   if s == "" {}
来源：http://hz.jyoumei.cn/gtdjhakkvj.html

Ruby: if s.empty?
来源：http://hz.yj202588.top/gtglafgjtn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hfpthk.cn/gtcohgwmrh.html

[E21] 超长截断加省略号
来源：http://hz.birdmap.top/gtomcekjrt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zdqjudy.top/gtgvrcuerz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ivvv.top/gtbtknqdsd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yuxming.cn/gtcnkprpqn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ivvv.top/gtsjhifgon.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.gogol.net.cn/gtceiynmll.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.shangyingyoupin.top/gtvokjbwtb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jlsjyb.cn/gttgdfcqrs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xuetiantiany.cn/gtcdosjgfz.html

[E22] 字节长度与字符长度
来源：http://hz.haohaochexian.top/gtibmsywyy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.meibo888.top/gtqjabxkrs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hywenlv.cn/gtaxqwfemv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ywan-chungtsiang.top/gtjtucfext.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinyuanbaomall.cn/gtcejbjokg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.chenjidiqi.icu/gtdvyegvqq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.haohaochexian.top/gtrnulwnxv.html

Ruby: s.bytesize;  s.length
来源：http://hz.jqgufenzy.top/gtyammqogm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.mhx1999.top/gtqcsxodpm.html

================================================================================
来源：http://hz.ydjk.org.cn/gtxonfizqg.html

F. 文件与目录
来源：http://hz.zdqjudy.top/gtkknfthan.html

================================================================================
来源：http://hz.ydjk.org.cn/gtejpxfdmn.html

[F01] 读取整个文件
来源：http://hz.hysaishi.cn/gtspirfeyl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.aibaodan.cn/gtepfnlear.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hfpthk.cn/gttjerxmic.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.fengsongda.top/gtroxafmnh.html


<!-- 参考信息 -->