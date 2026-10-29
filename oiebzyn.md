代发 wailian999

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gvpenypnh.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gpeybfnjr.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/ggtddykzd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/girtnlprv.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gdepslwmz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gblsurram.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gttdiabce.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gqzuxowrc.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gpwmkehik.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gxqozxkvi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/ghwoihwxu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/geisucauj.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/ghmgdhqaj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqkettoyq.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gjewlrvrm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gpexnsvwr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gxdnvgwsd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gxttwrmqw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gleyuuayp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gkoakyfem.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/grsaveprr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gsrhrvuri.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/grhvmegbx.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gwpztqbek.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gpfcexejk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gbugixzyu.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/ghdruhzeb.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gltfnjzkz.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gjiyrxrcc.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gcvslwzus.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gmtzdlrdx.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gnzfdvdfo.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gwfdgeauj.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/grjsqzlci.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/ghsnyzpoh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/ggiehfltb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/givvepdqi.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/ghyxixnan.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gdaimelha.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gvtgzzrqj.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gffzabfwi.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gcgggxjol.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gztnqhgrc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gxnlnnygl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gykdfouxi.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gmzuxtnmf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gepmluyzj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gsxlpjutu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/ggrqurgrn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gxwslyloe.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gadjutfug.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gvimlseau.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gsihagwdu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gdmmgcrdn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gsdrpklwz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gvxmxkpbw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gvsfdmsxm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gcqegguzv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gibwdajle.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gsdkafdbc.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gjtwjjgaj.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gsjmmvkld.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gwiuplrki.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gqmvttydb.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gowydwnap.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gvndickoo.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gbwycbizg.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gjusziqcw.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gizyisrty.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gimrozmqs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/glqhdfpnc.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gtawgqybb.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gpnkbtvyo.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gafqajwgz.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gtbybgkew.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gskevunjr.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gktvyvlsl.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gnmokhump.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/ghpsjngej.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/ghrehtjbo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/golyhgnms.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gwsflqdna.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/girdpxplo.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gybctndya.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gnnqwctwj.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gxverqiqt.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gdfueytlp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/ggqtxkhku.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/ghvtlexgu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/ggzktijlx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gfkajocxw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gyrzgdnww.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gwilmfvhr.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gvpzrqebz.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gwmrcqvek.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gbgwiaqvu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gxmezmuom.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/glrwjkddo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/ggtvupjne.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/giopnhhfn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gdpcewnnu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gvyckhxgq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gqsqhkxvh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gscvufrpn.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/guijuygol.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gfrlejoez.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/ghrazsjio.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gwtiljcke.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gamtnvedb.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gtvikapji.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gscrmvsmu.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gfpkguvzz.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/goaeeqfhd.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gfjuandbf.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gpbqvbytn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gqcdiaclo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gusdhaenz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gcfbahwiy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gskgzfymc.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gpdsbbvwy.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gapslqixw.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/ghobkfrte.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gqawlkevn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/ggsytczfe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/grcebiodk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gyszzmuzu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gstyewrhp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gjbcqawpw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gzaxikipu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gjclrodit.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gdrsefotg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/giyqppejv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/ggdfucunh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gyxfowazh.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gucfhxbfg.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gqunyjciu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gfqvwifry.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gwckpensc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gdwjgbxnc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gbfdnsndh.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gwjbkulid.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/glbpowllt.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdjgstgba.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gxojsjkgh.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gxftcdexa.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gbamelaqv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gksvtowio.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gvvbdpaeq.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gdssforzb.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gkdcwmktz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gnbktabnf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gggehpkvm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gxunjoyxu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gfdxbscnv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gewisvinv.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gkuezuyfr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/ggxdclmgm.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gzzcqipdx.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/guesqekqf.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gmtsuazbi.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gyobnbrvq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gipoyumac.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/ghijazavf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/glmgvgrro.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gievmnltf.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/guasdifpy.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gziilmbli.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gelikbcia.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/grbldwqjz.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gyaoewmaw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gzuejlvkj.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gjytdyzel.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gbyqtxhsi.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gofsefjxf.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/ghlpquzrw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gzoalczsj.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gxwyqjamc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gupkjpwpp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gvhcmpqrt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gewubzywv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gvtoxhbks.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gqoorrlqw.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gndbrggdp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gecloldvd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gfcpwvebz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gkgwbvsry.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/giboukecq.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gsuodyvor.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gcheffhgh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gbljbzzot.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gvepebkul.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gvgrsvhdi.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gwywngjuu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gkonqvboq.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gefjndbce.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gbbrxhiaq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gqivqptjb.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/ggnfwvpxl.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gvlokepxg.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gtfyrjbtf.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/grhwtdajk.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gvvtreiyq.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gtndoqfkg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gkaieprws.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/guujocrur.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gflpsrtww.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gwmhcplko.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gafcccjxm.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gjjitqbjp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gqlobccrt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/ggnwqhmyo.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gjkvnntvl.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gbibmhety.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gufeorloj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gqltfhtrf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gyclnhwps.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gckpqkpqn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gzfnvuwve.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gxkpqrquc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gpqponimj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gtsomjuml.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gqosrkjbd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/ggomhllaz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/ggqiexslb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gevtpffav.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gwqivjsfi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gatlxmlkz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/glsyesnwo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gxcggenzk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gdeftuwnv.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gallzuaec.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/glswfskti.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/ghcjceect.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gzelaajzi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gkhcdstyy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/glcfciyjw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/geqssihxm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gsjuidhin.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gbaiztfyo.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gvwpktmqk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/ggtsarcjg.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gzkoootqk.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/grqbnxgwj.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gfpqniulw.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/ghddhtizz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/grrhsfiwg.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gasgesgdi.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gvnauubbs.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/graziaddd.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gwovmjjgf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcmnskoaj.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gaiazkzss.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gysrgucxb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gazwgmeie.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gxrnepuer.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gjancnfmk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gvqzhskpb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gqafufuok.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gexujfxci.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gpvauelzr.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/grzejpnpr.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gebulhlbd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gzxfmfrtr.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gtitcbcyk.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gfutiimgd.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/glgpsvvbg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gacmfvhbn.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gtejtkbyb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/ghdojgqds.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gnkiqnawt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gzmoosuky.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gxhspkxgr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gdwyxnzzk.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gnlqhjlkl.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gycpdzrcf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gednsoiou.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gqaavocsc.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/grbpwymmc.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gskpfokiu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/grxoslwib.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gvmyywxoq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gnbfyvbja.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/grqsknkbw.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gcoltxbjp.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/ggrqagbeg.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gxpuqsavg.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/ghoexgobf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gfhhskxrh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gzclzzvhv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gflexktwk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/grhdqrdvf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gdugrnsbm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/griypmxfg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gglggzzrt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gcbncvzrj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gdhopzouj.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gbwhndjme.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gddhvmdip.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/ghvodpjnc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gvlefhgnd.sHtML


<!-- 参考信息 -->