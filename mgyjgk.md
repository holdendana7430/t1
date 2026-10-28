代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.sxryk.cn/gtlbqpyrvf.html

Go:   // 手写循环
来源：http://hz.wangdashe.top/gtdwrpnatd.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.chenjidiqi.icu/gtbnrgpalj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ppjwa.cn/gtixgryxkv.html

[D15] 去重
来源：http://hz.snrcjt.cn/gtqcnxrwam.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.gotoacloud.top/gtuwbpmahu.html

PHP:  array_unique($arr);
来源：http://hz.zhijiandao.cn/gtbswxcxvv.html

JS:   [...new Set(arr)]
来源：http://hz.yj20258.top/gtbxxbxxyw.html

TS:   [...new Set(arr)]
来源：http://hz.hysaishi.cn/gtlzrhqpeb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zdqjudy.top/gttyhfduvm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yangfankeji.com/gtuzzovtmu.html

Ruby: arr.uniq
来源：http://hz.ehwqpu.com/gtowsafcpz.html

C#:   list.Distinct().ToList()
来源：http://hz.zhijiandao.cn/gtxcvwtrfy.html

[D16] 求和与平均值
来源：http://hz.tianlin.xyz/gtoiuptaev.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.meibo888.top/gtmcymoaua.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yj202588.top/gtyxohsmip.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.havefunace.top/gtggcqcxbg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shuidangran.top/gtxulillvn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.iojbl.cn/gtlahsjqtw.html

Go:   // 手写循环累加
来源：http://hz.yvedp.cn/gtmqfxznxe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.wangshuangyany.cn/gtmlikeytl.html

C#:   list.Sum();  list.Average()
来源：http://hz.yj202588.top/gtukbiaeda.html

[D17] 最大值与最小值
来源：http://hz.tanke756.top/gtaqedveua.html

Py:   max(arr);  min(arr)
来源：http://hz.svipenyu.cn/gtafetgruo.html

PHP:  max($arr);  min($arr);
来源：http://hz.jyoumei.cn/gtliobmrbs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.birdmap.top/gtjczqxnes.html

TS:   Math.max(...arr);
来源：http://hz.gotoacloud.top/gtdbbjlvfp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.wangdashe.top/gtnukeigez.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.meibo888.top/gtgagfdjib.html

Ruby: arr.max;  arr.min
来源：http://hz.chenlongwang.top/gtcynpzzmd.html

C#:   list.Max();  list.Min()
来源：http://hz.yongpay.top/gttprngmhg.html

[D18] 扁平化嵌套数组
来源：http://hz.cheryme.top/gtyuvncshm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.aizwys.cn/gtstbtwbqe.html

PHP:  array_merge(...$nested);
来源：http://hz.ybcxt.top/gtltseqznt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yj20258.top/gtxwudbdoh.html

TS:   nested.flat();
来源：http://hz.chenjidiqi.icu/gtztawhdco.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ehwqpu.com/gtcexnctsd.html

Go:   // 手写双层循环
来源：http://hz.tian-w.cn/gtyitlakda.html

Ruby: nested.flatten
来源：http://hz.52xcode.cn/gtutwovdty.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.9152youxi.cn/gtdntqegzj.html

[D19] 按字段分组
来源：http://hz.hywenlv.cn/gtlrbxrpdg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.tian-w.cn/gthumhzwtg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.kuanghao11.cn/gtgqsizojw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.tian-w.cn/gtrifcrsty.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gotoacloud.top/gtghhuxtfn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.aizwys.cn/gtinanucel.html

Go:   // 手写 map[string][]T
来源：http://hz.zhiwuduotai.top/gtaudwaaea.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.daria6918.cn/gtzbdudyta.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.redwolf501.top/gtjufaidnz.html

[D20] 统计每个元素出现次数
来源：http://hz.hysaishi.cn/gtaunhucmu.html

Py:   Counter(arr)
来源：http://hz.gzhubu.top/gtxdleebyy.html

PHP:  array_count_values($arr);
来源：http://hz.hnxiangtu.top/gtdjluxyqe.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tanke756.top/gtzgksrxrc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigfzy.top/gtephwntaw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.vqdsnc.cn/gtdmhsqkbm.html

Go:   // 手写 map[T]int
来源：http://hz.guannengcc.top/gtftyqclws.html

Ruby: arr.tally
来源：http://hz.wangshuangyany.cn/gtbwqasmfj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhijiandao.cn/gtlpysccau.html

[D21] 判断是否包含某元素
来源：http://hz.yanxiufei.cn/gtfumqzjdh.html

Py:   x in arr
来源：http://hz.jlsjyb.cn/gtvwbiroek.html

PHP:  in_array($x, $arr, true);
来源：http://hz.nanxinkj.top/gtefcqalts.html

JS:   arr.includes(x)
来源：http://hz.hfpthk.cn/gtprfjiqjy.html

TS:   arr.includes(x)
来源：http://hz.fzhhl.top/gtputmdzfd.html

Java: list.contains(x)
来源：http://hz.chenlongwang.top/gtuthrvvqo.html

Go:   slices.Contains(arr, x)
来源：http://hz.cheryme.top/gtqdqfreej.html

Ruby: arr.include?(x)
来源：http://hz.guowangkeji.top/gtwpznenjn.html

C#:   list.Contains(x)
来源：http://hz.feifeiyinyue.top/gtphyipotr.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cucudq.cn/gtixiiyiyn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cheryme.top/gtkxefscwr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.quarkkingdee.top/gtwdmdidjt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jqgfzy.top/gtfipyvtqi.html

TS:   [...arr];
来源：http://hz.ppjwa.cn/gtvbxuhbqr.html

Java: new ArrayList<>(list);
来源：http://hz.yuanzhike.top/gtjdkovrkj.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.quarkkingdee.top/gtzlgagzpx.html

Ruby: arr.dup;  arr.clone
来源：http://hz.pycfn.com/gtizzzsqyb.html

C#:   new List<int>(list);
来源：http://hz.pengpengdd.cyou/gtdcffzvxn.html

[D23] reduce 累积计算
来源：http://hz.chenzaomai.com/gtugdpocvx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.fengsongda.top/gthmbvojqi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yongpay.top/gtiuimaaes.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hnxiangtu.top/gtjqpqckjd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cucudq.cn/gtegnkbehs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hysaishi.cn/gtdltkgndn.html

Go:   // 手写循环
来源：http://hz.andypj.xyz/gtdtvklhhp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.dianchejie.cn/gtetofhrcj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.gzhubu.top/gtxazovsno.html

[D24] 字典 / Map 基本操作
来源：http://hz.shzxlz.cn/gtrgrcvfwm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xuetiantiany.cn/gtolmxrcic.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sysykeji.top/gtonvmjqzl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yangfankeji.com/gtzaewbrxv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.daria6918.cn/gtehamkgki.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinyuanbaomall.cn/gtlgjnnmxl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hnqzz.top/gtmgovyoeq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.daxiang520.top/gtpvijalmp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jyoumei.cn/gtlempmnud.html

[D25] Set 集合去重与交并差
来源：http://hz.ehwqpu.com/gtjvynjuyl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cucudq.cn/gtpatlckdu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.nanxuanxn.top/gtodbsmblb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.tian-w.cn/gtowgjjwxd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ppjwa.cn/gtvdpoqlin.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.mhx1999.top/gtczdeblww.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.snrcjt.cn/gtgrsmfpls.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.pengpengdd.cyou/gtjrrylkot.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.nanxinkj.top/gtiocsyftv.html

[D26] 数组转字符串
来源：http://hz.tian-w.cn/gtjfejzatz.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhongyouzk.top/gttgbyyxdk.html

PHP:  implode(", ", $arr);
来源：http://hz.316326.xyz/gtktdpivfa.html

JS:   arr.join(", ")
来源：http://hz.zhiwuduotai.top/gtshwyoiez.html

TS:   arr.join(", ")
来源：http://hz.zdqjudy.top/gtqbulpbcx.html

Java: String.join(", ", list)
来源：http://hz.shangyingyoupin.top/gtsngujhhz.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jqgufenzy.top/gtqgpabomc.html

Ruby: arr.join(", ")
来源：http://hz.tian-w.cn/gtificnizx.html

C#:   string.Join(", ", list)
来源：http://hz.shanyushiyangtech.top/gtobdwoioo.html

================================================================================
来源：http://hz.yonumen.top/gtbzyaqsip.html

E. 字符串处理
来源：http://hz.yanxiufei.cn/gteeovggeh.html

================================================================================
来源：http://hz.zhixingplan.top/gtspqalymi.html

[E01] 拼接字符串
来源：http://hz.zhaomingkeji.xyz/gtlwngpiix.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.316326.xyz/gtwalcylee.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhixingplan.top/gtlgrmrmbr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.iojbl.cn/gthhuftgel.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj20258.top/gtgvfzipnb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ywan-chungtsiang.top/gtesmbsmvp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yongpay.top/gtspzcnsro.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.fzhhl.top/gtdejzzmsp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hammf.cn/gtpenhzewp.html

[E02] 重复字符串
来源：http://hz.nwbrower.top/gtkkvoqzwn.html

Py:   "ab" * 3
来源：http://hz.hongshengwenyu.top/gtfhjptmxm.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xuanzx.com/gtouugmmxu.html

JS:   "ab".repeat(3)
来源：http://hz.zhengqikj.top/gtfykafxxz.html

TS:   "ab".repeat(3)
来源：http://hz.nwbrower.top/gtutmfwdml.html

Java: "ab".repeat(3)
来源：http://hz.smart0.xyz/gtaaspurgn.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hnxiangtu.top/gtgqcgzwcm.html

Ruby: "ab" * 3
来源：http://hz.hnxiangtu.top/gtifmgyrdx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.guannengcc.top/gtrkevmsio.html

[E03] 截取子串
来源：http://hz.zycfv.cn/gtdccobbpd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.52xcode.cn/gtzniwajzn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gotoacloud.top/gtzopqcwsn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.fengsongda.top/gtaapzrryp.html

TS:   s.slice(1, 4)
来源：http://hz.cqqwz.cn/gtmdnifzzt.html

Java: s.substring(1, 4)
来源：http://hz.xingfuxueyuan.xyz/gtcxqyxuqe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yangfankeji.com/gtvylzenne.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shzxlz.cn/gtmixbvsdu.html

C#:   s.Substring(1, 3)
来源：http://hz.xuetiantiany.cn/gtvcozhknp.html

[E04] 查找子串位置
来源：http://hz.dashuyun.cn/gtpbqarbuc.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yuanzhike.top/gtvtaqdnlm.html

PHP:  strpos($s, "x");
来源：http://hz.yuanzhike.top/gtkibjownu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shangyingyoupin.top/gtdvbkoyoy.html

TS:   s.indexOf("x")
来源：http://hz.fzhhl.top/gtfiqvuvjh.html

Java: s.indexOf("x")
来源：http://hz.iojbl.cn/gtpcqnlpya.html

Go:   strings.Index(s, "x")
来源：http://hz.xingfuxueyuan.xyz/gtlkliuhuo.html

Ruby: s.index("x")
来源：http://hz.gotoacloud.top/gtkafdndez.html

C#:   s.IndexOf("x")
来源：http://hz.tanke756.top/gtkchnopkp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ivvv.top/gtbsbextkf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hysaishi.cn/gtivxjetig.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.svipenyu.cn/gtgrysmyqj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.pycfn.com/gtqfinlfde.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.guowangkeji.top/gtxptciadj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jqgfzy.top/gtmgxrnhrk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.sysykeji.top/gtbddosrje.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ydzc1.top/gtejjquync.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.mhx1999.top/gtnjwgnese.html

[E06] 替换子串
来源：http://hz.jyoumei.cn/gtwqcjcshg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.andypj.xyz/gtcwdgaftp.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.guowangkeji.top/gtysnwdkyz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sweek.top/gtnellqudw.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gtmlxtnsyv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sysykeji.top/gttyjdrdlz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yuanzhike.top/gtiguystrz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xylfe.cn/gtstuzatmx.html

C#:   s.Replace("a", "b")
来源：http://hz.nanxuanxn.top/gtaalzlkza.html

[E07] 按分隔符拆分
来源：http://hz.ybcxt.top/gtzygebdtn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.aizwys.cn/gtmnhqjoqu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shzxlz.cn/gtdcivjjtz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.aibaodan.cn/gtlhciqxjv.html

TS:   s.split(",")
来源：http://hz.havefunace.top/gtoguiaorh.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shanyushiyangkeji.top/gtssywtrbf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.kuanghao11.cn/gtfdikcqkl.html

Ruby: s.split(",");  s.split
来源：http://hz.zycfv.cn/gtfuzjhyvn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jlsjyb.cn/gtlknemlkj.html

[E08] 数组按分隔符合并
来源：http://hz.wangdashe.top/gtxbxcsrzj.html

Py:   ",".join(items)
来源：http://hz.yj20258888.top/gthitnottv.html

PHP:  implode(",", $items);
来源：http://hz.shangyingyoupin.top/gtkjplhtyr.html

JS:   items.join(",")
来源：http://hz.daxiang520.top/gteuptxmjj.html

TS:   items.join(",")
来源：http://hz.sufxvd.cn/gtqnoaomiy.html

Java: String.join(",", items)
来源：http://hz.iojbl.cn/gtahicaduj.html

Go:   strings.Join(items, ",")
来源：http://hz.dianchejie.cn/gtfjysoiau.html

Ruby: items.join(",")
来源：http://hz.316326.xyz/gtibvtscig.html

C#:   string.Join(",", items)
来源：http://hz.zhengqikj.top/gtecyzmgrf.html

[E09] 去除所有空白字符
来源：http://hz.316326.xyz/gtuofmznpz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.sweek.top/gtgpxewzcb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hywenlv.cn/gthhedcqgg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenzaomai.com/gtfucjcnjj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cdnleiting.top/gtlymmczio.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.cqqwz.cn/gtfqukdqrj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jlsjyb.cn/gtrvnytggc.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hfpthk.cn/gtznqwslsa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.shuidangran.top/gtuyzbiqxh.html

[E10] 左侧补零 / 定长填充
来源：http://hz.wangdashe.top/gtozupqwzm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.sweek.top/gtkhnmhdal.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.snrcjt.cn/gtklzslbkk.html

JS:   "7".padStart(3, "0")
来源：http://hz.gotoacloud.top/gtpyqcnahv.html

TS:   "7".padStart(3, "0")
来源：http://hz.yongpay.top/gttpzcsexk.html

Java: String.format("%03d", 7)
来源：http://hz.ybcxt.top/gtyxlftkpx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sufxvd.cn/gtgjehudnl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sweek.top/gtkkpktyxd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenlongwang.top/gtvvxpdyux.html

[E11] 反转字符串
来源：http://hz.sufxvd.cn/gtsyxpyiei.html

Py:   s[::-1]
来源：http://hz.smart0.xyz/gtvtabucra.html

PHP:  strrev($s);
来源：http://hz.jianghu66.top/gtwypgkmhz.html

JS:   [...s].reverse().join("")
来源：http://hz.ehwqpu.com/gtmkrdihge.html

TS:   [...s].reverse().join("")
来源：http://hz.mhx1999.top/gtzpaqjqzv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yuxming.cn/gtrndczuey.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jqgufenzy.top/gtumiblnta.html

Ruby: s.reverse
来源：http://hz.hywenlv.cn/gtwebxxjay.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jyoumei.cn/gtvjnleity.html

[E12] 统计某字符出现次数
来源：http://hz.quarkkingdee.top/gtlervtorn.html

Py:   s.count("a")
来源：http://hz.quarkkingdee.top/gtgliilssm.html

PHP:  substr_count($s, "a");
来源：http://hz.cdnleiting.top/gtjgcpszpd.html

JS:   s.split("a").length - 1
来源：http://hz.chenjidiqi.icu/gtuuagijin.html

TS:   s.split("a").length - 1
来源：http://hz.shuidangran.top/gtklvkszdu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yj202588.top/gtverzuwmg.html

Go:   strings.Count(s, "a")
来源：http://hz.hysaishi.cn/gtrqtvwvis.html

Ruby: s.count("a")
来源：http://hz.bjfxy.top/gthwjufnbm.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yuxming.cn/gtcnztofok.html

[E13] 逐字符遍历
来源：http://hz.vqdsnc.cn/gtbrouibam.html

Py:   for ch in s: print(ch)
来源：http://hz.gogol.net.cn/gtmdzyvcow.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhiwuduotai.top/gtuqojhgqa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nwbrower.top/gttqxbpzbm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.316326.xyz/gtfxpkmmgv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yonumen.top/gtcxhyfgyi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.gogol.net.cn/gtgmcwakkt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.tian-w.cn/gtiuienbwu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yongpay.top/gtzxsichym.html

[E14] URL 编码与 Base64
来源：http://hz.yuanzhike.top/gtmtrknhrb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.0kj1m.cn/gtxxhrcwdu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yangfankeji.com/gtqghwkldz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xingfuxueyuan.xyz/gtegjppbto.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cucudq.cn/gtdxsbgvvo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.bjfxy.top/gtlaueinwu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jyoumei.cn/gtvzikbnbs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhoulong.xyz/gtszerangh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jinqigufen.top/gtsfrbdrde.html

[E15] HTML 转义 / 反转义
来源：http://hz.jqgufenzy.top/gtruftzaqb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinqigfzy.top/gthgidpzzt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.haohaochexian.top/gtdhubtlhh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhixingplan.top/gtccqanxyg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.sweek.top/gtlzifnxdx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.sysykeji.top/gtpqeaevxj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.pycfn.com/gtlfcovmtw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hnqzz.top/gtfuxrzuby.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.tian-w.cn/gtxyiicvca.html

[E16] 数字千分位
来源：http://hz.jianghu66.top/gtmbxebntc.html

Py:   f"{1234567:,}"
来源：http://hz.sysykeji.top/gtxahkomyh.html

PHP:  number_format(1234567);
来源：http://hz.xingfuxueyuan.xyz/gtjrusncfp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xingfuxueyuan.xyz/gtqrdmydbb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hammf.cn/gtjlvdosrg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.birdmap.top/gtwyykqmjx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.pycfn.com/gtyptemnon.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yvedp.cn/gtzfinbcwb.html

C#:   1234567.ToString("N0")
来源：http://hz.gogol.net.cn/gtiuzwmggk.html

[E17] 首字母大写
来源：http://hz.sxryk.cn/gtuqhfetih.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.kuanghao11.cn/gtzeqmtlgc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.pengpengdd.cyou/gtzzbzitip.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yvedp.cn/gtgpxauwzy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.daria6918.cn/gtorwttqrl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.gzhubu.top/gtuqbsnxmk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.chenjidiqi.icu/gtsdwlpeod.html

Ruby: s.capitalize
来源：http://hz.zhongyouzk.top/gtqkfkwmuz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.chenlongwang.top/gtheipefax.html

[E18] 模板占位符替换
来源：http://hz.yongpay.top/gtskalxurw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shanyushiyangkeji.top/gtlsfmduat.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinqigufen.top/gtwwoyeatz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenlongwang.top/gtelqxjppl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hammf.cn/gtwczivjpi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.chenlongwang.top/gthtbpnqct.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yangfankeji.com/gtqgxprkqi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.gzhubu.top/gtaaltkzoc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yanxiufei.cn/gtnvxkicvj.html

[E19] 多行文本按行拆分
来源：http://hz.andypj.xyz/gtdwculdds.html

Py:   s.splitlines()
来源：http://hz.zhengqikj.top/gtkxkmflvf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shzxlz.cn/gtlnlbtlvu.html

JS:   s.split(/\r?\n/)
来源：http://hz.hfpthk.cn/gtzgzowjur.html

TS:   s.split(/\r?\n/)
来源：http://hz.xylfe.cn/gtvwqtngmy.html

Java: s.lines().toList()
来源：http://hz.zhixingplan.top/gthokzwobp.html

Go:   strings.Split(s, "\n")
来源：http://hz.gaohongyu789.top/gtwlkltgnk.html

Ruby: s.lines
来源：http://hz.zhengqikj.top/gtzzqxliwz.html

C#:   s.Split('\n')
来源：http://hz.andypj.xyz/gtuzvbnmvr.html

[E20] 判断字符串是否为空
来源：http://hz.yvedp.cn/gtvftivujl.html

Py:   if not s:
来源：http://hz.tanke756.top/gtfkefakmx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gogol.net.cn/gtjvhdiqnn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.wangshuangyany.cn/gtbwdiwemt.html

TS:   if (s === "") {}
来源：http://hz.guannengcc.top/gtmygpalei.html

Java: if (s.isEmpty()) {}
来源：http://hz.zycfv.cn/gtwbaiznpo.html

Go:   if s == "" {}
来源：http://hz.ywan-chungtsiang.top/gtzusbejin.html

Ruby: if s.empty?
来源：http://hz.shzxlz.cn/gtbyjnlwtt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.pengpengdd.cyou/gtmpperijy.html

[E21] 超长截断加省略号
来源：http://hz.guannengcc.top/gtzocefsds.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jqgufenzy.top/gtzdtaqsrf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.chenjidiqi.icu/gtueulvtki.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.0kj1m.cn/gtfukpulnz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gtahtuwnmk.html


<!-- 参考信息 -->