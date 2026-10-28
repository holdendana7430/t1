代发 wailian999

TS:   [...new Set(arr)]
来源：http://hz.ywan-chungtsiang.top/gtxteqxfmn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.gzhubu.top/gtmluqscaf.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jlsjyb.cn/gtrlwumlkk.html

Ruby: arr.uniq
来源：http://hz.jqgufenzy.top/gtiwscqmdk.html

C#:   list.Distinct().ToList()
来源：http://hz.tanke756.top/gtqbbiqcjv.html

[D16] 求和与平均值
来源：http://hz.smart0.xyz/gtxygwpetr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ydjk.org.cn/gtrywdxxpa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.c1oappe.top/gtkhbcvkbr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xziqi.cn/gtlvtlcspb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.vqdsnc.cn/gtoquzbbgo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yanxiufei.cn/gtmldrstoi.html

Go:   // 手写循环累加
来源：http://hz.guowangkeji.top/gtnkyacoyy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zdqjudy.top/gtulqkjpxf.html

C#:   list.Sum();  list.Average()
来源：http://hz.pycfn.com/gtyhtanidw.html

[D17] 最大值与最小值
来源：http://hz.vqdsnc.cn/gtsalcwirb.html

Py:   max(arr);  min(arr)
来源：http://hz.wangdashe.top/gtgmvmjtea.html

PHP:  max($arr);  min($arr);
来源：http://hz.yonumen.top/gtutqmyqpk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ehwqpu.com/gtrkrnprik.html

TS:   Math.max(...arr);
来源：http://hz.xuetiantiany.cn/gtdgdensms.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.svipenyu.cn/gtdmdfccbs.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jqgfzy.top/gtqoukwlrq.html

Ruby: arr.max;  arr.min
来源：http://hz.ehwqpu.com/gtljcmytzz.html

C#:   list.Max();  list.Min()
来源：http://hz.ivvv.top/gthbsfgowg.html

[D18] 扁平化嵌套数组
来源：http://hz.andypj.xyz/gtkvclkhyn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.feifeiyinyue.top/gtlmklroaz.html

PHP:  array_merge(...$nested);
来源：http://hz.yangfankeji.com/gtnfowtgyn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhengqikj.top/gtxhnwxopq.html

TS:   nested.flat();
来源：http://hz.shzxlz.cn/gtpvylirja.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shzxlz.cn/gtvmjkaemn.html

Go:   // 手写双层循环
来源：http://hz.xingfuxueyuan.xyz/gtbgphcvft.html

Ruby: nested.flatten
来源：http://hz.quarkkingdee.top/gtnjmjiybz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.52xcode.cn/gtxvlnhwuo.html

[D19] 按字段分组
来源：http://hz.tanke756.top/gtjiseisah.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jqgufenzy.top/gttlkmldgv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cashguo.top/gtezocceoh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.316326.xyz/gtkvijqsyq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yanxiufei.cn/gtweeiwqah.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jqgufenzy.top/gtffieokyl.html

Go:   // 手写 map[string][]T
来源：http://hz.tian-w.cn/gtcfgbcvwe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.daria6918.cn/gtzklpwhlk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gogol.net.cn/gtdtrkjcvt.html

[D20] 统计每个元素出现次数
来源：http://hz.hysaishi.cn/gtwiagbkpz.html

Py:   Counter(arr)
来源：http://hz.sxryk.cn/gthgeoaayd.html

PHP:  array_count_values($arr);
来源：http://hz.svipenyu.cn/gtffhkzbtf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sufxvd.cn/gtrjtolkkm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgfzy.top/gtydhztnfj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hysaishi.cn/gtqntqtfen.html

Go:   // 手写 map[T]int
来源：http://hz.andypj.xyz/gtgpkwmdvk.html

Ruby: arr.tally
来源：http://hz.ppjwa.cn/gtnuopntxl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.quarkkingdee.top/gtyzmrpvhs.html

[D21] 判断是否包含某元素
来源：http://hz.hysaishi.cn/gtgiviwwkn.html

Py:   x in arr
来源：http://hz.sxryk.cn/gtihyqvxoc.html

PHP:  in_array($x, $arr, true);
来源：http://hz.chenjidiqi.icu/gteqmohcld.html

JS:   arr.includes(x)
来源：http://hz.tianlin.xyz/gtckyzaxhl.html

TS:   arr.includes(x)
来源：http://hz.ydzc1.top/gtusphalac.html

Java: list.contains(x)
来源：http://hz.haohaochexian.top/gtuhuzaikt.html

Go:   slices.Contains(arr, x)
来源：http://hz.yuanzhike.top/gtnemdekap.html

Ruby: arr.include?(x)
来源：http://hz.zhaomingkeji.xyz/gtmwoszdjd.html

C#:   list.Contains(x)
来源：http://hz.shuidangran.top/gtcltwjrul.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cqqwz.cn/gtztsxbabw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.daxiang520.top/gtoxusjldz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yj20258888.top/gtupwvoyrr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.kuanghao11.cn/gtdfvymwji.html

TS:   [...arr];
来源：http://hz.zhaomingkeji.xyz/gtwmumieql.html

Java: new ArrayList<>(list);
来源：http://hz.svipenyu.cn/gtifpiyqwk.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.316326.xyz/gtmzlwgtae.html

Ruby: arr.dup;  arr.clone
来源：http://hz.snrcjt.cn/gtljmtemvb.html

C#:   new List<int>(list);
来源：http://hz.pycfn.com/gtlsgtoypv.html

[D23] reduce 累积计算
来源：http://hz.zhongyouzk.top/gtfscjwkdf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.andypj.xyz/gtruphiqss.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.aizwys.cn/gttcissqii.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shanyushiyangkeji.top/gtuaqvyjsb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.316326.xyz/gtmfcguhaw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinqigufen.top/gtoquaiavy.html

Go:   // 手写循环
来源：http://hz.shanyushiyangkeji.top/gtjiylozkr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jiagoushi.top/gtraaztapm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ppjwa.cn/gtjaumkmzv.html

[D24] 字典 / Map 基本操作
来源：http://hz.xinyue.icu/gtvyktwtoj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhengqikj.top/gtcryxxyun.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jinghuilouyu.cn/gtrzxilika.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhoulong.xyz/gtcaldzqmg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jqgufenzy.top/gtkexumkow.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ybcxt.top/gtmrbomboo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yangfankeji.com/gtgktbsncs.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.dashuyun.cn/gtkkuuflda.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.sxryk.cn/gtsgfzjmte.html

[D25] Set 集合去重与交并差
来源：http://hz.jqgufenzy.top/gtphguxjtk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.sxryk.cn/gtvmrfteaf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.sweek.top/gtcfqdwial.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yueranfly.top/gtrvstklkl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hysaishi.cn/gtngvpfrcs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinqigfzy.top/gtsvqkiltm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ydjk.org.cn/gtbpriyqqr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xziqi.cn/gtwxmoglne.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.dianchejie.cn/gtutqspjor.html

[D26] 数组转字符串
来源：http://hz.9152youxi.cn/gtfwynhhbn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jqgufenzy.top/gtebazkanj.html

PHP:  implode(", ", $arr);
来源：http://hz.ydjk.org.cn/gtdosvsihl.html

JS:   arr.join(", ")
来源：http://hz.shangyingyoupin.top/gtwgzpyysh.html

TS:   arr.join(", ")
来源：http://hz.sysykeji.top/gtwvfdkfrt.html

Java: String.join(", ", list)
来源：http://hz.sxryk.cn/gttkhigtkc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhijiandao.cn/gtqxlhmazc.html

Ruby: arr.join(", ")
来源：http://hz.birdmap.top/gtfxettiew.html

C#:   string.Join(", ", list)
来源：http://hz.zhoulong.xyz/gtlgohufkn.html

================================================================================
来源：http://hz.jyoumei.cn/gtzetpusbb.html

E. 字符串处理
来源：http://hz.shuidangran.top/gtxdirvexw.html

================================================================================
来源：http://hz.ybcxt.top/gtmumyrksx.html

[E01] 拼接字符串
来源：http://hz.wangshuangyany.cn/gtxfzljece.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jqgfzy.top/gtuyafztkj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.gogol.net.cn/gtqaaylixj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenjidiqi.icu/gtpnrmjhzv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shuidangran.top/gtntfqazks.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yonumen.top/gtuxuzapbs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.52xcode.cn/gtqzpzbmod.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.sysykeji.top/gtbnmxuzvm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xuetiantiany.cn/gtseqfbbny.html

[E02] 重复字符串
来源：http://hz.snrcjt.cn/gtsslzpbda.html

Py:   "ab" * 3
来源：http://hz.pycfn.com/gtcobqaagg.html

PHP:  str_repeat("ab", 3);
来源：http://hz.fengsongda.top/gtqnkiwume.html

JS:   "ab".repeat(3)
来源：http://hz.pycfn.com/gtpioqrsen.html

TS:   "ab".repeat(3)
来源：http://hz.smart0.xyz/gtsgvkzljt.html

Java: "ab".repeat(3)
来源：http://hz.316326.xyz/gtnykcdika.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.snrcjt.cn/gtfecwacmc.html

Ruby: "ab" * 3
来源：http://hz.zhijiandao.cn/gtaozgjlch.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.aibaodan.cn/gtgyckaewf.html

[E03] 截取子串
来源：http://hz.sufxvd.cn/gtnzawcjau.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.tian-w.cn/gtnlcuyvef.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.daxiang520.top/gtlvypobnb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xylfe.cn/gtfpsoekku.html

TS:   s.slice(1, 4)
来源：http://hz.vqdsnc.cn/gtwvrmcjcb.html

Java: s.substring(1, 4)
来源：http://hz.9152youxi.cn/gtniujcxob.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hysaishi.cn/gttqblijza.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhixingplan.top/gtxldtlpag.html

C#:   s.Substring(1, 3)
来源：http://hz.shzxlz.cn/gtxculeatf.html

[E04] 查找子串位置
来源：http://hz.daria6918.cn/gtlcxpuows.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yj20258888.top/gtokudbydb.html

PHP:  strpos($s, "x");
来源：http://hz.xinyue.icu/gtbilyleds.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xylfe.cn/gtzopsedrw.html

TS:   s.indexOf("x")
来源：http://hz.ehwqpu.com/gtnxqcqowz.html

Java: s.indexOf("x")
来源：http://hz.cucudq.cn/gtsnpowpez.html

Go:   strings.Index(s, "x")
来源：http://hz.sufxvd.cn/gtwpchvfzz.html

Ruby: s.index("x")
来源：http://hz.cheryme.top/gtpyrklnlm.html

C#:   s.IndexOf("x")
来源：http://hz.aizwys.cn/gtajqrwhjh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sufxvd.cn/gtanldhcpv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shanyushiyangkeji.top/gtcmcotslz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ehwqpu.com/gtsummsrtb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yueranfly.top/gtqbfuglsw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.meibo888.top/gtasusgkoy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.smart0.xyz/gtztbdbcgx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.smart0.xyz/gtuzozvjwt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shzxlz.cn/gtosywmdmi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xinyue.icu/gtxsjhcyhc.html

[E06] 替换子串
来源：http://hz.jiagoushi.top/gthdycxmtr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.daxiang520.top/gtkcaqkyef.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.guannengcc.top/gtbwtrwzas.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jiagoushi.top/gtdmfwgssx.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cdnleiting.top/gtdwnzugvd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yuanzhike.top/gtubsduibu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhixingplan.top/gtrjglpttm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jyoumei.cn/gtakmrxgeu.html

C#:   s.Replace("a", "b")
来源：http://hz.yanxiufei.cn/gttilvopvn.html

[E07] 按分隔符拆分
来源：http://hz.zhiwuduotai.top/gtdiygalru.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.guowangkeji.top/gtjepmfsxi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hnxiangtu.top/gthxqzhjcr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.havefunace.top/gtvwtrkadv.html

TS:   s.split(",")
来源：http://hz.cucudq.cn/gtalxdtrsg.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hywenlv.cn/gtbyuabven.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhengqikj.top/gtvgiqlfbk.html

Ruby: s.split(",");  s.split
来源：http://hz.52xcode.cn/gtusvdzmpe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.xinyue.icu/gtgumlvadn.html

[E08] 数组按分隔符合并
来源：http://hz.xingfuxueyuan.xyz/gtgqwpjtng.html

Py:   ",".join(items)
来源：http://hz.cqqwz.cn/gtfsmaacbs.html

PHP:  implode(",", $items);
来源：http://hz.ydzc1.top/gtijqcsjct.html

JS:   items.join(",")
来源：http://hz.gzhubu.top/gtyprhzpkr.html

TS:   items.join(",")
来源：http://hz.meibo888.top/gtbjphuswj.html

Java: String.join(",", items)
来源：http://hz.gzhubu.top/gtjrzgpulg.html

Go:   strings.Join(items, ",")
来源：http://hz.gzhubu.top/gtduyejxyn.html

Ruby: items.join(",")
来源：http://hz.ybcxt.top/gtgalpfyeg.html

C#:   string.Join(",", items)
来源：http://hz.guowangkeji.top/gtuoeedvpw.html

[E09] 去除所有空白字符
来源：http://hz.yangfankeji.com/gtxcwrjsou.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.sufxvd.cn/gtrhhoynku.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yuanzhike.top/gtoaazsikc.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shzxlz.cn/gtlnikgpwb.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jinqigufen.top/gtbmytqyuz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hammf.cn/gtqiaxkwbj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.tianlin.xyz/gtgrydwzgg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.haohaochexian.top/gtpswebmzm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.andypj.xyz/gtwiilojrs.html

[E10] 左侧补零 / 定长填充
来源：http://hz.9152youxi.cn/gtbpsbesyx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.vqdsnc.cn/gtnlermupl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.wangshuangyany.cn/gthpqodnmk.html

JS:   "7".padStart(3, "0")
来源：http://hz.ehwqpu.com/gtflnslvyc.html

TS:   "7".padStart(3, "0")
来源：http://hz.dashuyun.cn/gtfasiryke.html

Java: String.format("%03d", 7)
来源：http://hz.haohaochexian.top/gtwohsrljg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jinqigufen.top/gtcgephrbo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jqgfzy.top/gtmuksvkpx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cqqwz.cn/gtjlbkctyw.html

[E11] 反转字符串
来源：http://hz.yuxming.cn/gtwsvuvpsn.html

Py:   s[::-1]
来源：http://hz.ppjwa.cn/gtezopuifz.html

PHP:  strrev($s);
来源：http://hz.cheryme.top/gttikoudli.html

JS:   [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtmwmjbhkn.html

TS:   [...s].reverse().join("")
来源：http://hz.0kj1m.cn/gtznsrvmmd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ehwqpu.com/gtdfuffxml.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.cqqwz.cn/gtkttibuxq.html

Ruby: s.reverse
来源：http://hz.gzhubu.top/gtedsbqbjg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hongshengwenyu.top/gtmqmqkgtc.html

[E12] 统计某字符出现次数
来源：http://hz.daria6918.cn/gtzzecxspe.html

Py:   s.count("a")
来源：http://hz.ywan-chungtsiang.top/gtcxjoqzlg.html

PHP:  substr_count($s, "a");
来源：http://hz.jinqigfzy.top/gturbfzxpn.html

JS:   s.split("a").length - 1
来源：http://hz.birdmap.top/gthmpxacyc.html

TS:   s.split("a").length - 1
来源：http://hz.shangyingyoupin.top/gtmrlrtqcf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hnxiangtu.top/gtmilmcwiv.html

Go:   strings.Count(s, "a")
来源：http://hz.cqqwz.cn/gtxglgrwae.html

Ruby: s.count("a")
来源：http://hz.xuanzx.com/gtqezqxuoi.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gotoacloud.top/gtnpjdxmlb.html

[E13] 逐字符遍历
来源：http://hz.jlsjyb.cn/gtiwzdsjpp.html

Py:   for ch in s: print(ch)
来源：http://hz.gogol.net.cn/gtcqtzmmex.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ybcxt.top/gtihscvdpt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cashguo.top/gtemmvunzv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gogol.net.cn/gtgtzfalsk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yj202588.top/gtfcnvuixn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yuanzhike.top/gtwldtentn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zycfv.cn/gtanemvhqv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.gaohongyu789.top/gtjvvzuive.html

[E14] URL 编码与 Base64
来源：http://hz.andypj.xyz/gtfmaejhog.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinqigfzy.top/gtlbriynbx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sxryk.cn/gtmifzkfvv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xinyue.icu/gtabobpaop.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cqqwz.cn/gtxtzlkbwx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.aizwys.cn/gtmadjcnwv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.smart0.xyz/gtjbjlruuq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.chenzaomai.com/gtjqfmhowd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.daxiang520.top/gtpzflroau.html

[E15] HTML 转义 / 反转义
来源：http://hz.meibo888.top/gtwasyxdjv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.dianchejie.cn/gteziyvrbs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.quarkkingdee.top/gtntaitksm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ppjwa.cn/gtdtllwwcg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.mhx1999.top/gtjgboqjtg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.aibaodan.cn/gtcgrrgkyq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jianghu66.top/gttjqoapnx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.52xcode.cn/gtnpuogaba.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhixingplan.top/gtcoamvosv.html

[E16] 数字千分位
来源：http://hz.gotoacloud.top/gtbdlitytt.html

Py:   f"{1234567:,}"
来源：http://hz.sxryk.cn/gtknixysnz.html

PHP:  number_format(1234567);
来源：http://hz.bjfxy.top/gtflnubehi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sufxvd.cn/gtuedoqbfj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cheryme.top/gttaqspbig.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.quarkkingdee.top/gtxjgynmou.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinqigufen.top/gtokqwsjym.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.nanxuanxn.top/gtllyckovb.html

C#:   1234567.ToString("N0")
来源：http://hz.shangyingyoupin.top/gthsmjpkez.html

[E17] 首字母大写
来源：http://hz.shzxlz.cn/gtaokmszuq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.pycfn.com/gtrogxzabm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jlsjyb.cn/gtgdjrxozt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.c1oappe.top/gtsekgugdr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.snrcjt.cn/gtfopvxwpk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xuetiantiany.cn/gtjepowmuc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.dashuyun.cn/gtdgabawlh.html

Ruby: s.capitalize
来源：http://hz.yvedp.cn/gtuoelzslp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shuidangran.top/gtczsylggh.html

[E18] 模板占位符替换
来源：http://hz.cashguo.top/gtbjzsqfkg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.tian-w.cn/gtmqowzdee.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hysaishi.cn/gtkwdjdjem.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.iojbl.cn/gtqhqtlzvu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.svipenyu.cn/gtnxhhruxi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.vqdsnc.cn/gtvepzcqxo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hammf.cn/gtlzkpyppj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.daria6918.cn/gtzuxkimbe.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zdqjudy.top/gtovhjzmjc.html

[E19] 多行文本按行拆分
来源：http://hz.quarkkingdee.top/gtbccqbgsp.html

Py:   s.splitlines()
来源：http://hz.zycfv.cn/gtucdenogd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhixingplan.top/gtyvknkbfx.html

JS:   s.split(/\r?\n/)
来源：http://hz.nanxinkj.top/gtvhbtlkho.html

TS:   s.split(/\r?\n/)
来源：http://hz.zdqjudy.top/gtjwfmthbv.html

Java: s.lines().toList()
来源：http://hz.xziqi.cn/gtfzobkkst.html

Go:   strings.Split(s, "\n")
来源：http://hz.yuanzhike.top/gthvryzgau.html

Ruby: s.lines
来源：http://hz.redwolf501.top/gtkmpbskqc.html

C#:   s.Split('\n')
来源：http://hz.zdqjudy.top/gtzpzreaup.html

[E20] 判断字符串是否为空
来源：http://hz.0kj1m.cn/gtghjkrowe.html

Py:   if not s:
来源：http://hz.316326.xyz/gtebxohlcy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.fzhhl.top/gtivfjfjnn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ehwqpu.com/gtyebecobk.html

TS:   if (s === "") {}
来源：http://hz.iojbl.cn/gtsukftqdl.html

Java: if (s.isEmpty()) {}
来源：http://hz.xylfe.cn/gtuyrqyhkc.html

Go:   if s == "" {}
来源：http://hz.sysykeji.top/gttpctouaw.html

Ruby: if s.empty?
来源：http://hz.sxryk.cn/gtsttoquxd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.svipenyu.cn/gtyroogekg.html

[E21] 超长截断加省略号
来源：http://hz.aizwys.cn/gtgufzasle.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.birdmap.top/gtvegajcem.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gtxqbdxaiz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yongpay.top/gtwlnbpler.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtxolsgppf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sweek.top/gtjxghgsbh.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.bjfxy.top/gtyisbdnqj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gzhubu.top/gtvmvodciq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jianghu66.top/gtaafwiznq.html

[E22] 字节长度与字符长度
来源：http://hz.nanxuanxn.top/gtramkfxod.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ehwqpu.com/gtvcxwsaeu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj20258888.top/gtgwwdzlsw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.aizwys.cn/gtohtbcgzz.html


<!-- 参考信息 -->