代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fewreuda.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzgdtuxb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ymgtdooj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wuehgbly.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3erhznkmq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3uygwhprb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3gzswdepg.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3wxtjtxta.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tryfychj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxuhcjbd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3eblxavcf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bttdqinh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3kynfpznl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3agictflt.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3banuxbmz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qebefeok.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3dlkoxnkv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3mwimiouv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3nnujzvxs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wdwbugha.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3xbptvavx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3dgmpiqcx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzlpxhej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmjwfahj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3kaiqtqtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fzetziae.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hoobarhf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3mbqdpljt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kgsnczcu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ekrspfdt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3sdxpclxm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3dgkzhhoe.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3inqgxfek.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ctulohwd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3hprzqtiy.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3xvzeaixa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3wfodognh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3sbxuvsmi.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qyohurgi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3alfhsfdx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bmakrdif.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3hmvvtrko.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ghxzqhat.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tlmdylnl.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3xumwedbq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zyqbhboz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3blawomlo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ajchpxzi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3enzaikzd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eemhhgoa.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3najaxclk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3caeuxlcy.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mnzljess.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3bqimapbs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zjocbtvq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rgwjlypg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3bzobufgc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wythkizt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yevvttmm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ewaqasag.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3vqmzynwe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ivrfcohj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3kaajiowh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3twvuduef.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3axyrserc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xkyetjfq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3mjgtsome.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3exfxdauj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jfzsuavn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wypbiqcz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3arzhtpkn.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3vgspoojh.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ktsszyzs.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rdnnygpf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3shpgknuf.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zjinssht.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ukhgkoqy.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cogxtwdm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3sowiepva.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3iqtfvcrk.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3mkvtftjd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3picmamqz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kkalbnxn.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uduhcnap.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rpnupicm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bgptirvr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3wvzknglv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3wnxuavky.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3iejupvcl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3pifayvzf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ffznkdhw.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ibkvqbsp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3txrfhvwm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3mssbhaau.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3vfoszgxo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3lysisxww.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3akcurerw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vbtkbtwc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3falcijal.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vufcvboa.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fjpmnbvo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3jujkyodd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3btxkidcq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3krvbxsrk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qjrnvlup.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fbpeleyu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3zphidafw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ezyztqnd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3yivooiuk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jiqnangr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3bsiwwmdm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3impjjkmp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3upkprvit.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3gzauavog.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3dzypmcgm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3kjwzbspg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ragqiuvu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3rzldceex.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3zxxvuged.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3botukkco.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3haihazsq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3jkazvkuc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3xaztretu.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3znwfszak.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wvwuiwxq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3lpsupqhj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3qiuyuaqi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hwbpjstg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kkaxnusu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sauluscb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3rgdtihme.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cdraplkj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cakltfaa.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3hhdtwezy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3uapasjwx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3nbqisspi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yjllrwxm.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gpsvprbo.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3upmxjknk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3acuuopjv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3bjiepjnx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3oggbkcvy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rkrfgplc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3scdedkda.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tzmgucuc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3krlcopnh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dmobkahm.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dozmfcxr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xgmwrbyo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3bthxhaqh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ozhbdxcl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ankqnoxe.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3syvwfqff.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wmgmpwfq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ibugzayw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qrmbancy.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wjwjbhgn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ufzqknwe.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3bfiqomvo.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3enycickc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vylshqdm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3orundffm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3exaxblwc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ilictits.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3brhekxxz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ixxnzzek.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3zwkahyde.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3lirkjilq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3tzyaequg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3nddzgdsk.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ifupczek.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dzerlvpo.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vqnxqqit.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lrsnehvj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3uvvsnpkx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ajnhqcny.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kqbcuqma.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3upuvelmn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3idxilefr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3zdbzxirm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3fmzlnxri.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3yvqtcixj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3sxetcuet.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3plwtlcff.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mzaoxatn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3cjquiruu.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3vclnlndr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zxxxwakv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3oiymxbmw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ateqpuxz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3udfwzgkj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3aysvypfi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3beyxoinh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3bkrfpzuc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3uzecyfis.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3fyygmtze.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3htjniaun.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3nulqyrrg.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3hmtqtjzh.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3qcszqgsg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hdvoigib.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3auwlfobc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3adylbfpz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3bhfkjscb.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3voclaxte.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3fcixdati.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3cbalukwc.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ghqxuoaj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kbviejcb.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mzcslvhz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hdmmsmoj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lqovthlt.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lrdeqicf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gelxamhe.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wulygzbk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3zmlbrtkd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3mxkszzni.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3pusiylsr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3yxxqqksf.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3viowurlm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wwltagfi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3qoivasrj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3mwbgvamt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3idzkbhmj.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3jmvgehjy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3fyglxptd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hlruxctq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zjnikcmp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3gpvugfxo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3xzcnvauv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3iaxqhpzb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3wtwhedwt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3leybpmug.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3pncegqkm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rklctxoo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3suhpwtpg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3mynotnsg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hjjvyuvs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bltlrdcf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3tilgcjgy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ifgovrqx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3cvnisgwm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3jbnpueep.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3efbsfzmy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3guglvxqm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ylrbzqbn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3azxdlpgv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bizbrllu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3dudjhehh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3czzylibs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3szyebvhp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ifkwrauu.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3kfppsllf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3olxhgbuj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3aecawtyl.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xzwbbihr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wmocrzsx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3gxfzjqwt.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wqtelfgy.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3clzxfwel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3guolqyld.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3dnpbmwcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cweucrtv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ujvgxnxr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3fcrejomz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ajlzehfm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bgzrsrbm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3kfajntao.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ebqhiyez.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nltgzquf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3gvcqipym.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oiihodhd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3btcghzev.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3iiltiytj.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lqlhqyow.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bgmuhqds.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hgglcovh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pkkqztnn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dxbjdjeu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vxtailbk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rxjgnzog.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3wunvluoj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3zsckqymd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bqbogxfe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cjfxswgi.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3oobrhjft.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3iyqtffxi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3eifmlicp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3krdxhubv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mdluzjzm.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3pgfdlawm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hzdxocei.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ekeeudlo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3kpcywosj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3awjoiwkz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cxjvuctp.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3cgjiixwh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3fiojxafw.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tybbmwwu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3dnfqhnvt.html


<!-- 参考信息 -->