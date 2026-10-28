代发 wailian999

Ruby: arr.index(x)
来源：http://hz.tanke756.top/gtplfxpwjp.html

C#:   list.IndexOf(x);
来源：http://hz.yonumen.top/gttyizjrpf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cqqwz.cn/gtmlqvzptr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hnqzz.top/gtusdninpm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.fzhhl.top/gtdzhgftmw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.daxiang520.top/gtxawtlvcc.html

TS:   arr.filter(x => x > 3)
来源：http://hz.wangshuangyany.cn/gtumjcimvb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sysykeji.top/gtoxjslbxh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj20258888.top/gtdflsdcbm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shzxlz.cn/gtptbdbksq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhongyouzk.top/gtriaiynwf.html

[D14] 映射转换（每个元素变形）
来源：http://hz.vqdsnc.cn/gtszhzvdpg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.daria6918.cn/gtmlcrawpo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.wangshuangyany.cn/gtscloaqcx.html

JS:   arr.map(x => x * 2)
来源：http://hz.feifeiyinyue.top/gteagbhqne.html

TS:   arr.map(x => x * 2)
来源：http://hz.ehwqpu.com/gtwzfsqmxr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.wangdashe.top/gtuxtpxxpn.html

Go:   // 手写循环
来源：http://hz.haohaochexian.top/gtfrkrsjeh.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hnqzz.top/gtupmsauwe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.mhx1999.top/gtyeydqpco.html

[D15] 去重
来源：http://hz.cucudq.cn/gtwtpavgat.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cheryme.top/gtwvjprhou.html

PHP:  array_unique($arr);
来源：http://hz.yongpay.top/gturfnkwjd.html

JS:   [...new Set(arr)]
来源：http://hz.snrcjt.cn/gtwhrihlub.html

TS:   [...new Set(arr)]
来源：http://hz.chenzaomai.com/gtnhnejiio.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.dashuyun.cn/gtmwqicfyf.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.nwbrower.top/gtedqenwde.html

Ruby: arr.uniq
来源：http://hz.kuanghao11.cn/gtjblphdgd.html

C#:   list.Distinct().ToList()
来源：http://hz.guowangkeji.top/gtundxqbxr.html

[D16] 求和与平均值
来源：http://hz.kuanghao11.cn/gttpgvqkbo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.cheryme.top/gtqffzahlb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jinyuanbaomall.cn/gtlnvgvkdw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgufenzy.top/gtxygfmuor.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shanyushiyangtech.top/gtwblewyhq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.daxiang520.top/gtvusmosgx.html

Go:   // 手写循环累加
来源：http://hz.redwolf501.top/gthwsjpbgq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hongshengwenyu.top/gtwjrnrsli.html

C#:   list.Sum();  list.Average()
来源：http://hz.shuidangran.top/gtlscbyhvz.html

[D17] 最大值与最小值
来源：http://hz.vqdsnc.cn/gtjtjykpvw.html

Py:   max(arr);  min(arr)
来源：http://hz.sysykeji.top/gtvjvzsbad.html

PHP:  max($arr);  min($arr);
来源：http://hz.guannengcc.top/gttwyudzrs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.snrcjt.cn/gtzlpqnrig.html

TS:   Math.max(...arr);
来源：http://hz.yuxming.cn/gtsvnqtzld.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.wangdashe.top/gtrgumhitl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yvedp.cn/gtmcdyizyh.html

Ruby: arr.max;  arr.min
来源：http://hz.jqgfzy.top/gteusisgqm.html

C#:   list.Max();  list.Min()
来源：http://hz.xuanzx.com/gtkkjyppxg.html

[D18] 扁平化嵌套数组
来源：http://hz.zhaomingkeji.xyz/gtscryhpyv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hnxiangtu.top/gtvvnkmabo.html

PHP:  array_merge(...$nested);
来源：http://hz.yvedp.cn/gtgefbgddm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.svipenyu.cn/gtgcrvpjwl.html

TS:   nested.flat();
来源：http://hz.gzhubu.top/gtfiqqzhfq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yvedp.cn/gtcbaesjqo.html

Go:   // 手写双层循环
来源：http://hz.c1oappe.top/gtonytfrbq.html

Ruby: nested.flatten
来源：http://hz.xingfuxueyuan.xyz/gtdqwhrubf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hongshengwenyu.top/gtrutyonfq.html

[D19] 按字段分组
来源：http://hz.tian-w.cn/gtdipbzywf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cqqwz.cn/gtgxjebbkg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhixingplan.top/gtjhprbzmk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.52xcode.cn/gtbrowefmk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yj202588.top/gtwitkhhqo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yvedp.cn/gtrohfwoby.html

Go:   // 手写 map[string][]T
来源：http://hz.sxryk.cn/gtqjnxubju.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xziqi.cn/gtuxuvkslq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.c1oappe.top/gtmtkpqgru.html

[D20] 统计每个元素出现次数
来源：http://hz.xingfuxueyuan.xyz/gtrzkhgyfh.html

Py:   Counter(arr)
来源：http://hz.yongpay.top/gtdxnquljo.html

PHP:  array_count_values($arr);
来源：http://hz.yuxming.cn/gtymrrpsye.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yuanzhike.top/gtcwfticjw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sweek.top/gtmntwktqa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.guowangkeji.top/gtzirpbvpu.html

Go:   // 手写 map[T]int
来源：http://hz.chenzaomai.com/gtnbrtxrvg.html

Ruby: arr.tally
来源：http://hz.yueranfly.top/gtctpwisll.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.svipenyu.cn/gtauylhyaq.html

[D21] 判断是否包含某元素
来源：http://hz.dashuyun.cn/gtmmvvucop.html

Py:   x in arr
来源：http://hz.ppjwa.cn/gtsxreecxm.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tian-w.cn/gtonyalcpq.html

JS:   arr.includes(x)
来源：http://hz.iojbl.cn/gtfqaybhmm.html

TS:   arr.includes(x)
来源：http://hz.meibo888.top/gtoonpecrc.html

Java: list.contains(x)
来源：http://hz.jianghu66.top/gtcjfacfdk.html

Go:   slices.Contains(arr, x)
来源：http://hz.shanyushiyangtech.top/gtpmtnpxrc.html

Ruby: arr.include?(x)
来源：http://hz.sysykeji.top/gtzaniedkn.html

C#:   list.Contains(x)
来源：http://hz.ybcxt.top/gtvoahkyho.html

[D22] 复制数组（避免共享引用）
来源：http://hz.nanxinkj.top/gttlykdoev.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.smart0.xyz/gtgzoxpfse.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.nwbrower.top/gtfdwbrvgl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.dashuyun.cn/gtlnzybknj.html

TS:   [...arr];
来源：http://hz.ydzc1.top/gtjlgetxhy.html

Java: new ArrayList<>(list);
来源：http://hz.bjfxy.top/gtswxmotht.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhijiandao.cn/gtehpxnmhn.html

Ruby: arr.dup;  arr.clone
来源：http://hz.52xcode.cn/gtoromfnmj.html

C#:   new List<int>(list);
来源：http://hz.sufxvd.cn/gtezjagkuv.html

[D23] reduce 累积计算
来源：http://hz.nwbrower.top/gtrtvifdek.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.chenzaomai.com/gttpaqnlcn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yangfankeji.com/gtfbinqktc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cheryme.top/gtxvnlfaxh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinqigfzy.top/gtpqoeiyed.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj20258888.top/gtwzufwrpy.html

Go:   // 手写循环
来源：http://hz.wangshuangyany.cn/gtagoadbxc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yuanzhike.top/gtnilfgmrg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jianghu66.top/gtfcbnzrto.html

[D24] 字典 / Map 基本操作
来源：http://hz.chenzaomai.com/gtyqejkelw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.aibaodan.cn/gtoslspask.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jinqigfzy.top/gtkmtlgfdo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jianghu66.top/gtopaohuqz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ehwqpu.com/gtgbfqjwqg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.c1oappe.top/gtkitwmnpc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.9152youxi.cn/gtzrdkpbwm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cashguo.top/gtjtgoivws.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xuanzx.com/gtbfkoanjw.html

[D25] Set 集合去重与交并差
来源：http://hz.wangdashe.top/gtqzjaxymv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ydzc1.top/gtlpmxjxvr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinqigfzy.top/gtjsjxjolj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yuanzhike.top/gtqplqxmnf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.nanxuanxn.top/gtbceyccjr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yuxming.cn/gtsohoqnrq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yonumen.top/gtqcyrtmax.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xuanzx.com/gtsvntdpqd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhiwuduotai.top/gtzrnflxfx.html

[D26] 数组转字符串
来源：http://hz.tianlin.xyz/gtqpahuzaz.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yj20258888.top/gtbjdzidfw.html

PHP:  implode(", ", $arr);
来源：http://hz.daxiang520.top/gticvzmhdp.html

JS:   arr.join(", ")
来源：http://hz.gogol.net.cn/gttkdycvau.html

TS:   arr.join(", ")
来源：http://hz.zhiwuduotai.top/gtwkkdtopn.html

Java: String.join(", ", list)
来源：http://hz.chenjidiqi.icu/gtkcgkuplr.html

Go:   strings.Join(strs, ", ")
来源：http://hz.nwbrower.top/gtkdcsjoyy.html

Ruby: arr.join(", ")
来源：http://hz.zhaomingkeji.xyz/gtqzzphvpo.html

C#:   string.Join(", ", list)
来源：http://hz.jinyuanbaomall.cn/gtsdjnfxal.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtvlvabhsn.html

E. 字符串处理
来源：http://hz.cheryme.top/gtlnrfxdfd.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtzjxepqfb.html

[E01] 拼接字符串
来源：http://hz.kuanghao11.cn/gtzkiueqou.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ydzc1.top/gtktuhomtz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ehwqpu.com/gtfmdvfjuj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.wangshuangyany.cn/gtltwlmgrn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.dianchejie.cn/gttttslyme.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.bjfxy.top/gtpttyfbpb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shuidangran.top/gtdprfvvcy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhiwuduotai.top/gtfdplliol.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.chenzaomai.com/gtmygippmb.html

[E02] 重复字符串
来源：http://hz.havefunace.top/gtoduscrbh.html

Py:   "ab" * 3
来源：http://hz.tian-w.cn/gtrcoolnyg.html

PHP:  str_repeat("ab", 3);
来源：http://hz.havefunace.top/gtncdbeylq.html

JS:   "ab".repeat(3)
来源：http://hz.jqgufenzy.top/gtxwngisnd.html

TS:   "ab".repeat(3)
来源：http://hz.ivvv.top/gtptplboig.html

Java: "ab".repeat(3)
来源：http://hz.yueranfly.top/gtocgpjbhj.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ydjk.org.cn/gtsprlibmk.html

Ruby: "ab" * 3
来源：http://hz.xuetiantiany.cn/gtdwlyhdrk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.wangdashe.top/gtqzuaqixa.html

[E03] 截取子串
来源：http://hz.jqgfzy.top/gtgdcsdpmt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.tian-w.cn/gtkwqniniy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yuxming.cn/gtfqvkiaay.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jqgufenzy.top/gtqdxhfklg.html

TS:   s.slice(1, 4)
来源：http://hz.zhijiandao.cn/gtntyxudem.html

Java: s.substring(1, 4)
来源：http://hz.feifeiyinyue.top/gtoidaptop.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.snrcjt.cn/gtsopjxdum.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhiwuduotai.top/gtrzjrrthv.html

C#:   s.Substring(1, 3)
来源：http://hz.sysykeji.top/gtqvgusjrj.html

[E04] 查找子串位置
来源：http://hz.zhixingplan.top/gtalqgczte.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhengqikj.top/gtjcdbwcux.html

PHP:  strpos($s, "x");
来源：http://hz.aibaodan.cn/gtaehfdmcd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jinyuanbaomall.cn/gteebbkvnv.html

TS:   s.indexOf("x")
来源：http://hz.haohaochexian.top/gtblwixljp.html

Java: s.indexOf("x")
来源：http://hz.zdqjudy.top/gtzlgmyuwr.html

Go:   strings.Index(s, "x")
来源：http://hz.zycfv.cn/gtiylwbnrb.html

Ruby: s.index("x")
来源：http://hz.hywenlv.cn/gtmtwhgkqi.html

C#:   s.IndexOf("x")
来源：http://hz.feifeiyinyue.top/gtbgwmhbzn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.fengsongda.top/gtjtvoesxc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.pycfn.com/gtcluvavtn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shuidangran.top/gtuecpacxk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.guannengcc.top/gtoqxkdgna.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cucudq.cn/gtxglspiru.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhaomingkeji.xyz/gtrefgrhse.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hnqzz.top/gtnkgscagr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.andypj.xyz/gtxndxqxco.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hongshengwenyu.top/gtwbkxjjlr.html

[E06] 替换子串
来源：http://hz.smart0.xyz/gtwvfsymwg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.nwbrower.top/gtcnbzzxbc.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.wangdashe.top/gtbdkpvykn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhijiandao.cn/gtrfogkrxx.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yj20258.top/gtazzwgojp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtulanfeyu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.bjfxy.top/gtirfuahny.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.fengsongda.top/gtxvciomke.html

C#:   s.Replace("a", "b")
来源：http://hz.yonumen.top/gtyzwgjmgj.html

[E07] 按分隔符拆分
来源：http://hz.smart0.xyz/gtoqznvcbo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.tanke756.top/gtfupijino.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ybcxt.top/gtstfkxhxk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yanxiufei.cn/gtuqpskuiq.html

TS:   s.split(",")
来源：http://hz.bjfxy.top/gtbracqbrr.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.aibaodan.cn/gtufftcfcc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.aizwys.cn/gtbyfovbvj.html

Ruby: s.split(",");  s.split
来源：http://hz.jinqigufen.top/gttzgkyfya.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.wangshuangyany.cn/gtdssxortb.html

[E08] 数组按分隔符合并
来源：http://hz.wangdashe.top/gtyqllhmiu.html

Py:   ",".join(items)
来源：http://hz.9152youxi.cn/gtirgdmmfb.html

PHP:  implode(",", $items);
来源：http://hz.yonumen.top/gtpibnvbtp.html

JS:   items.join(",")
来源：http://hz.jqgfzy.top/gtulhdwcwa.html

TS:   items.join(",")
来源：http://hz.shangyingyoupin.top/gtiidojafj.html

Java: String.join(",", items)
来源：http://hz.yuxming.cn/gtomfojkhc.html

Go:   strings.Join(items, ",")
来源：http://hz.sysykeji.top/gtcgrcmybn.html

Ruby: items.join(",")
来源：http://hz.birdmap.top/gtaeufkqzy.html

C#:   string.Join(",", items)
来源：http://hz.pengpengdd.cyou/gtbqqyogjc.html

[E09] 去除所有空白字符
来源：http://hz.dianchejie.cn/gtumsgnrya.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhengqikj.top/gtjekhorlj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ydzc1.top/gtwzhgoudq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yj202588.top/gtckjkbnkp.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hnqzz.top/gtnagqnbti.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.haohaochexian.top/gtxywcxjqh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhiwuduotai.top/gtdkewasaz.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.tian-w.cn/gtqtbwfnij.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.dashuyun.cn/gthewqxsbg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhiwuduotai.top/gtyizlwisn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenlongwang.top/gtloofoizv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.andypj.xyz/gtzjyhgpyb.html

JS:   "7".padStart(3, "0")
来源：http://hz.xuetiantiany.cn/gtheifesmf.html

TS:   "7".padStart(3, "0")
来源：http://hz.hnxiangtu.top/gtsxjflhdd.html

Java: String.format("%03d", 7)
来源：http://hz.hnqzz.top/gtrgmoglbx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shanyushiyangkeji.top/gtzdevcyxh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yj20258888.top/gtaolsinwy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenzaomai.com/gtgxpvgwry.html

[E11] 反转字符串
来源：http://hz.smart0.xyz/gtucoywyms.html

Py:   s[::-1]
来源：http://hz.jinyuanbaomall.cn/gtnadtokam.html

PHP:  strrev($s);
来源：http://hz.xuanzx.com/gtcxuhbgjm.html

JS:   [...s].reverse().join("")
来源：http://hz.xylfe.cn/gtaedmbspd.html

TS:   [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtgilagihb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xylfe.cn/gtkdstxrcj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.iojbl.cn/gtgeurfxgc.html

Ruby: s.reverse
来源：http://hz.yuxming.cn/gtnshzkkim.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.redwolf501.top/gtcbidauvi.html

[E12] 统计某字符出现次数
来源：http://hz.ybcxt.top/gtpytbbhdc.html

Py:   s.count("a")
来源：http://hz.daxiang520.top/gthgdrodug.html

PHP:  substr_count($s, "a");
来源：http://hz.9152youxi.cn/gtjxehckyy.html

JS:   s.split("a").length - 1
来源：http://hz.havefunace.top/gtqochqdmi.html

TS:   s.split("a").length - 1
来源：http://hz.jiagoushi.top/gttitzxvan.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.dianchejie.cn/gtrmbfqjli.html

Go:   strings.Count(s, "a")
来源：http://hz.shzxlz.cn/gtywwsutfy.html

Ruby: s.count("a")
来源：http://hz.shangyingyoupin.top/gtiessyysi.html

C#:   s.Count(c => c == 'a')
来源：http://hz.chenzaomai.com/gtepbvvzvy.html

[E13] 逐字符遍历
来源：http://hz.meibo888.top/gtpfpftebm.html

Py:   for ch in s: print(ch)
来源：http://hz.yj20258.top/gtomcarwvn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gaohongyu789.top/gtrsignjoi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhongyouzk.top/gtjsglklgh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xinyue.icu/gtqmiqvosv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yueranfly.top/gtqycogkks.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yonumen.top/gtoyrnswvb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jyoumei.cn/gtuwmhyhig.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hywenlv.cn/gtfsgqewga.html

[E14] URL 编码与 Base64
来源：http://hz.fzhhl.top/gtxjamwftg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xuetiantiany.cn/gtzfqgwebe.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hywenlv.cn/gtjfgrlovx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhixingplan.top/gtskyyekdt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.fzhhl.top/gtukkbvxtk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.feifeiyinyue.top/gtnpfhxhxg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yongpay.top/gtaudumjpq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jqgufenzy.top/gtuyojzczi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.pengpengdd.cyou/gtncuvnfjx.html

[E15] HTML 转义 / 反转义
来源：http://hz.sufxvd.cn/gtvkspgjpf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zycfv.cn/gtojuxpjfc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yueranfly.top/gtpzcvygcy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xylfe.cn/gttfszjjgo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guowangkeji.top/gtclmwmvvh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xylfe.cn/gtaugzacau.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.guannengcc.top/gtciuwbqhz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xuetiantiany.cn/gtvrthpueb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.bjfxy.top/gtsigkocrc.html

[E16] 数字千分位
来源：http://hz.yueranfly.top/gtgztlheai.html

Py:   f"{1234567:,}"
来源：http://hz.meibo888.top/gtostmlhlu.html

PHP:  number_format(1234567);
来源：http://hz.xuetiantiany.cn/gtmpomqkii.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.andypj.xyz/gtwgeobfdu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.redwolf501.top/gtavnsajtx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.feifeiyinyue.top/gtwytdygoz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj202588.top/gtfaqzochi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jinyuanbaomall.cn/gtzjjabnao.html

C#:   1234567.ToString("N0")
来源：http://hz.yj20258888.top/gthryaqlpe.html

[E17] 首字母大写
来源：http://hz.yj202588.top/gtryhczyhn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.316326.xyz/gtcmfmjwfn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yj202588.top/gtqycoersl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinghuilouyu.cn/gtytmpymma.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhongyouzk.top/gtraeyxncr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xuetiantiany.cn/gttdwushbb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhengqikj.top/gtugshzlow.html

Ruby: s.capitalize
来源：http://hz.shangyingyoupin.top/gtokrrnizp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yonumen.top/gtvhnufjxu.html

[E18] 模板占位符替换
来源：http://hz.shanyushiyangkeji.top/gtribyqdal.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hfpthk.cn/gtzbnhaign.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.meibo888.top/gtefeuwerl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hongshengwenyu.top/gtfdyqpuro.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.feifeiyinyue.top/gtcenpkxwy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtrfdrfnok.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.0kj1m.cn/gtqavsqhah.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.tanke756.top/gtipusdfjr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ydzc1.top/gtfgzkrcaj.html

[E19] 多行文本按行拆分
来源：http://hz.jinyuanbaomall.cn/gtfxxagkoz.html

Py:   s.splitlines()
来源：http://hz.ydzc1.top/gtfacoauab.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hammf.cn/gtmdcrsuty.html

JS:   s.split(/\r?\n/)
来源：http://hz.nanxinkj.top/gtfbilueqg.html

TS:   s.split(/\r?\n/)
来源：http://hz.yj20258.top/gtbtcbawqe.html

Java: s.lines().toList()
来源：http://hz.yj20258888.top/gtndbexvab.html

Go:   strings.Split(s, "\n")
来源：http://hz.cqqwz.cn/gtupmifnxb.html


<!-- 参考信息 -->