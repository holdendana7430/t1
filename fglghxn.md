代发 wailian999

PHP:  // 无重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gednunlwr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjokmuab.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvvkhmqb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fanxiaobao.xyz/Article/details/grgusnfax.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fanxiaobao.xyz/Article/details/gykjsizfo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulpfgtku.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtnuklrnw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjddqamuz.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwlavnzv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gnsplszbg.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fanxiaobao.xyz/Article/details/glhjfzltm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fanxiaobao.xyz/Article/details/gngpnvwcr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fanxiaobao.xyz/Article/details/ghddcchyn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fanxiaobao.xyz/Article/details/guydwhlqt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldhbapoi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fanxiaobao.xyz/Article/details/gmhvoqeex.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxyfzovh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fanxiaobao.xyz/Article/details/gehirwkqp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fanxiaobao.xyz/Article/details/gpuylyvij.sHtML

[D02] 追加元素到末尾
来源：http://3g.fanxiaobao.xyz/Article/details/gggbqzwew.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzmrgklh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fanxiaobao.xyz/Article/details/gnnwydfrh.sHtML

JS:   arr.push(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgiyarfz.sHtML

TS:   arr.push(4);
来源：http://blog.fanxiaobao.xyz/Article/details/glzjxvgpx.sHtML

Java: list.add(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gwlbjsewv.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvchhaid.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdnunbtk.sHtML

C#:   list.Add(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gapdkphqk.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fanxiaobao.xyz/Article/details/gxgpovisa.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gttexywqz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fanxiaobao.xyz/Article/details/gpanjdfna.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fanxiaobao.xyz/Article/details/gbzznibzx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/grtbprabx.sHtML

Java: list.add(0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gflzptdwg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fanxiaobao.xyz/Article/details/gffqtnmxi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmokcshms.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfprnjas.sHtML

[D04] 删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gycopqboe.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gqxajhuyo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gjowjggxe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fanxiaobao.xyz/Article/details/gkfynkkbp.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gatbhdavz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gvyeigvsq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxufogjzu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fanxiaobao.xyz/Article/details/grcqrzqos.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fanxiaobao.xyz/Article/details/gtdqcxnyh.sHtML

[D05] 访问与修改元素
来源：http://blog.fanxiaobao.xyz/Article/details/gyekqbfzz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/grhcvgwbp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gdfkhzvya.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyykrjotn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghphuixdo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fanxiaobao.xyz/Article/details/guxxbxlyo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/gecjqymin.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmjalmop.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/gozzckhvr.sHtML

[D06] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gdpxtvyir.sHtML

Py:   len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/grdijydzl.sHtML

PHP:  count($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gbspiyrrv.sHtML

JS:   arr.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrclyixl.sHtML

TS:   arr.length
来源：http://wap.fanxiaobao.xyz/Article/details/gvhwplqkc.sHtML

Java: list.size();
来源：http://baike.fanxiaobao.xyz/Article/details/gfnwyqkak.sHtML

Go:   len(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjcrwsuk.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fanxiaobao.xyz/Article/details/gaacyzyqv.sHtML

C#:   list.Count;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golsthiqx.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkiwzowv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzrdafmu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwhxsbgc.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/gasiczccm.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gbbonyfzx.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbzzuptb.sHtML

Go:   arr[1:4]
来源：http://baike.fanxiaobao.xyz/Article/details/gyczzzyta.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdledeydb.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gllmidlsa.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicmluzuj.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfisbyrow.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdchalgq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fanxiaobao.xyz/Article/details/gqldqcehi.sHtML

TS:   [...a, ...b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gpayjbjhg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gnweuajdw.sHtML

Go:   append(a, b...)
来源：http://3g.fanxiaobao.xyz/Article/details/gwxcpdvfy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkbroybq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrfaosfu.sHtML

[D09] 排序（升序）
来源：http://read.share.fanxiaobao.xyz/Article/details/gafenbhwy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/glzokitwn.sHtML

PHP:  sort($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gwtqojqzf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fanxiaobao.xyz/Article/details/gveleoaxl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fanxiaobao.xyz/Article/details/gijhmdvvo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdkdstxw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpukeouj.sHtML

Ruby: arr.sort
来源：http://read.share.fanxiaobao.xyz/Article/details/givigorfq.sHtML

C#:   list.Sort();
来源：http://blog.fanxiaobao.xyz/Article/details/ggipkuqzs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfdeneem.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonjrqrrq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gpdgzydbd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqiwwetg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fanxiaobao.xyz/Article/details/gfqgtmhdt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvwsclsa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fanxiaobao.xyz/Article/details/gonuwfptq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fanxiaobao.xyz/Article/details/gelupndlc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fanxiaobao.xyz/Article/details/gddtasfsp.sHtML

[D11] 反转数组
来源：http://3g.fanxiaobao.xyz/Article/details/gscsedmqv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fanxiaobao.xyz/Article/details/gkbrjoadf.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvsrvdqz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvupuyrvl.sHtML

TS:   [...arr].reverse();
来源：http://baike.fanxiaobao.xyz/Article/details/giklnzduj.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiiwyflg.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gybrbhhfe.sHtML

Ruby: arr.reverse
来源：http://wap.fanxiaobao.xyz/Article/details/gmudysnbv.sHtML

C#:   list.Reverse();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzzvzhxo.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqsdcmid.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fanxiaobao.xyz/Article/details/gbugnasvx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeddabyj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gochjqymu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpefqwyrc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fanxiaobao.xyz/Article/details/gzgjjczmo.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawntkpnd.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfrradun.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fanxiaobao.xyz/Article/details/gyqyxnhxn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fanxiaobao.xyz/Article/details/gtybszxoc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gsfqcyddw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliupblri.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grklxygkk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/gkaunaqsx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gocbkcbzi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzktykyb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fanxiaobao.xyz/Article/details/gkpfbwxwy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gpjcvwokb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/globrnkxr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gwubkgxdv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuvccajl.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/guhgswlyy.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbmgrlnq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gubqgdiuh.sHtML

Go:   // 手写循环
来源：http://wap.fanxiaobao.xyz/Article/details/gagixhqnq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gtngkkgar.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gpytuwiof.sHtML

[D15] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhtwhced.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfaiadwb.sHtML

PHP:  array_unique($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gycivjoax.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gglxdbypy.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqcyilmg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fanxiaobao.xyz/Article/details/gomxrwznu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvocqukuw.sHtML

Ruby: arr.uniq
来源：http://mobile.fanxiaobao.xyz/Article/details/gszldsyuc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuxwtsul.sHtML

[D16] 求和与平均值
来源：http://www.share.fanxiaobao.xyz/Article/details/gccffvkca.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gksdharpz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/ggimyfzvq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gifknvaai.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gpfayudca.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjytohzek.sHtML

Go:   // 手写循环累加
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpztzxmm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrvqzppx.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fanxiaobao.xyz/Article/details/guqyrmjcm.sHtML

[D17] 最大值与最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvuqoplm.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkraffpq.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gbqqljppq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwywxvqps.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsycdkbjm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjswbepa.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/ggwyetipx.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fanxiaobao.xyz/Article/details/gtomixfbo.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fanxiaobao.xyz/Article/details/gsstbdmdx.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwkmjuph.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkrmyhkj.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fanxiaobao.xyz/Article/details/gbfnutnep.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtdwnkib.sHtML

TS:   nested.flat();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkyhncbq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxpolkyl.sHtML

Go:   // 手写双层循环
来源：http://mobile.fanxiaobao.xyz/Article/details/goxywwxhp.sHtML

Ruby: nested.flatten
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyynsmsr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmiqbngv.sHtML

[D19] 按字段分组
来源：http://baike.fanxiaobao.xyz/Article/details/gmmvdxgex.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmeqvwvm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwmvkfoy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fanxiaobao.xyz/Article/details/govclghmg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtymehvsb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fanxiaobao.xyz/Article/details/ggwhjtywh.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fanxiaobao.xyz/Article/details/gllvwgtwj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdoqtsujw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuevzglo.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fanxiaobao.xyz/Article/details/gxepctilf.sHtML

Py:   Counter(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gvuisqjqf.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gitdwpifk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fanxiaobao.xyz/Article/details/goocyxguh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvvtmptx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fanxiaobao.xyz/Article/details/gguzyccdz.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fanxiaobao.xyz/Article/details/glashjmuy.sHtML

Ruby: arr.tally
来源：http://wap.fanxiaobao.xyz/Article/details/gzdwbbnee.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fanxiaobao.xyz/Article/details/gisbkljnz.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsfcvfby.sHtML

Py:   x in arr
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkfmvtic.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gzlluanqz.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goufqjfeg.sHtML

TS:   arr.includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gfrerfqzz.sHtML

Java: list.contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrnmaauc.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhaurvun.sHtML

Ruby: arr.include?(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gmbdfvggx.sHtML

C#:   list.Contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyrxmlzv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmseewbg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/glejqvlvr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fanxiaobao.xyz/Article/details/ginicvosi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnebslwe.sHtML

TS:   [...arr];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfkqolrg.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvryrcds.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfstfaaz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfovffua.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsfgeffj.sHtML

[D23] reduce 累积计算
来源：http://wap.fanxiaobao.xyz/Article/details/giydqxzrd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrrwijvq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gobtwobpw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcfadkfx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrdssaoh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiogwqol.sHtML

Go:   // 手写循环
来源：http://wap.fanxiaobao.xyz/Article/details/gjpctktds.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhkhjhzq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhcixuxt.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fanxiaobao.xyz/Article/details/gcyvqfyfw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fanxiaobao.xyz/Article/details/gujephddk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtzehreg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gtuvkvzrz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gxqlylvjx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fanxiaobao.xyz/Article/details/gbeklmbms.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fanxiaobao.xyz/Article/details/gmmcjfsdn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyrcweal.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fanxiaobao.xyz/Article/details/gkezaayal.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fanxiaobao.xyz/Article/details/gfuvzwmlh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fanxiaobao.xyz/Article/details/gcmgdgkmm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fanxiaobao.xyz/Article/details/gijgjngrl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gxqzmgrdz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fanxiaobao.xyz/Article/details/gdjvkjugu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnkayifs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjlmkbeq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjrgdxqe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghatembzo.sHtML

[D26] 数组转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlmjbsuj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcwbgtui.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpowywcmq.sHtML

JS:   arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuugdxmj.sHtML

TS:   arr.join(", ")
来源：http://3g.fanxiaobao.xyz/Article/details/gwxblzpgg.sHtML

Java: String.join(", ", list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gufndygil.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghezfducu.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdowghhd.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fanxiaobao.xyz/Article/details/giidnrygt.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnexwbax.sHtML

E. 字符串处理
来源：http://blog.fanxiaobao.xyz/Article/details/glvqjxtod.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoocsvcq.sHtML

[E01] 拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gqfhlojwr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fanxiaobao.xyz/Article/details/gdfgxzlve.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwddybzdn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fanxiaobao.xyz/Article/details/ggqlcpmhj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftalfoyl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzktxgqu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhqilfvd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklzhwxdc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhqvjxcz.sHtML

[E02] 重复字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilumpuqd.sHtML

Py:   "ab" * 3
来源：http://blog.fanxiaobao.xyz/Article/details/geiyzgqyf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjhomqxe.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpzftdfq.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesbhtlnp.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaczugczl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjkajkeh.sHtML

Ruby: "ab" * 3
来源：http://3g.fanxiaobao.xyz/Article/details/gyqexfaud.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gqrjnytez.sHtML

[E03] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlovcoph.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fanxiaobao.xyz/Article/details/gehdyydpx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fanxiaobao.xyz/Article/details/gejgneova.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgvjmqsf.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fanxiaobao.xyz/Article/details/geekuapti.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkageebmf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsmnrivq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysryxwmx.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fanxiaobao.xyz/Article/details/gedrgbaul.sHtML

[E04] 查找子串位置
来源：http://baike.fanxiaobao.xyz/Article/details/gcfxbkjoq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fanxiaobao.xyz/Article/details/gzfwsnhyu.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fanxiaobao.xyz/Article/details/gbsayvoib.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkmbsxvx.sHtML

TS:   s.indexOf("x")
来源：http://wap.fanxiaobao.xyz/Article/details/grljpcnvz.sHtML

Java: s.indexOf("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gskmxuamr.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fanxiaobao.xyz/Article/details/glwsvjcfb.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqzyqefq.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkdytmxf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fanxiaobao.xyz/Article/details/gkwqzquuz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fanxiaobao.xyz/Article/details/gchfgqziw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzfizsvo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gsdbhabyq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqganstt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjhqpemb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzpivrlp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxejuigg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fanxiaobao.xyz/Article/details/goqwwaphy.sHtML

[E06] 替换子串
来源：http://3g.fanxiaobao.xyz/Article/details/gguikcnwt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gohqcbmdl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrlvtvql.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gbujuqyfn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/guwxqtzeo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gxiqvvczm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gxcsydmem.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gnnnscsgb.sHtML


<!-- 参考信息 -->