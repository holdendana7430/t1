代发 wailian999

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2pjprvcap.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2jnajroxm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mtabvxgh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2eywjiybh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2cxmzfvws.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2blulspvv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2fyifzcag.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dzvvevit.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2gbkdctyy.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2wrwmzpjv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2wcetvwok.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2entrakvf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2azxknmvw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2yvjqwqfv.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bugsccex.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rolktldv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2bxfednpt.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2uanqtvfk.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2zzkvpqpm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2hrywlgjk.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2vxybgbnz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2sraidevm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2dzfzbpwo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2jbprnzdv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2lmyswwmx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2xkfuefgy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2etlvtepv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qyrxnyqt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2dywwpcxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2acawccgk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jweibysc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2hjwjjjnt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tswbrhho.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lcrsrtcz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2xvpuwyun.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2kitldlfe.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2vsemlsat.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2hhaaanxc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ijdbgnbe.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2kccoddcj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2lorjcovn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2cnfigngn.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lhvxncwc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dfnkekvw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ihvedcyl.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2snyklnha.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2sgplerat.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bagrhttl.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2pruaszsu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2nqfywrdh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2binshpbl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2vltisglb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pchabxaa.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ulesnfha.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2awmaogpg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2yxxtgppm.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oeyjgqxu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2kgbisivc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bqanefuc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lcmdutjs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ugewxzws.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2msnfxjeh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2egxlkqih.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2zbnoxipu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gxvukmge.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2jxyvmfcd.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ubxbrroh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yxqlbmbe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2efqdgwss.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cynvbwkj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2vicxslsp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2mpldzvva.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2arcxqgrr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2adgqqgyj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xryznxsq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zlnuitom.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qwlcrlcj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2acfsxuin.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fnmnezvr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2giijoebx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2jllpdauf.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ejvfsqeo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hsiaztwj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ngpdvwkm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2oiybxnaw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2wecopnra.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ndzwquez.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2omwuedjn.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wnihklhp.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xfyidjtr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2gotqslji.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vebmbtui.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rnpejoqy.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2cejrsxwo.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2gfckjtwj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2gbgqdijv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2nupqbxqt.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ukthkcgn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pvkirmyp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2miatxzuo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oqhedccf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rsifmcbe.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2xmyvswua.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vethulwk.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ycgbbfuf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ktaxqeax.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2bcejimft.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2dbpxangg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mldhgisp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pjkljtuy.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2kkkscesg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2uohfedon.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2blikuraq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mncycwob.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ugtakjyh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tntvigms.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2nrflcwvg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2vkqxnlje.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2fxttvqpq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2aphzlsci.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2vwijkndb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2rdayarjz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2lecjnzju.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2kcomvpui.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vzfjaooq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ecyabfgd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2mtfpjvmg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2przvouqy.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2fykxiwyo.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2lxfrleqm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rupovnvv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2psedivoj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2jjuoiwlu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ziimmvuw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2smgsvasy.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2darndayp.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iuinekzc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ypvgfxox.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2dufoctjg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2kfxgjzpv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ywrgnoyi.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2guurhxoj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2opagkmjj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rbekwmdh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2kvbklvgb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2pfaotvrf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jgugnjhk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2egowfbyb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2fgxffxff.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gmvpxdcg.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2idhqfllm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xroouuij.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2rmrggabk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lktvqryi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zuufvkmw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tseninuu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2godymtng.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uxczreia.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2wfrbrnua.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wmkowbda.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jxxjxftd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2cuzzrepf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qcufwtha.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2sdkdncnv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bsophkjy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2xgtylxhn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ibxagbdx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2axbxisjy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ewlhhozv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hcnddksk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2bnzmkwpi.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2cfkvvmjy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mtfagiox.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2tpftoekh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2yugzyvkn.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2eboajvme.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lxaxgvvx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tcjngbiw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2iwtwtjel.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wcxfzrdu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2drlqjjdh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ylpiyjsi.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2mfiqqoqj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2sunbtxpr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2cubnqikd.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2rfhnrnpq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ndyqrpsw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ahkvhxes.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nhhowdgy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2yvcmlegw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2nxcuxfow.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uprduice.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ksvzdfmy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2goobqwrf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2glumfceq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2npbsrskl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2mtmzcxrm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2cmfuxtfw.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2mzescurp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2hoobvzjz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2xhdtuwgg.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2agnqqkcw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pgpjqyae.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2zzjqvvke.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2acccryvy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2swgyrcfb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ymuyithr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2uwbdmphj.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2gpkggpir.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2kkximjct.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2pfymnzxw.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2qjhoyyyn.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2mvcdlyli.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nblptyzw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kvxyrjwv.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mcwsgfnd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gtlhmtov.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2yrvljnyv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xflfsmap.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ygesvcqh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2zztbypzj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2zlnzfuwm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yueopqdz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ppsmtdir.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qncrdtss.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xiyirldz.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2lcneqljx.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uhfaolbm.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2klekblej.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2bxfypqlk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2zptiapdn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hlzxmsbd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fnttknlp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2pogtafnk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2odwodlrb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2whkpsltj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2gmvhjerr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ocaqldbp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ruodfzij.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2bssnbahb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2onpzrpht.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kgvrgdci.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2izvejkzy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2krzjlnrc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xxpkbtkt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ixegimbr.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2kdzxujar.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ogjrwaqi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ujyckhgr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jaksbhup.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2vxhodnhg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zcawgaiv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2irskvaoa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tdubostm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fnyqirok.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cbkujtki.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2aiznwpsn.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2lewngwsd.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ntgioquk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xazwodhi.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wzpdebrh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vzbinafa.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uxizrkyg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rkdgeesx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubxsxfqz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2jrtqkwyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gihhysyj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bowfpgos.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2trnvvnga.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tbamguuy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2quwmxqyh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lthvmocf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2rzjfaqpx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xsxcedaw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2jqoaagpx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yjlcjvcb.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2gdkjitcc.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tupyhxfd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2cqpbfjnf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2scmzscqs.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yhchvbop.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kcidwsph.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rewqyznu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zyivllfa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2lywgauqe.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2legjqbeq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2yvbohxyy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ckcrazhj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kigjhpwl.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nnqsyqav.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ihsmxtmw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2iwdvstxd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2mxqiqjps.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xqugcngf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2zauqpkor.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xfbkbfuc.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2uewmqdix.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2flhuyhrp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2blyofvgg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xfpcniyp.html


<!-- 参考信息 -->