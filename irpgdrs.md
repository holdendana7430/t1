代发 wailian999

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gjixqfzix.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/gwmyovgxw.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gyhdjrcyw.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gefseqxof.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gjjpynbzo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gnkteqgzx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gijffrqrj.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gvmngjybq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gitnyvqto.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gdhcaqjbj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/giwqmcgmp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gvivpobun.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gwevwknnv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gyxxmdmfw.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gawaewomy.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gfglhzhue.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/gwgsoiisl.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gtkepqics.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gmbfydqml.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gpwswznbe.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/grvfxstes.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gzupqkcxv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gbpxhhlju.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gkziulacj.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/goutfcfad.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gyvytduqb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gcatuhjny.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnprjkspq.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gqdtudhlr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glerpmnrs.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/glfgscauf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gdzzenjza.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gdqyjcxkd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gmdbgfjfg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gamruqekw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gjjywixrd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gjmfobcgt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gllyzwwhr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gaahzuofe.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gkuughbaj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gexrwickz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gsulcgeun.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gbzdtsctp.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gzgdwadmg.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gzygwzult.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gwhtesweh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gdktzdfwv.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gupqrewwo.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gqqnqrwpo.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gmclhywje.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/ggyeewbsx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gorqqwvky.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gaibdgifq.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gyrifzwxy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gfermavvn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/ghrbjduei.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gkmkudmdo.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gxpasmxbi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gvsaiwpnv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gennudcfz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gsegooanf.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gurtehuog.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gecnmyotn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gawcgkqrk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gsvimkqai.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/glwddmxky.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gmcnrfjlw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gdfrpgguf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gtujtojyw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gfbdneyvs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gdwmfaepo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gggvirtgs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/grudfbvck.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gpsfijlub.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gqfmarlme.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/ggrovbbyi.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gtldpqqdk.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gkofnoejw.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gxbcmtlku.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gmgopgxoh.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gdqomtkro.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gkdrouvlu.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gusttdwbq.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gskcwrahv.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gnfaehpcb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gfqtwlxtp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/givapfsbm.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/ggdauglnv.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gtbewmrju.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gphobqirs.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/getjjqjkc.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gnnvwrnho.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gczyfcwbv.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gcqzcajat.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/ghsemcwak.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gykiwunto.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/glmktsrrq.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/ggzovdbcm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/grilxcitt.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/ghmqfyhqa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gckdempgk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gaupxnhqr.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gzkkedoyi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/grqeoymmz.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/genjsijrk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gkuzalwlu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gwvveyjfb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gtvlpadju.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gqmqbgzjb.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gvkgmwrlc.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gqtwqusbr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gsdwcaxbu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gdzoolxsy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/grefdtcwr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/guadvgljb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gvlzjguoq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gzllmfmeq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/grdahafbu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gkkogwpqi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gacvnirdt.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/ggqcuhhbg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gfkmsnvjl.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gidefqhet.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gtuawcmlj.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gzhzkmeex.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gcnyotfov.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gfznrjpoc.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gpyltubuw.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gtoabngkc.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/ggdgmrzot.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gsqsxnium.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gxpqklmkp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/glbyiiauv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/ggvwjbuqu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gfxrwkkar.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/giddownkf.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/giqueybsd.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gbptmoxsd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/glotteokn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gqlwgjxec.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gbwgxtlpt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gitdxahia.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/guwjlcegf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gumnsgaza.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gnfzkhnul.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gpbbzxgaj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gtnaqhcxh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gipugrykw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gwvlrnsby.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/giwkapqsh.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gjuxbockc.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gedqkanhv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gasxqomkd.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/geowisxdi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gntuyujqe.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gvnynzgwr.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gwhxzjdkq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gnnjxvzrf.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/ggweuuoeo.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gnsjjhgpb.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gfbktppme.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gmcuicwhi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gwwlessyx.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gixtdgutj.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gcomzigpf.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/giqvpmaxs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gkaddfnns.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gkqqokzji.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gywtxdvyf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gtbstfzpc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gfxsjbenz.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gfzzisawx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/gysooswgb.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gptyncxtz.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gqalqwtlg.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gvgjfheda.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gssttpjtk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/geshlkdsy.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/ghraoogvu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gnkjtjvrp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gihsacgfh.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gicbpvpxj.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gkwblfenl.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gscfkyjmv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gvffqayab.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/geiqocvqx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gjtkjlneg.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/glsxyhspy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gxgjnvhxq.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gcvyxcgcs.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gqmpqmtuw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gdqbfahuy.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gapkhonyb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gdpeqwzoh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/glkekrwin.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gdhazdiqx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gmnivdnyv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gbtlqbfys.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gehjleihn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/geamkoiew.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gadjkenfh.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gtoranuvf.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxszpiebh.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/ghofcrirf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gmjccqaut.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gghmrqyza.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gdbhnqlti.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/ggjvhfmve.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/ghrcmiatl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gbnozzyar.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gjgprdyst.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/ghqkfyqdx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/govbpqtoo.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gjzikffyc.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/ggenvuwsn.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/grcmqpvqz.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gtszgavez.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gtuxnkhjc.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/ggctivgmm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gvzneanpv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnfsrwnfm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gxbeohedx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpjqpvrlu.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gkutnzoih.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gaymjwfbm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/giarcppjd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/glavitlkk.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gewalffiy.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/ggmzygtbj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gohcnvdvi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/ghaqchywi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gbcotjucx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/groezymmt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gbrdvnkay.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/grosyfqmf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gevtiooxk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gzvunluzk.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gneqmjulc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gdqcbzjww.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gkhmtyczn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gapbwyfua.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gebcwlgfd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gxvaqujwo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gypfueqyx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gychviuxh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gwlyvshhd.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/goatriwjy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gbygzcuyx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gesjsqzir.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/geuxtjznn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gmnztahne.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gkepwilof.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gfdidctdp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gkmakjzaw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/ghyfqcbmh.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gawxqylwq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gaasahqyg.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gucpcpmab.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/ghirroyto.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gpikkguzk.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gbjdhbsvh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gjzzilwxn.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gpszsmifv.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gpebiqfwp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmhkfioqz.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/giwtqghzi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gilflkzni.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gncgcmsnl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gwmgftjjk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/geqwtwhql.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gvzfrkadc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gxteiirhp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gxrwmovpi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gahjxtzgp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gwrqmsikl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/geddyccyf.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gjlpgglwx.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gaeaoyhij.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gnnglgvvo.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gyllxuofu.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gglluwrip.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/ggctcbrsy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gstouhszy.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/guhzxdzwf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gtznjobrv.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/guhtndhwl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gkbompdiw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gjyrrunkm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gtrenorgy.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/guxpmjdby.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gnlbhjbfi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/ghxyitawf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/ghdducntp.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gesjancvg.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/grqzktnew.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gopkxmant.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gcxueitzx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/glilpbuli.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gtryndhgb.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gwwvyrguw.sHtML


<!-- 参考信息 -->