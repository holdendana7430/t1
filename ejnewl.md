代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.nanxinkj.top/gtmqekwieg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhoulong.xyz/gtcxrkmodh.html

JS:   arr.map(x => x * 2)
来源：http://hz.kuanghao11.cn/gthzafeijm.html

TS:   arr.map(x => x * 2)
来源：http://hz.yj20258888.top/gtdpocniwf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yj202588.top/gtlqyprfem.html

Go:   // 手写循环
来源：http://hz.zhengqikj.top/gteljwqutp.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hnqzz.top/gtmhvopqxt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hammf.cn/gtlzlmshzh.html

[D15] 去重
来源：http://hz.jiagoushi.top/gtqluszhwb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.tanke756.top/gtwmbzakgo.html

PHP:  array_unique($arr);
来源：http://hz.cqqwz.cn/gtsqncabpy.html

JS:   [...new Set(arr)]
来源：http://hz.zdqjudy.top/gtrfzeyjsb.html

TS:   [...new Set(arr)]
来源：http://hz.yuxming.cn/gteffwbuud.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.smart0.xyz/gtyfysfhub.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yj20258.top/gtokrtxlxk.html

Ruby: arr.uniq
来源：http://hz.52xcode.cn/gtjmtyxolu.html

C#:   list.Distinct().ToList()
来源：http://hz.xuetiantiany.cn/gtzpkrchwm.html

[D16] 求和与平均值
来源：http://hz.9152youxi.cn/gtbbnwvicm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gogol.net.cn/gtfoctoxzc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cheryme.top/gtfuxkdtto.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj202588.top/gtrsgpaewm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgufenzy.top/gtuboslikv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.smart0.xyz/gtrqfscuoe.html

Go:   // 手写循环累加
来源：http://hz.smart0.xyz/gtcjjtpklx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.redwolf501.top/gtfsogccqf.html

C#:   list.Sum();  list.Average()
来源：http://hz.snrcjt.cn/gtpktqcfxr.html

[D17] 最大值与最小值
来源：http://hz.gaohongyu789.top/gtgbhjzrol.html

Py:   max(arr);  min(arr)
来源：http://hz.smart0.xyz/gtslrjgtdk.html

PHP:  max($arr);  min($arr);
来源：http://hz.zycfv.cn/gttjjfympy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cheryme.top/gtkbxbqaqo.html

TS:   Math.max(...arr);
来源：http://hz.yueranfly.top/gtjxjzhhqa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jqgfzy.top/gtxsnnwmhk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.nanxuanxn.top/gtwzqtogwv.html

Ruby: arr.max;  arr.min
来源：http://hz.zhengqikj.top/gtcpnpttmd.html

C#:   list.Max();  list.Min()
来源：http://hz.xziqi.cn/gtnbevzbak.html

[D18] 扁平化嵌套数组
来源：http://hz.jianghu66.top/gtdrihbyij.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhaomingkeji.xyz/gtxfzosiav.html

PHP:  array_merge(...$nested);
来源：http://hz.hywenlv.cn/gtjizvyykn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.fengsongda.top/gtofembhux.html

TS:   nested.flat();
来源：http://hz.yuxming.cn/gtcbuxdsde.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.bjfxy.top/gtvjhsbhfc.html

Go:   // 手写双层循环
来源：http://hz.gogol.net.cn/gtatmhmmkp.html

Ruby: nested.flatten
来源：http://hz.yueranfly.top/gtitjrrbet.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ppjwa.cn/gtlzkjerfd.html

[D19] 按字段分组
来源：http://hz.dianchejie.cn/gtjrejrwzf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shuidangran.top/gtldkrxnan.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.sufxvd.cn/gtkognqsdu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.aibaodan.cn/gtbrjmcxzj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jinyuanbaomall.cn/gtcmvwpuxw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xinyue.icu/gtqepbabib.html

Go:   // 手写 map[string][]T
来源：http://hz.ehwqpu.com/gtvnxkodgk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhengqikj.top/gtfjlswhym.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yonumen.top/gthlsiwvbd.html

[D20] 统计每个元素出现次数
来源：http://hz.yj20258.top/gtjyfhlmqv.html

Py:   Counter(arr)
来源：http://hz.yueranfly.top/gtxxskvzjw.html

PHP:  array_count_values($arr);
来源：http://hz.nwbrower.top/gtpmtehnsm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cqqwz.cn/gtpmiztsti.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj20258.top/gtuvosabyj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.quarkkingdee.top/gtxilwbkce.html

Go:   // 手写 map[T]int
来源：http://hz.snrcjt.cn/gtuubstsqn.html

Ruby: arr.tally
来源：http://hz.iojbl.cn/gtsmzxwtek.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.fzhhl.top/gthykuwoyj.html

[D21] 判断是否包含某元素
来源：http://hz.gzhubu.top/gtodsrabar.html

Py:   x in arr
来源：http://hz.yj20258.top/gtmbisvaao.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gotoacloud.top/gtgakmfrxi.html

JS:   arr.includes(x)
来源：http://hz.dianchejie.cn/gtkczpuotl.html

TS:   arr.includes(x)
来源：http://hz.xylfe.cn/gtlgnydykz.html

Java: list.contains(x)
来源：http://hz.shanyushiyangtech.top/gtqmdhymmy.html

Go:   slices.Contains(arr, x)
来源：http://hz.guowangkeji.top/gtxmpbajbw.html

Ruby: arr.include?(x)
来源：http://hz.pycfn.com/gtcmqxpwii.html

C#:   list.Contains(x)
来源：http://hz.pengpengdd.cyou/gtsgxxjgcm.html

[D22] 复制数组（避免共享引用）
来源：http://hz.xuanzx.com/gtnfhaqple.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.redwolf501.top/gtvzbzzpjn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.tianlin.xyz/gtpcnctikz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jlsjyb.cn/gtbpuhqewq.html

TS:   [...arr];
来源：http://hz.smart0.xyz/gtrydsjggn.html

Java: new ArrayList<>(list);
来源：http://hz.52xcode.cn/gtdlprslgw.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.cucudq.cn/gtokpbfdbn.html

Ruby: arr.dup;  arr.clone
来源：http://hz.cqqwz.cn/gtlqkmkkfz.html

C#:   new List<int>(list);
来源：http://hz.yvedp.cn/gtofzcxctp.html

[D23] reduce 累积计算
来源：http://hz.cheryme.top/gtpblgluko.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cheryme.top/gtvoznuwga.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jqgufenzy.top/gtbgiwdlac.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hnqzz.top/gtpfjvpggb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.dianchejie.cn/gtkzrivtjd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.feifeiyinyue.top/gtaejdlrdx.html

Go:   // 手写循环
来源：http://hz.tianlin.xyz/gtfqidwvxj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.svipenyu.cn/gtaajeatdx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hywenlv.cn/gtezzteoaa.html

[D24] 字典 / Map 基本操作
来源：http://hz.ppjwa.cn/gtrndhxeee.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhoulong.xyz/gttwhczkhd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xuetiantiany.cn/gtnendwgyh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shanyushiyangkeji.top/gtruqqpcsn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zhengqikj.top/gtmnxwwqsw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sxryk.cn/gtmqqpinxz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.gaohongyu789.top/gtzcrkacry.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ehwqpu.com/gtuplscssn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.chenlongwang.top/gtwbvagkat.html

[D25] Set 集合去重与交并差
来源：http://hz.guowangkeji.top/gtjqhdejle.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhengqikj.top/gtqlfceigl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.birdmap.top/gtsjihcyir.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yuxming.cn/gtjurhjabo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cdnleiting.top/gtzeoqvtvf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.vqdsnc.cn/gtjhkcxlts.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jlsjyb.cn/gtsznmhbwm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jianghu66.top/gtgljcszei.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.pengpengdd.cyou/gtuagafcyw.html

[D26] 数组转字符串
来源：http://hz.yueranfly.top/gtiideczrv.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ydzc1.top/gtskkbeekb.html

PHP:  implode(", ", $arr);
来源：http://hz.bjfxy.top/gtzicguiqc.html

JS:   arr.join(", ")
来源：http://hz.yueranfly.top/gthiftbwws.html

TS:   arr.join(", ")
来源：http://hz.shanyushiyangkeji.top/gtiqhmnima.html

Java: String.join(", ", list)
来源：http://hz.aibaodan.cn/gtjybxlgdo.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hnxiangtu.top/gtquccnyma.html

Ruby: arr.join(", ")
来源：http://hz.pycfn.com/gtwmvvtttn.html

C#:   string.Join(", ", list)
来源：http://hz.snrcjt.cn/gtkuemechr.html

================================================================================
来源：http://hz.gotoacloud.top/gtnahpjgcd.html

E. 字符串处理
来源：http://hz.sufxvd.cn/gtoijejdni.html

================================================================================
来源：http://hz.pycfn.com/gtosvsmssg.html

[E01] 拼接字符串
来源：http://hz.yj20258888.top/gtqvvdzeqf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hnqzz.top/gtrvxvbmaw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ppjwa.cn/gttheahfkl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.birdmap.top/gtzdzmdeie.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tian-w.cn/gtrhnxckub.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.c1oappe.top/gtqebtpxim.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenzaomai.com/gtzxzendzo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.snrcjt.cn/gtbjbasghx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yonumen.top/gtpwljfypp.html

[E02] 重复字符串
来源：http://hz.shanyushiyangtech.top/gtqkrcrjnl.html

Py:   "ab" * 3
来源：http://hz.yangfankeji.com/gtnvtwtjjv.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xylfe.cn/gtbzvjuotr.html

JS:   "ab".repeat(3)
来源：http://hz.dashuyun.cn/gtezgqcame.html

TS:   "ab".repeat(3)
来源：http://hz.52xcode.cn/gtbkfvbrkg.html

Java: "ab".repeat(3)
来源：http://hz.cheryme.top/gtactnhjce.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hfpthk.cn/gtmemhmetp.html

Ruby: "ab" * 3
来源：http://hz.yj20258.top/gthpbbeiez.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jyoumei.cn/gtvjdsoiqr.html

[E03] 截取子串
来源：http://hz.quarkkingdee.top/gtqmqiakbi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zdqjudy.top/gtbhckfzix.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.tianlin.xyz/gticjilaol.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.redwolf501.top/gtdkchrdly.html

TS:   s.slice(1, 4)
来源：http://hz.hywenlv.cn/gtfodyzdup.html

Java: s.substring(1, 4)
来源：http://hz.cdnleiting.top/gtbbaalhxm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.chenzaomai.com/gtqzappkfb.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ivvv.top/gtntbxoleg.html

C#:   s.Substring(1, 3)
来源：http://hz.yanxiufei.cn/gtrpsdcnrt.html

[E04] 查找子串位置
来源：http://hz.meibo888.top/gtnwawxizo.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yongpay.top/gtwjfsfmyd.html

PHP:  strpos($s, "x");
来源：http://hz.zhaomingkeji.xyz/gtdjgwhnfh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.fengsongda.top/gtfgysraed.html

TS:   s.indexOf("x")
来源：http://hz.wangshuangyany.cn/gtywxfrjor.html

Java: s.indexOf("x")
来源：http://hz.hnxiangtu.top/gtwtwvjzgi.html

Go:   strings.Index(s, "x")
来源：http://hz.shangyingyoupin.top/gtsqvhiqss.html

Ruby: s.index("x")
来源：http://hz.aibaodan.cn/gtugtsifud.html

C#:   s.IndexOf("x")
来源：http://hz.birdmap.top/gtgwjdjfzg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.0kj1m.cn/gtabbjqnds.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.havefunace.top/gtmjbomotq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.316326.xyz/gthdjtpxdz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinqigufen.top/gtjigsuytt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.pengpengdd.cyou/gttlvkxnun.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yueranfly.top/gtvycmbate.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zycfv.cn/gtuoatfxiz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.pengpengdd.cyou/gtvcsmerje.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ehwqpu.com/gtalkdywnk.html

[E06] 替换子串
来源：http://hz.smart0.xyz/gtzpxorbri.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.pycfn.com/gtcntmstao.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.316326.xyz/gtrrfmlyae.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jyoumei.cn/gtmnriulnp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yangfankeji.com/gthunfeeej.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhongyouzk.top/gtezjoiepj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.tanke756.top/gtrfqbqizt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.vqdsnc.cn/gtcleopzkz.html

C#:   s.Replace("a", "b")
来源：http://hz.jiagoushi.top/gtwocndpcn.html

[E07] 按分隔符拆分
来源：http://hz.gaohongyu789.top/gtjhpgzfea.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.c1oappe.top/gtgoycuira.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shanyushiyangkeji.top/gtlxolplur.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cqqwz.cn/gtgkwuevmx.html

TS:   s.split(",")
来源：http://hz.wangshuangyany.cn/gtlxadmdek.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.sxryk.cn/gtfilaiobc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ywan-chungtsiang.top/gtnteyvhxn.html

Ruby: s.split(",");  s.split
来源：http://hz.pycfn.com/gthxdrqage.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cdnleiting.top/gtmxrsiohp.html

[E08] 数组按分隔符合并
来源：http://hz.snrcjt.cn/gtrrdbnajp.html

Py:   ",".join(items)
来源：http://hz.xuanzx.com/gtoucwqqgm.html

PHP:  implode(",", $items);
来源：http://hz.jinqigfzy.top/gtlzbqhood.html

JS:   items.join(",")
来源：http://hz.sxryk.cn/gtjdwotepv.html

TS:   items.join(",")
来源：http://hz.hammf.cn/gtlgjjlqmu.html

Java: String.join(",", items)
来源：http://hz.aizwys.cn/gtikawahjv.html

Go:   strings.Join(items, ",")
来源：http://hz.svipenyu.cn/gtddzoeems.html

Ruby: items.join(",")
来源：http://hz.shangyingyoupin.top/gtgsyzjunt.html

C#:   string.Join(",", items)
来源：http://hz.52xcode.cn/gtqnsiozlj.html

[E09] 去除所有空白字符
来源：http://hz.tian-w.cn/gtsccqpxnw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.pycfn.com/gtwislndbg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.quarkkingdee.top/gtlhiseztn.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jyoumei.cn/gtbbejtvao.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jyoumei.cn/gtvuhbpzjz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tian-w.cn/gtbglwatdw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xingfuxueyuan.xyz/gtmebfxhno.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yj20258888.top/gthszjlgwm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhixingplan.top/gtbptimajl.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yanxiufei.cn/gtmfwmqrxq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.tanke756.top/gtubcmjrbr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gzhubu.top/gtxhokunpk.html

JS:   "7".padStart(3, "0")
来源：http://hz.xingfuxueyuan.xyz/gteppamncp.html

TS:   "7".padStart(3, "0")
来源：http://hz.gotoacloud.top/gtxhohxtmx.html

Java: String.format("%03d", 7)
来源：http://hz.ydjk.org.cn/gtqpzfcnmf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ppjwa.cn/gtmegopprk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.fengsongda.top/gtqalvgern.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yvedp.cn/gtzkpngfvq.html

[E11] 反转字符串
来源：http://hz.vqdsnc.cn/gtksinbyxh.html

Py:   s[::-1]
来源：http://hz.ydjk.org.cn/gtwywaogut.html

PHP:  strrev($s);
来源：http://hz.haohaochexian.top/gtgbinjcvg.html

JS:   [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtzhukkkyo.html

TS:   [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtquuqjqmi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.pengpengdd.cyou/gtigjoldun.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.9152youxi.cn/gtiobkwjll.html

Ruby: s.reverse
来源：http://hz.haohaochexian.top/gthvwwffxw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.tian-w.cn/gtiodihnox.html

[E12] 统计某字符出现次数
来源：http://hz.xziqi.cn/gthchhulbi.html

Py:   s.count("a")
来源：http://hz.c1oappe.top/gttvcalwjo.html

PHP:  substr_count($s, "a");
来源：http://hz.yanxiufei.cn/gtkfrnpckj.html

JS:   s.split("a").length - 1
来源：http://hz.tian-w.cn/gtgugwokuu.html

TS:   s.split("a").length - 1
来源：http://hz.xuanzx.com/gtltmwmpgd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinghuilouyu.cn/gtwzrlweio.html

Go:   strings.Count(s, "a")
来源：http://hz.9152youxi.cn/gtjkieaome.html

Ruby: s.count("a")
来源：http://hz.cheryme.top/gtojhkqvjg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gzhubu.top/gtlouizcqg.html

[E13] 逐字符遍历
来源：http://hz.jinqigufen.top/gtyiivspre.html

Py:   for ch in s: print(ch)
来源：http://hz.redwolf501.top/gtsjkpggms.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.aibaodan.cn/gtrvexspnj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenlongwang.top/gtvmeknarp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gotoacloud.top/gtnnhjzjgu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.0kj1m.cn/gtkutmfmeh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ywan-chungtsiang.top/gtrfppaaaw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhengqikj.top/gtezlheesb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ivvv.top/gttbjteurc.html

[E14] URL 编码与 Base64
来源：http://hz.yangfankeji.com/gtebltfspb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hnxiangtu.top/gtwaggoefy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.smart0.xyz/gtqwyujdra.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.guannengcc.top/gtsqrthnhi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yj20258888.top/gtsiujqkum.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.c1oappe.top/gthlqnbbqi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.fzhhl.top/gtdhxpwusy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jianghu66.top/gtkwzxktuw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xylfe.cn/gtwjtkxkbd.html

[E15] HTML 转义 / 反转义
来源：http://hz.sysykeji.top/gtjrjaycjc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cheryme.top/gtxxvjqypu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hongshengwenyu.top/gtcylafmra.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.gaohongyu789.top/gtkkufgccs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jinqigfzy.top/gthwankkdf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.haohaochexian.top/gtidfqfglf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jianghu66.top/gthqlllwzg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.andypj.xyz/gtppahavyd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xuanzx.com/gtzeamjmbk.html

[E16] 数字千分位
来源：http://hz.daria6918.cn/gtvyxsusni.html

Py:   f"{1234567:,}"
来源：http://hz.cashguo.top/gtcaemlaor.html

PHP:  number_format(1234567);
来源：http://hz.havefunace.top/gtuzemdvsl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuanzx.com/gtnwlbspdu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnqzz.top/gtmhfhveqw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinqigufen.top/gtdunqjkan.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yonumen.top/gtcolvvhfs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.pycfn.com/gtgblwhyhh.html

C#:   1234567.ToString("N0")
来源：http://hz.aibaodan.cn/gtjijfolau.html

[E17] 首字母大写
来源：http://hz.quarkkingdee.top/gtgdopqhjo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zdqjudy.top/gtcmtwezpo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.guannengcc.top/gtpmksxjmr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.bjfxy.top/gtcwlnriwb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zdqjudy.top/gtdikyzlfo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ivvv.top/gtgqlygdjr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hywenlv.cn/gtcqyzdqvm.html

Ruby: s.capitalize
来源：http://hz.meibo888.top/gtpmpsllnv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jiagoushi.top/gtpcujygaw.html

[E18] 模板占位符替换
来源：http://hz.vqdsnc.cn/gtkwcxiaji.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yj20258.top/gtimajbsrn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ybcxt.top/gtmkrxrrub.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.aibaodan.cn/gtqqkytpwd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yvedp.cn/gtymsxjmfk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.kuanghao11.cn/gtknwpcsuf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hywenlv.cn/gtjbubzbjz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yj202588.top/gtekneqzwa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.guowangkeji.top/gtrwlqpvkq.html

[E19] 多行文本按行拆分
来源：http://hz.tianlin.xyz/gtgdjwcznt.html

Py:   s.splitlines()
来源：http://hz.cashguo.top/gtoeophend.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ivvv.top/gtxpzaldjx.html

JS:   s.split(/\r?\n/)
来源：http://hz.yongpay.top/gtjxhzhawx.html

TS:   s.split(/\r?\n/)
来源：http://hz.zycfv.cn/gtackbgyrc.html

Java: s.lines().toList()
来源：http://hz.jyoumei.cn/gtmyzvklwr.html

Go:   strings.Split(s, "\n")
来源：http://hz.cashguo.top/gtcpzvrcav.html

Ruby: s.lines
来源：http://hz.yonumen.top/gtceovvqeb.html

C#:   s.Split('\n')
来源：http://hz.zhaomingkeji.xyz/gtiyjlenov.html

[E20] 判断字符串是否为空
来源：http://hz.xinyue.icu/gtzqjdekew.html

Py:   if not s:
来源：http://hz.jqgfzy.top/gtjzlyfgyc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zycfv.cn/gtcjfmtiap.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cqqwz.cn/gtuywwvokd.html

TS:   if (s === "") {}
来源：http://hz.yangfankeji.com/gtnalgnaom.html

Java: if (s.isEmpty()) {}
来源：http://hz.feifeiyinyue.top/gtexwssaae.html

Go:   if s == "" {}
来源：http://hz.yj202588.top/gtpbtgeywe.html

Ruby: if s.empty?
来源：http://hz.meibo888.top/gtsvwabtii.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.guannengcc.top/gtbbpxrmfx.html

[E21] 超长截断加省略号
来源：http://hz.zhaomingkeji.xyz/gtfsmnncfq.html


<!-- 参考信息 -->