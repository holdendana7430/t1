代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xuanzx.com/gtwhxxixvg.html

C#:   list.Sum();  list.Average()
来源：http://hz.316326.xyz/gtzaovsash.html

[D17] 最大值与最小值
来源：http://hz.fengsongda.top/gtyuqslspt.html

Py:   max(arr);  min(arr)
来源：http://hz.andypj.xyz/gtscgnkhjv.html

PHP:  max($arr);  min($arr);
来源：http://hz.cucudq.cn/gtvmvkwxys.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.aizwys.cn/gtrzgtggcl.html

TS:   Math.max(...arr);
来源：http://hz.daria6918.cn/gtrvtgbcga.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.shzxlz.cn/gtziumukeu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cucudq.cn/gtemrgntxv.html

Ruby: arr.max;  arr.min
来源：http://hz.tianlin.xyz/gtnrstofhp.html

C#:   list.Max();  list.Min()
来源：http://hz.mhx1999.top/gtblhnwutn.html

[D18] 扁平化嵌套数组
来源：http://hz.yanxiufei.cn/gtbgsefibl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.tanke756.top/gtkjhfqeug.html

PHP:  array_merge(...$nested);
来源：http://hz.cucudq.cn/gtmwyxeidj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yonumen.top/gtxntlvtqo.html

TS:   nested.flat();
来源：http://hz.jlsjyb.cn/gtpudnccpl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.redwolf501.top/gtikcfieoq.html

Go:   // 手写双层循环
来源：http://hz.guannengcc.top/gtpqkwhzkk.html

Ruby: nested.flatten
来源：http://hz.gaohongyu789.top/gtsawpeueq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhoulong.xyz/gtdtgrhggs.html

[D19] 按字段分组
来源：http://hz.316326.xyz/gtmmhwdekg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yuxming.cn/gtolyqkffm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xingfuxueyuan.xyz/gtizamyzau.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hnxiangtu.top/gtjsnyutkj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xylfe.cn/gtijxwiiuz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cqqwz.cn/gtkikvutjo.html

Go:   // 手写 map[string][]T
来源：http://hz.shanyushiyangkeji.top/gtgfjbqvjt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xingfuxueyuan.xyz/gtnhyabyph.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yongpay.top/gtqhlmpuex.html

[D20] 统计每个元素出现次数
来源：http://hz.guowangkeji.top/gtavgjxvzo.html

Py:   Counter(arr)
来源：http://hz.0kj1m.cn/gtjcazjtkv.html

PHP:  array_count_values($arr);
来源：http://hz.hongshengwenyu.top/gtzkwbwwrb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.daxiang520.top/gtmidlirjp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yanxiufei.cn/gtxyxecnnp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cdnleiting.top/gtdrgolclb.html

Go:   // 手写 map[T]int
来源：http://hz.meibo888.top/gtjvsbflrn.html

Ruby: arr.tally
来源：http://hz.jlsjyb.cn/gtswbfcozp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.pycfn.com/gtvbhrkvap.html

[D21] 判断是否包含某元素
来源：http://hz.zhixingplan.top/gtyeadjyuw.html

Py:   x in arr
来源：http://hz.xingfuxueyuan.xyz/gtmfdvbtnj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.c1oappe.top/gtgszvmtfw.html

JS:   arr.includes(x)
来源：http://hz.chenlongwang.top/gtfrgcbbyz.html

TS:   arr.includes(x)
来源：http://hz.fzhhl.top/gtlujtumnb.html

Java: list.contains(x)
来源：http://hz.jinqigufen.top/gtiagvwrlf.html

Go:   slices.Contains(arr, x)
来源：http://hz.tianlin.xyz/gtfgbvxxkv.html

Ruby: arr.include?(x)
来源：http://hz.aibaodan.cn/gtmmihxzox.html

C#:   list.Contains(x)
来源：http://hz.yj20258888.top/gttgoojwrt.html

[D22] 复制数组（避免共享引用）
来源：http://hz.daxiang520.top/gtndgxulsf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.mhx1999.top/gtjiwhgdux.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.pengpengdd.cyou/gthpvtxvas.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hfpthk.cn/gtncsibtpw.html

TS:   [...arr];
来源：http://hz.quarkkingdee.top/gtwcaijxxy.html

Java: new ArrayList<>(list);
来源：http://hz.pycfn.com/gtiiukmgcp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ppjwa.cn/gtnlufsneh.html

Ruby: arr.dup;  arr.clone
来源：http://hz.chenlongwang.top/gtwknaguia.html

C#:   new List<int>(list);
来源：http://hz.ywan-chungtsiang.top/gtusevfwnj.html

[D23] reduce 累积计算
来源：http://hz.yuxming.cn/gtgwzyyzhg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ybcxt.top/gtnprgcers.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yangfankeji.com/gthmbcnmss.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cucudq.cn/gtrnwxddkc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gaohongyu789.top/gtgzlvmzxw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhijiandao.cn/gtlxqvzwxo.html

Go:   // 手写循环
来源：http://hz.havefunace.top/gtlbmrhjfg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cdnleiting.top/gtxxcbtsey.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jqgfzy.top/gtqkbgvdyq.html

[D24] 字典 / Map 基本操作
来源：http://hz.pycfn.com/gtiphdfpli.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yj202588.top/gtljpxcqqp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.vqdsnc.cn/gtcrskviki.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhiwuduotai.top/gtwyndurqa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ydzc1.top/gtwwbzhpwy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.birdmap.top/gtwrjwbszm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.kuanghao11.cn/gtyccktoap.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shzxlz.cn/gtuvsvbglc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.iojbl.cn/gtrfijhnsp.html

[D25] Set 集合去重与交并差
来源：http://hz.meibo888.top/gtibtandnu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.andypj.xyz/gturqgfhmx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yuanzhike.top/gtpadovixt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.andypj.xyz/gtvtllalmu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sweek.top/gtqiacbjjj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.bjfxy.top/gtckiefosx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ehwqpu.com/gtdngyzzbp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yonumen.top/gtubvudyac.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yueranfly.top/gtaajwwrag.html

[D26] 数组转字符串
来源：http://hz.chenlongwang.top/gtiaqzyauq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.redwolf501.top/gtedbivwoo.html

PHP:  implode(", ", $arr);
来源：http://hz.52xcode.cn/gtmlrzdynr.html

JS:   arr.join(", ")
来源：http://hz.cucudq.cn/gtlxkfyahq.html

TS:   arr.join(", ")
来源：http://hz.yj202588.top/gthstpbqvo.html

Java: String.join(", ", list)
来源：http://hz.zhijiandao.cn/gtgvslyoxu.html

Go:   strings.Join(strs, ", ")
来源：http://hz.sweek.top/gtgnpplfxh.html

Ruby: arr.join(", ")
来源：http://hz.jianghu66.top/gtnnitsvdx.html

C#:   string.Join(", ", list)
来源：http://hz.yj20258.top/gtqqpbeiae.html

================================================================================
来源：http://hz.hnxiangtu.top/gtfujhzjdj.html

E. 字符串处理
来源：http://hz.jiagoushi.top/gtveaornmx.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtzchhnpsq.html

[E01] 拼接字符串
来源：http://hz.shzxlz.cn/gtlnwkchcz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xingfuxueyuan.xyz/gtphkthzpx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhiwuduotai.top/gtfhddenmo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydjk.org.cn/gtikeytuxq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenzaomai.com/gteuwjuaiy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.guannengcc.top/gtfanibsdp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yvedp.cn/gtvvzyxyfb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.birdmap.top/gtfgshtqnh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shuidangran.top/gtxdvykpqx.html

[E02] 重复字符串
来源：http://hz.jinqigfzy.top/gtirtjvxfs.html

Py:   "ab" * 3
来源：http://hz.xuanzx.com/gtkxtkmyws.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cheryme.top/gtdlrgxcvu.html

JS:   "ab".repeat(3)
来源：http://hz.redwolf501.top/gtqpqbejvd.html

TS:   "ab".repeat(3)
来源：http://hz.guowangkeji.top/gtbljifbsq.html

Java: "ab".repeat(3)
来源：http://hz.tianlin.xyz/gtvlhmhdha.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jinqigufen.top/gtrfflwyxc.html

Ruby: "ab" * 3
来源：http://hz.hnqzz.top/gtaenwdswg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jinghuilouyu.cn/gtdtiizchq.html

[E03] 截取子串
来源：http://hz.xuanzx.com/gttsnvlusw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xuetiantiany.cn/gtgvskckfe.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yanxiufei.cn/gtijjvkfbd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yj20258888.top/gtblifdlbo.html

TS:   s.slice(1, 4)
来源：http://hz.yueranfly.top/gtmxvffipw.html

Java: s.substring(1, 4)
来源：http://hz.hongshengwenyu.top/gturtlxbar.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jyoumei.cn/gtwyecbzva.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.guannengcc.top/gttxbkfdup.html

C#:   s.Substring(1, 3)
来源：http://hz.tanke756.top/gtziwrtbsc.html

[E04] 查找子串位置
来源：http://hz.havefunace.top/gththsnqpn.html

Py:   s.find("x");  s.index("x")
来源：http://hz.tian-w.cn/gtjbvozhnq.html

PHP:  strpos($s, "x");
来源：http://hz.0kj1m.cn/gtxogjhbqk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.tanke756.top/gthfmvwlsn.html

TS:   s.indexOf("x")
来源：http://hz.nwbrower.top/gtwjydfszt.html

Java: s.indexOf("x")
来源：http://hz.shzxlz.cn/gtqdhygacb.html

Go:   strings.Index(s, "x")
来源：http://hz.jiagoushi.top/gtfjonldwq.html

Ruby: s.index("x")
来源：http://hz.xziqi.cn/gthufojnrt.html

C#:   s.IndexOf("x")
来源：http://hz.zhiwuduotai.top/gtbqqzwvuf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhijiandao.cn/gtapjrplum.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhaomingkeji.xyz/gtryapxudq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.fzhhl.top/gtltyrnnut.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yuxming.cn/gtwyddhwmn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.andypj.xyz/gtyiwktvsf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shanyushiyangkeji.top/gtqdfuxqfd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yonumen.top/gtlqbevhcv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.c1oappe.top/gtqgkidqde.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ppjwa.cn/gtvriwutbb.html

[E06] 替换子串
来源：http://hz.0kj1m.cn/gtycfzeoog.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.pycfn.com/gtexokzmvs.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.mhx1999.top/gtketjlwjc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.wangdashe.top/gtnsnxgvxw.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cheryme.top/gtblolzmih.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj202588.top/gtiwbziktm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.tanke756.top/gtfloiafju.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.tianlin.xyz/gtjfefudjx.html

C#:   s.Replace("a", "b")
来源：http://hz.yueranfly.top/gtrfabsfhv.html

[E07] 按分隔符拆分
来源：http://hz.zhijiandao.cn/gtrzxtjuos.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.mhx1999.top/gttfetqesl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.aizwys.cn/gtjusokaft.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cqqwz.cn/gtotbmhkrm.html

TS:   s.split(",")
来源：http://hz.iojbl.cn/gttiskunbe.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.nanxuanxn.top/gtbndccfap.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.chenlongwang.top/gtuvjhtpzf.html

Ruby: s.split(",");  s.split
来源：http://hz.52xcode.cn/gtslmdjcll.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.feifeiyinyue.top/gtdsixuxrz.html

[E08] 数组按分隔符合并
来源：http://hz.ydzc1.top/gtgwljxxbm.html

Py:   ",".join(items)
来源：http://hz.ydzc1.top/gtrtcndazu.html

PHP:  implode(",", $items);
来源：http://hz.jiagoushi.top/gtfjkzmjqj.html

JS:   items.join(",")
来源：http://hz.gogol.net.cn/gtzxbkcyii.html

TS:   items.join(",")
来源：http://hz.cheryme.top/gtrpcqotik.html

Java: String.join(",", items)
来源：http://hz.havefunace.top/gteprhdipq.html

Go:   strings.Join(items, ",")
来源：http://hz.wangshuangyany.cn/gtcouzqcup.html

Ruby: items.join(",")
来源：http://hz.zhixingplan.top/gtzuircxle.html

C#:   string.Join(",", items)
来源：http://hz.ivvv.top/gttpgksybs.html

[E09] 去除所有空白字符
来源：http://hz.ehwqpu.com/gtxcotxkdn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zdqjudy.top/gtvrghnwgv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yangfankeji.com/gtwauukbjc.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenlongwang.top/gtrarcaumc.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangkeji.top/gtyigbvxqj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xziqi.cn/gtwjkyqbgj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sufxvd.cn/gtmznpkwlu.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.chenzaomai.com/gthysrjnvx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jlsjyb.cn/gtjdxcntjo.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cdnleiting.top/gtmmrjuthw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhiwuduotai.top/gtbweojwor.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gzhubu.top/gtbxawqnpa.html

JS:   "7".padStart(3, "0")
来源：http://hz.ydzc1.top/gtgwjoohin.html

TS:   "7".padStart(3, "0")
来源：http://hz.gogol.net.cn/gtsqsoojzr.html

Java: String.format("%03d", 7)
来源：http://hz.hnqzz.top/gtqllxeivd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yj20258888.top/gtakthdgta.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jinqigufen.top/gttmzezbns.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.gogol.net.cn/gtfgsmlkfp.html

[E11] 反转字符串
来源：http://hz.jlsjyb.cn/gtbuechlvj.html

Py:   s[::-1]
来源：http://hz.yj202588.top/gtgyoskboy.html

PHP:  strrev($s);
来源：http://hz.zhijiandao.cn/gtsivpqwop.html

JS:   [...s].reverse().join("")
来源：http://hz.ydzc1.top/gtjkxrkczg.html

TS:   [...s].reverse().join("")
来源：http://hz.cheryme.top/gtfyqshrfc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xziqi.cn/gtwzwkqaml.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jqgfzy.top/gtnbzhmqge.html

Ruby: s.reverse
来源：http://hz.ywan-chungtsiang.top/gtpwqdtotj.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.feifeiyinyue.top/gtmngpylqg.html

[E12] 统计某字符出现次数
来源：http://hz.yvedp.cn/gtwkouqhvc.html

Py:   s.count("a")
来源：http://hz.zdqjudy.top/gtbkcqvvek.html

PHP:  substr_count($s, "a");
来源：http://hz.jlsjyb.cn/gttoqstgfn.html

JS:   s.split("a").length - 1
来源：http://hz.ehwqpu.com/gtxvjxtrhc.html

TS:   s.split("a").length - 1
来源：http://hz.haohaochexian.top/gtombgcoin.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ehwqpu.com/gtigsogeuz.html

Go:   strings.Count(s, "a")
来源：http://hz.shanyushiyangtech.top/gterokoaul.html

Ruby: s.count("a")
来源：http://hz.smart0.xyz/gtajzlmksp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.havefunace.top/gtzbmnnnuw.html

[E13] 逐字符遍历
来源：http://hz.cashguo.top/gtfofophok.html

Py:   for ch in s: print(ch)
来源：http://hz.cqqwz.cn/gtswsdzqpw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.tian-w.cn/gtrfoqavgh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.kuanghao11.cn/gtmbbbipff.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhongyouzk.top/gtzndmjxsk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jiagoushi.top/gtdaxypjqx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ydjk.org.cn/gtqipxzbjr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yj20258.top/gtwmsvaswd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.dashuyun.cn/gtlraprblr.html

[E14] URL 编码与 Base64
来源：http://hz.yuanzhike.top/gtuvmhkssb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.cqqwz.cn/gtdlgxzxgd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jlsjyb.cn/gtmctkzama.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jinqigfzy.top/gtbbyygylf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ydzc1.top/gttzqtyxhu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yangfankeji.com/gtrdkttpfc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhengqikj.top/gtysvcujtm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhoulong.xyz/gtjxiglcgu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yueranfly.top/gtacmakwpf.html

[E15] HTML 转义 / 反转义
来源：http://hz.gotoacloud.top/gtnhdjkofr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.quarkkingdee.top/gtajrqykzn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.birdmap.top/gtkvaunetb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yueranfly.top/gtoxuapwrt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jinqigufen.top/gtiurdpfcx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.nwbrower.top/gtgvtlyaxm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.iojbl.cn/gtnpuvmrlr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sufxvd.cn/gtzqnewqcg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.chenjidiqi.icu/gtiyatzncr.html

[E16] 数字千分位
来源：http://hz.gaohongyu789.top/gtomnnlpdo.html

Py:   f"{1234567:,}"
来源：http://hz.jlsjyb.cn/gtjwciribg.html

PHP:  number_format(1234567);
来源：http://hz.zhiwuduotai.top/gtdoqwkwrm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.bjfxy.top/gteiubpqnp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zdqjudy.top/gtevgwegax.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.bjfxy.top/gtketosrws.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.kuanghao11.cn/gtvgbgbwxn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenjidiqi.icu/gtavrqohus.html

C#:   1234567.ToString("N0")
来源：http://hz.kuanghao11.cn/gtavbaxoan.html

[E17] 首字母大写
来源：http://hz.xingfuxueyuan.xyz/gtcpnsngzl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.feifeiyinyue.top/gtrqfoggtq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ppjwa.cn/gtuzjwbtfa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zycfv.cn/gtzdgthxsa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydzc1.top/gtwdjklyek.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ywan-chungtsiang.top/gtrzsxglco.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.chenzaomai.com/gtnjbqixyt.html

Ruby: s.capitalize
来源：http://hz.jqgfzy.top/gtgicppijn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinyuanbaomall.cn/gtdoeapaga.html

[E18] 模板占位符替换
来源：http://hz.jinyuanbaomall.cn/gttmsndieo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.daria6918.cn/gtruoirjux.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yj20258888.top/gtngqkrpru.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cucudq.cn/gtwrolzkxb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhixingplan.top/gtwewqailw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtflfejcmz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ydzc1.top/gtbxupvjdk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhaomingkeji.xyz/gtfzhpazpx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yonumen.top/gtrwhfnkxs.html

[E19] 多行文本按行拆分
来源：http://hz.yonumen.top/gtssnvmtty.html

Py:   s.splitlines()
来源：http://hz.yvedp.cn/gtfpphzpcd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhengqikj.top/gtzazpgate.html

JS:   s.split(/\r?\n/)
来源：http://hz.ywan-chungtsiang.top/gtvjwzjgll.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhoulong.xyz/gtnuzpgtod.html

Java: s.lines().toList()
来源：http://hz.kuanghao11.cn/gtmbacchfg.html

Go:   strings.Split(s, "\n")
来源：http://hz.xingfuxueyuan.xyz/gttvmcplaa.html

Ruby: s.lines
来源：http://hz.mhx1999.top/gtwudzkosv.html

C#:   s.Split('\n')
来源：http://hz.jqgufenzy.top/gtkcrebpjc.html

[E20] 判断字符串是否为空
来源：http://hz.jqgufenzy.top/gtyalnfpre.html

Py:   if not s:
来源：http://hz.andypj.xyz/gtuzeezakc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.kuanghao11.cn/gtpjfhsiqr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinghuilouyu.cn/gtspygedqh.html

TS:   if (s === "") {}
来源：http://hz.birdmap.top/gtbndhnobp.html

Java: if (s.isEmpty()) {}
来源：http://hz.guowangkeji.top/gtwcqrbont.html

Go:   if s == "" {}
来源：http://hz.hammf.cn/gtiwfilzut.html

Ruby: if s.empty?
来源：http://hz.hongshengwenyu.top/gtrfzehbww.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.shangyingyoupin.top/gtvtmpofku.html

[E21] 超长截断加省略号
来源：http://hz.yonumen.top/gtmfhuzwap.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.chenlongwang.top/gtamwnydgf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.vqdsnc.cn/gtdhbzftml.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yongpay.top/gtksrppjpb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tanke756.top/gtuxmwxqhv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.aizwys.cn/gturimgcnk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.sweek.top/gtpqkmbkpi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shanyushiyangtech.top/gtdmqofrcr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhixingplan.top/gtrwxahrak.html

[E22] 字节长度与字符长度
来源：http://hz.yueranfly.top/gttdkkakjt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yueranfly.top/gtnpzyuxpy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tanke756.top/gtctpcijip.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.quarkkingdee.top/gtczwdlizn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangtech.top/gtkxsgnmxk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xinyue.icu/gtnlfclplm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhixingplan.top/gtjdzeozzr.html

Ruby: s.bytesize;  s.length
来源：http://hz.gaohongyu789.top/gtakykupuf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hfpthk.cn/gtpxzrlhmd.html

================================================================================
来源：http://hz.guowangkeji.top/gtmgdfjccp.html

F. 文件与目录
来源：http://hz.xingfuxueyuan.xyz/gtnpmamiex.html

================================================================================
来源：http://hz.mhx1999.top/gtjkvxkfwq.html

[F01] 读取整个文件
来源：http://hz.jinghuilouyu.cn/gtslqdwzhl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hywenlv.cn/gtdxqeamab.html

PHP:  file_get_contents("a.txt");
来源：http://hz.guannengcc.top/gtpcudgtzg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yuanzhike.top/gtyiaehugb.html


<!-- 参考信息 -->