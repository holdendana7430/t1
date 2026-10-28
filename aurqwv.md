代发 wailian999

TS:   [...new Set(arr)]
来源：http://hz.yangfankeji.com/gtahfkuhiy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xuanzx.com/gtdglestco.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.svipenyu.cn/gtgtwbcyfv.html

Ruby: arr.uniq
来源：http://hz.shzxlz.cn/gtieqivrbr.html

C#:   list.Distinct().ToList()
来源：http://hz.ybcxt.top/gtmjrdyzlu.html

[D16] 求和与平均值
来源：http://hz.ydjk.org.cn/gtcypyyekq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.smart0.xyz/gtetghwgtt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hammf.cn/gtvdfpfaxb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.0kj1m.cn/gtvttaaiei.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.redwolf501.top/gtpwsrxcan.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gotoacloud.top/gtfdfgqtat.html

Go:   // 手写循环累加
来源：http://hz.zhijiandao.cn/gtazhkehed.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xylfe.cn/gtgghicsqd.html

C#:   list.Sum();  list.Average()
来源：http://hz.feifeiyinyue.top/gtpbirqtwq.html

[D17] 最大值与最小值
来源：http://hz.gzhubu.top/gtgydrezcl.html

Py:   max(arr);  min(arr)
来源：http://hz.jiagoushi.top/gtswzsnasd.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhaomingkeji.xyz/gtnhxlqlgb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jinqigufen.top/gtipfuxgub.html

TS:   Math.max(...arr);
来源：http://hz.yueranfly.top/gtjvhyyinj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xylfe.cn/gtpzdulhsq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xingfuxueyuan.xyz/gtyvgoyoxo.html

Ruby: arr.max;  arr.min
来源：http://hz.zycfv.cn/gtnxrpdwhd.html

C#:   list.Max();  list.Min()
来源：http://hz.shanyushiyangtech.top/gtiyjoaehp.html

[D18] 扁平化嵌套数组
来源：http://hz.jianghu66.top/gtxuxbsxvn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhoulong.xyz/gtiephfggf.html

PHP:  array_merge(...$nested);
来源：http://hz.jlsjyb.cn/gtxkhjcxnk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jyoumei.cn/gtghotzufz.html

TS:   nested.flat();
来源：http://hz.nwbrower.top/gtrmvhqjzv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.guowangkeji.top/gtibjejdqi.html

Go:   // 手写双层循环
来源：http://hz.jlsjyb.cn/gtbcqscbyp.html

Ruby: nested.flatten
来源：http://hz.jinqigfzy.top/gtmgxuhpng.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.cqqwz.cn/gtrncdbffk.html

[D19] 按字段分组
来源：http://hz.xziqi.cn/gtbjserzdl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.havefunace.top/gtivifywzg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.pengpengdd.cyou/gtrndglbgm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hfpthk.cn/gtcswawxkq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhijiandao.cn/gtwcqemptu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.c1oappe.top/gtyugritqz.html

Go:   // 手写 map[string][]T
来源：http://hz.hywenlv.cn/gtcbxsdjbg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.mhx1999.top/gtfvsecnyr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ydzc1.top/gtkupeubju.html

[D20] 统计每个元素出现次数
来源：http://hz.jinghuilouyu.cn/gtxhygtuoz.html

Py:   Counter(arr)
来源：http://hz.yvedp.cn/gtgaspnfcl.html

PHP:  array_count_values($arr);
来源：http://hz.hywenlv.cn/gtuvfcxckr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxinkj.top/gtdsthsvgz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fzhhl.top/gtixcrayoq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yvedp.cn/gtrckqofux.html

Go:   // 手写 map[T]int
来源：http://hz.svipenyu.cn/gtlgoktllt.html

Ruby: arr.tally
来源：http://hz.ydzc1.top/gtmjocmewr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jlsjyb.cn/gtftcfdecd.html

[D21] 判断是否包含某元素
来源：http://hz.yangfankeji.com/gttwywtyvs.html

Py:   x in arr
来源：http://hz.xuanzx.com/gtvfihmana.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cashguo.top/gttojutuvt.html

JS:   arr.includes(x)
来源：http://hz.aibaodan.cn/gtywfogogk.html

TS:   arr.includes(x)
来源：http://hz.andypj.xyz/gtldadzejf.html

Java: list.contains(x)
来源：http://hz.nanxuanxn.top/gtofpjwrur.html

Go:   slices.Contains(arr, x)
来源：http://hz.sufxvd.cn/gtscmrbvvc.html

Ruby: arr.include?(x)
来源：http://hz.sysykeji.top/gtclmivwuq.html

C#:   list.Contains(x)
来源：http://hz.yvedp.cn/gtgqezoxws.html

[D22] 复制数组（避免共享引用）
来源：http://hz.snrcjt.cn/gtunrkdtye.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xuanzx.com/gtlluuetmw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shanyushiyangtech.top/gtnvfvftan.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shanyushiyangkeji.top/gtstdmhdsy.html

TS:   [...arr];
来源：http://hz.fengsongda.top/gthcyzgrdm.html

Java: new ArrayList<>(list);
来源：http://hz.jianghu66.top/gtxbxyhlfv.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.cucudq.cn/gteuophrok.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xziqi.cn/gtiiocegfj.html

C#:   new List<int>(list);
来源：http://hz.316326.xyz/gtvvlqnhou.html

[D23] reduce 累积计算
来源：http://hz.tianlin.xyz/gtszlygydc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jiagoushi.top/gtgsglaxwa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.pycfn.com/gtampmksfb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hnxiangtu.top/gtvhxflzmk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sufxvd.cn/gttphpytgw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.cqqwz.cn/gtdtphhypk.html

Go:   // 手写循环
来源：http://hz.shanyushiyangkeji.top/gtayulxkdg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yvedp.cn/gtofjkogoi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.snrcjt.cn/gtivymtjil.html

[D24] 字典 / Map 基本操作
来源：http://hz.sufxvd.cn/gtwwspzefx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ivvv.top/gtphiouvfw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yueranfly.top/gtfdtasijg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ppjwa.cn/gtuquwblhy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yueranfly.top/gtzbfyakri.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cqqwz.cn/gtrrhumimv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.sysykeji.top/gtcaohgmev.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.guowangkeji.top/gttsjyoipg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shangyingyoupin.top/gtlhatpfwa.html

[D25] Set 集合去重与交并差
来源：http://hz.hnqzz.top/gtukbcwttu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.sxryk.cn/gtplctamwq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.tanke756.top/gtajdimfey.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hfpthk.cn/gtxelerjdu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yangfankeji.com/gthjsiblib.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.haohaochexian.top/gtiddbxjay.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.daxiang520.top/gtzcdjwrlm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jqgufenzy.top/gtaphobupg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.guowangkeji.top/gtzhjxmmcm.html

[D26] 数组转字符串
来源：http://hz.shangyingyoupin.top/gtcsvacghn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.nanxinkj.top/gtplakktks.html

PHP:  implode(", ", $arr);
来源：http://hz.snrcjt.cn/gtafzapjuy.html

JS:   arr.join(", ")
来源：http://hz.zhixingplan.top/gtqqtbnnbn.html

TS:   arr.join(", ")
来源：http://hz.haohaochexian.top/gtovhxvvru.html

Java: String.join(", ", list)
来源：http://hz.mhx1999.top/gtfeziremp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhoulong.xyz/gtwliukhzi.html

Ruby: arr.join(", ")
来源：http://hz.nwbrower.top/gtieumyibm.html

C#:   string.Join(", ", list)
来源：http://hz.aibaodan.cn/gtgcvwzydb.html

================================================================================
来源：http://hz.cqqwz.cn/gtksphvobx.html

E. 字符串处理
来源：http://hz.ybcxt.top/gtpsavtrlz.html

================================================================================
来源：http://hz.quarkkingdee.top/gtplooehng.html

[E01] 拼接字符串
来源：http://hz.yuanzhike.top/gtftaghuct.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.gogol.net.cn/gthwvmdjwg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hywenlv.cn/gtueeltamx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shanyushiyangtech.top/gtqvayzxvs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuanzhike.top/gtdimvoocr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.gaohongyu789.top/gttwmeylew.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xingfuxueyuan.xyz/gtnopmlrnv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.mhx1999.top/gtunuyylwh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yuxming.cn/gtmdzfugis.html

[E02] 重复字符串
来源：http://hz.iojbl.cn/gtelkgzjag.html

Py:   "ab" * 3
来源：http://hz.hywenlv.cn/gtyqfkjapf.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hnxiangtu.top/gtlnvlgkoc.html

JS:   "ab".repeat(3)
来源：http://hz.shzxlz.cn/gtjgdzlavg.html

TS:   "ab".repeat(3)
来源：http://hz.haohaochexian.top/gtgzixrzux.html

Java: "ab".repeat(3)
来源：http://hz.chenjidiqi.icu/gtvawiaksz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.9152youxi.cn/gtpfyepjco.html

Ruby: "ab" * 3
来源：http://hz.shanyushiyangkeji.top/gtqyerohug.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xziqi.cn/gtfrflpjcv.html

[E03] 截取子串
来源：http://hz.yvedp.cn/gtyuocknsw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hongshengwenyu.top/gtdtvpkpyi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.chenlongwang.top/gtsvcthvgy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shanyushiyangtech.top/gteehkurhu.html

TS:   s.slice(1, 4)
来源：http://hz.sweek.top/gtwhzfugpl.html

Java: s.substring(1, 4)
来源：http://hz.xuanzx.com/gttloiwbbq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yangfankeji.com/gtodgujkqh.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.kuanghao11.cn/gtlhdwmxqt.html

C#:   s.Substring(1, 3)
来源：http://hz.tian-w.cn/gtevyevzmq.html

[E04] 查找子串位置
来源：http://hz.cucudq.cn/gtjziuihkt.html

Py:   s.find("x");  s.index("x")
来源：http://hz.birdmap.top/gtkbbshnzp.html

PHP:  strpos($s, "x");
来源：http://hz.zhaomingkeji.xyz/gthluocwyt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.mhx1999.top/gtafiolosr.html

TS:   s.indexOf("x")
来源：http://hz.nanxuanxn.top/gtltpyovmz.html

Java: s.indexOf("x")
来源：http://hz.shanyushiyangkeji.top/gtjsbwgxju.html

Go:   strings.Index(s, "x")
来源：http://hz.nanxinkj.top/gtlcgbzzlp.html

Ruby: s.index("x")
来源：http://hz.yj20258888.top/gtcksiedam.html

C#:   s.IndexOf("x")
来源：http://hz.xuanzx.com/gtyjajwfzn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ivvv.top/gtngyuyntr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hammf.cn/gtkemhzosp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.meibo888.top/gtwthgxvat.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj202588.top/gtogbimaqk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cdnleiting.top/gtxkbqzdud.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gzhubu.top/gtcjrjbfbq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.quarkkingdee.top/gtczmnhajm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shuidangran.top/gtlfioatfz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.316326.xyz/gtokgelwhr.html

[E06] 替换子串
来源：http://hz.wangdashe.top/gtoqasfidk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.gotoacloud.top/gtugfbfrty.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.gaohongyu789.top/gtnnwguncc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yvedp.cn/gtsrhncszj.html

TS:   s.replaceAll("a", "b")
来源：http://hz.xylfe.cn/gtprjjueov.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.pycfn.com/gtwluaxfle.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.feifeiyinyue.top/gtjoxkillp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yuanzhike.top/gtcljfzmay.html

C#:   s.Replace("a", "b")
来源：http://hz.jyoumei.cn/gtksaciene.html

[E07] 按分隔符拆分
来源：http://hz.nanxinkj.top/gtgwjfgfjc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.birdmap.top/gtlawxgboy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jqgfzy.top/gtqsywjzhv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.tianlin.xyz/gtxzubxzje.html

TS:   s.split(",")
来源：http://hz.cucudq.cn/gthsztrmyl.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xuetiantiany.cn/gtjkbtanpy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.svipenyu.cn/gtwoowlzil.html

Ruby: s.split(",");  s.split
来源：http://hz.yj202588.top/gtcocgijps.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.nanxuanxn.top/gtpfmsckol.html

[E08] 数组按分隔符合并
来源：http://hz.hongshengwenyu.top/gtjizbhdcm.html

Py:   ",".join(items)
来源：http://hz.9152youxi.cn/gtmtokvlya.html

PHP:  implode(",", $items);
来源：http://hz.yongpay.top/gtpiwtjezq.html

JS:   items.join(",")
来源：http://hz.aizwys.cn/gtxhxdbvje.html

TS:   items.join(",")
来源：http://hz.ydjk.org.cn/gtvpothkvu.html

Java: String.join(",", items)
来源：http://hz.xuanzx.com/gtxfotvyvd.html

Go:   strings.Join(items, ",")
来源：http://hz.yuxming.cn/gtlheptpgk.html

Ruby: items.join(",")
来源：http://hz.sxryk.cn/gtwaokstak.html

C#:   string.Join(",", items)
来源：http://hz.iojbl.cn/gtqjacjwjs.html

[E09] 去除所有空白字符
来源：http://hz.daxiang520.top/gtjgecgxex.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xinyue.icu/gtadhsksyy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hywenlv.cn/gtgxvowljr.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenlongwang.top/gtazbwobie.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.gzhubu.top/gtzcctndpr.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jiagoushi.top/gtghsvgohn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sxryk.cn/gthsoknwrm.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.9152youxi.cn/gtlmjaezpl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.shanyushiyangkeji.top/gtbgamnnvh.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhixingplan.top/gtxjsukjhx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hnqzz.top/gtmptsvswn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.shangyingyoupin.top/gtftzxbqvh.html

JS:   "7".padStart(3, "0")
来源：http://hz.xuetiantiany.cn/gtvodpnxde.html

TS:   "7".padStart(3, "0")
来源：http://hz.ppjwa.cn/gtefnrhaud.html

Java: String.format("%03d", 7)
来源：http://hz.ehwqpu.com/gtroffjpdo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.mhx1999.top/gttigffzed.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.pengpengdd.cyou/gtyirlgzlc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.redwolf501.top/gtrcqwdnvu.html

[E11] 反转字符串
来源：http://hz.daria6918.cn/gtwawepops.html

Py:   s[::-1]
来源：http://hz.gotoacloud.top/gtsergtxsp.html

PHP:  strrev($s);
来源：http://hz.hywenlv.cn/gtlpcoeecj.html

JS:   [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtkmbmjjyn.html

TS:   [...s].reverse().join("")
来源：http://hz.yonumen.top/gthblbhdfi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinyuanbaomall.cn/gtgyhrpgmr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.cdnleiting.top/gtakqtkusf.html

Ruby: s.reverse
来源：http://hz.zycfv.cn/gtllleakvi.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.chenjidiqi.icu/gtdyedcnae.html

[E12] 统计某字符出现次数
来源：http://hz.jianghu66.top/gtoasodivz.html

Py:   s.count("a")
来源：http://hz.andypj.xyz/gteztfynga.html

PHP:  substr_count($s, "a");
来源：http://hz.shzxlz.cn/gtaxrctfew.html

JS:   s.split("a").length - 1
来源：http://hz.ywan-chungtsiang.top/gtakqawswb.html

TS:   s.split("a").length - 1
来源：http://hz.redwolf501.top/gtymwpkwrd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zycfv.cn/gttyjrkamw.html

Go:   strings.Count(s, "a")
来源：http://hz.sufxvd.cn/gtxuiwuhno.html

Ruby: s.count("a")
来源：http://hz.ehwqpu.com/gtfpiwxhxs.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shuidangran.top/gttubjhdwb.html

[E13] 逐字符遍历
来源：http://hz.ppjwa.cn/gtpbaosndh.html

Py:   for ch in s: print(ch)
来源：http://hz.aibaodan.cn/gtylmukqyt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yueranfly.top/gtrfpbxrju.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jlsjyb.cn/gtbstjlrsu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zdqjudy.top/gtvkrxfffm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.aizwys.cn/gtymdoznjm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xingfuxueyuan.xyz/gtldawdvjn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xuetiantiany.cn/gtqwjrlhhr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jqgufenzy.top/gtimncwycb.html

[E14] URL 编码与 Base64
来源：http://hz.meibo888.top/gtqjiqcctb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.iojbl.cn/gtotxakwec.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jianghu66.top/gtnflceyis.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.pycfn.com/gttxlehekq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.nwbrower.top/gtsltocvas.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.dianchejie.cn/gtpyubczbp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yanxiufei.cn/gtrnuviqby.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yongpay.top/gtsnfhgons.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ivvv.top/gtmghxeqzw.html

[E15] HTML 转义 / 反转义
来源：http://hz.ydzc1.top/gtpldbykpa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yj202588.top/gtprddbgos.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ywan-chungtsiang.top/gtcyikxyqq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ydzc1.top/gtntoguajo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhaomingkeji.xyz/gtmxwbdcrh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.guowangkeji.top/gtddapajan.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhiwuduotai.top/gtugbirfwn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sweek.top/gtkmknsovf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xinyue.icu/gtxgqxrzcu.html

[E16] 数字千分位
来源：http://hz.shanyushiyangkeji.top/gterhkctfi.html

Py:   f"{1234567:,}"
来源：http://hz.ivvv.top/gtypjzsgdk.html

PHP:  number_format(1234567);
来源：http://hz.feifeiyinyue.top/gtbouljaas.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinyuanbaomall.cn/gtfibyrvuw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.tanke756.top/gtohapimul.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.dianchejie.cn/gtgzwxjpvi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.shzxlz.cn/gteltfacvn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.nwbrower.top/gtnsoglvch.html

C#:   1234567.ToString("N0")
来源：http://hz.tian-w.cn/gtifcujcpp.html

[E17] 首字母大写
来源：http://hz.shzxlz.cn/gtlsrvxhms.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.fengsongda.top/gtpynfsryn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gzhubu.top/gttcnmnhnu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xingfuxueyuan.xyz/gtfbyiwaou.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.andypj.xyz/gtodtjjuxp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jiagoushi.top/gtyiyjvdip.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zdqjudy.top/gttdyzljay.html

Ruby: s.capitalize
来源：http://hz.9152youxi.cn/gtvlrrjxmm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zdqjudy.top/gtynikolrb.html

[E18] 模板占位符替换
来源：http://hz.shanyushiyangkeji.top/gtbguhrpoy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ydjk.org.cn/gttsuutaus.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.pycfn.com/gtgxpptdun.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenzaomai.com/gtbclaqdzn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuanzx.com/gtkyzgdeat.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhijiandao.cn/gtkmpfchal.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.sysykeji.top/gtiweffitq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.redwolf501.top/gtgnddnrlo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.daxiang520.top/gtlelwrwkz.html

[E19] 多行文本按行拆分
来源：http://hz.meibo888.top/gtrpeavtsa.html

Py:   s.splitlines()
来源：http://hz.birdmap.top/gthrlsgveg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.smart0.xyz/gtemcefiyt.html

JS:   s.split(/\r?\n/)
来源：http://hz.andypj.xyz/gtvjescqwk.html

TS:   s.split(/\r?\n/)
来源：http://hz.jyoumei.cn/gteytavzrd.html

Java: s.lines().toList()
来源：http://hz.yangfankeji.com/gtuaqwfrxc.html

Go:   strings.Split(s, "\n")
来源：http://hz.ydjk.org.cn/gtyekfhbre.html

Ruby: s.lines
来源：http://hz.xylfe.cn/gtzmpndylo.html

C#:   s.Split('\n')
来源：http://hz.shuidangran.top/gtyzwvxxgb.html

[E20] 判断字符串是否为空
来源：http://hz.jqgfzy.top/gtkfhwlhkb.html

Py:   if not s:
来源：http://hz.guannengcc.top/gtgueompjr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hywenlv.cn/gtmpyjniev.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.0kj1m.cn/gtdtxijwph.html

TS:   if (s === "") {}
来源：http://hz.hywenlv.cn/gtzjpaqnct.html

Java: if (s.isEmpty()) {}
来源：http://hz.smart0.xyz/gtmfvihdun.html

Go:   if s == "" {}
来源：http://hz.hnxiangtu.top/gttbqqdhzz.html

Ruby: if s.empty?
来源：http://hz.zhiwuduotai.top/gtqnjrbbdx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ydjk.org.cn/gttmyunncf.html

[E21] 超长截断加省略号
来源：http://hz.316326.xyz/gtccoalxfd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shzxlz.cn/gtgdxjrrkz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.smart0.xyz/gtcbnehtgk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sufxvd.cn/gtvvkeffld.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtxlwrjdau.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtzvqacurl.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yongpay.top/gtiurkrcen.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.fengsongda.top/gtdsibuprv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jianghu66.top/gtytacdfgo.html

[E22] 字节长度与字符长度
来源：http://hz.smart0.xyz/gtkzecaujt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.chenzaomai.com/gthswcnkzp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yvedp.cn/gtsdqwiwvg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangtech.top/gtxyjxgfuh.html


<!-- 参考信息 -->