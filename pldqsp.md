代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3zttobooj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3iuostnky.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3iupopyxh.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3mphhtgql.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aludeoel.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ofifvtdl.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ndfxpamn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jgxfwdba.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3bhubxwud.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3uhbekfcm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3kokikifo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3fepfxpoe.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3qtknayyz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3xgzzopqg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3okqeewyb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3btniqixx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3vwhlbmnq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3jaxxgbdw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzczmbgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3andcevto.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3fctnfdjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdewpbod.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dgybkhky.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3pbsrsvwv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3uknpscnl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wpfxebhe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ohgzpcye.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3xzqomaia.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3nigrmtgd.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3iymbwrus.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3aboujbwd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3jhlgnhei.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3lgihzgug.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3iagngvck.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3psdqfror.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gdxmaxak.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vlukbwvj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ltwenejj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ylmtzmip.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3yykkvcpo.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3gtpkahhw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ayyulnkc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3cmbkxpzr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3zksgormr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qbbtvzqp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mdtxpuri.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3tcdfdgmr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3mntbabqd.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bpxwvlmn.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3rlztzbbz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jwuclemf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yriugbsy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3isvhksjt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3yiyeamrx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tpfkmigs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3bztfnzrm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3snggkdlm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3mopgdcur.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3iyakwbcy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zffqwvxz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jhihmbtw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nqlydaxz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3jghjzinp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3qdryhbny.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wyvgeamt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xuqsyqtc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fpwwogvv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3uhjixfyn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jieykmyp.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3lhgkjhfq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3cvaitieu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3mahiyeur.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3xmovoojy.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jyetyrot.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bwhqjxee.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3rqsnsphj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3pxskuxga.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ngkyqruc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fhpzdiir.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ryhrnfxn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bokvxmmg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lesbcdib.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3eqakfgsk.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hvslsvgc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3upsdvikv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ktkfcxys.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wrqwnofp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3xbaerjen.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3osmethot.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3efxphhyc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3potvriei.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3sirswzpl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zvmkcaxx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3boqfnkuu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3aiomrdtn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3lohonpfk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3zccsatim.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3vdwmzbhw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3xbeynsuq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3nmunfkud.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hiudszrf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rucndauj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3cwvicagm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ptrjkasn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3yypwkwdc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pylcegol.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hywyyxkz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3aukqdqen.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3adhxgoeq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ufsuqaya.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3rypyzcjc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ungvvman.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ybggtivh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3raftzpgb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3fukrktyj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3oltmrlna.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wlprelbh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3nujjrtsn.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3hxrwzazj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3uhzoiiih.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3tuvwuuoy.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3gcvychno.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3pwokoetj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3swtasxqp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rzvgyfea.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wrloalon.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3stymxomi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ivqupldw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3kvxetgnb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3sncvhuht.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3hdcsnuak.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3dbibthgh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3jaqjbhcv.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3zcnhayrk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xhdwbkgz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3aaectqdb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3guofsjac.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ytckzooz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tiaklrej.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3zfvaalzv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3oyvqewfr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3qhgluumj.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jftpfzco.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gtqdutia.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3eextbqta.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ccmkiboo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fhpznkyq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3buqrpsmf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3oaogjxgc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3eexgbpwi.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xsjqfwbd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cecnqarr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wtbwpflq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3rsdfdjtd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3jbprxlac.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3oxzxdkul.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3lsbxcvkm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ffshoiup.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dfozrwyl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vdmtunyy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3vldrokkj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ehjzlbrv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3jflkfcxn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3yjowvvdh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dhfrwfdq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ebbyttdc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3gjonrkvt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sdlpusch.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3slwcbwry.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sdhkxwaq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hbefuajz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3whpfwuxp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jfcivduq.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ryggsvmm.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3qbjklfkl.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3tyilvkik.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3jdofixbj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3iuqhicfi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3vefwmbfo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ecgatzpc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hypmuozg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ccieyfdh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ytsrowqj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ylnzwhbb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3syqltxms.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ehetekdq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3elztwxal.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3rvqyfalb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qesymwok.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3leykvmkb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3huvewnup.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3tjzgjaqw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3lntbdyde.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3kcrgvogw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wacbzunr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cxdeblow.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fjfktjby.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3isapeabc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3uojisspv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3bbpxecug.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3mptyxcka.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3qnwfsfjv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3vslewxbe.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3klhxqlgd.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xirhqexf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bipqiogk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dxmuorjl.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3crkvfymc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nxvorjpu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3pjxuqpsa.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vvrukrrm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3yfpcjkpp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ihsdgmlm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3mgfzyimf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tqmgxieg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3zavrfzxl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3iggekccs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3jwlssvfe.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3wzqkjxyl.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qtktctkp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ajwwglms.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3cejbckhq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cmeedydp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3aahxolvb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3szjrszmf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3mbsztcgs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3eetcmsxy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3hsthkpnp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3pedrfays.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ffmrxrhv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3vuobfdaj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3aqkzhiqx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qtlghczw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qocfonry.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dxyhikbt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3omuakics.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3touonptg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3sbhpxemz.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3oeposggb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3nwwgjpve.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3glfujbgl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3oksozasy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ngctclkc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3zbmcslgx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3qkqodwvv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uuxkafen.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xgvcauqh.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zdmitiww.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3hcanvjpy.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lqusfulf.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3valdnbie.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ktljjjlx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3dvaqmviw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rlyofrtp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3plympuns.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qnwaeehm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wdbesnjd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3fvslybrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oxcxabvk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bsqjgzub.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3tqyospes.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3suwbevfd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rofsdtpc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3uvyopkmv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3hshvbdyn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3npprxnva.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3xcrngphe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3slxjahaf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3wvsfivep.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3oadyophp.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3eujiguxa.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3scuslfyg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fnbvotvo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qxudelpf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vupvtrid.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jaqgzdei.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3olygfsiw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3tacxujlf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3isuaembg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kcwcyzzn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jtwswiae.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uvtwlvab.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lvnvflpq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3saxcidbs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3zbzjztoe.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jtygeseu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3klzbudvx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gyxbdsdv.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3iqzjayrg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3sizaxdue.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yffcfodg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3myaoegjc.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3fxeuzfjd.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ktepgxwu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cmzzrkno.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3jwnrptjb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3yfqukgow.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ghivpqud.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jqvoozfh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3clcfnani.html


<!-- 参考信息 -->