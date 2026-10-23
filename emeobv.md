代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3wzwsmoas.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3dtfaeeui.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3dockniim.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3jygwqxdu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3vslpwfog.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3cfugkcfk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3cccfdgyh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3goegofss.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3xhhmfjzx.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3tmvaffvx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ktwbgmcd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3masgrwef.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xpiqxcwf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hbjixbgf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3lyoybbkc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqhkprrr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qwfbluhg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ejbhenxk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3cifycwzc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3rnpdauls.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3mxwylqwi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3gcvxtdua.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qxhbpyjw.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dranukyg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jycllkac.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvjvfwwy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3eheyichh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3athylhph.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3zipdwair.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3eraqsetq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3vvqkepqt.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3acideyjh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3krmfkant.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3qrgehatu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3pkzyqhze.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3peyixmbn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3eiwhcbmn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kbkkvmaf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3mtswgazh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3dcploaql.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3qumjavmy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3kysedghv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3eusjdkzh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3hptuvrnr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3aqrariue.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3yzufkqzg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3jckcgncb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvwjqjto.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3tpunttog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fgriuxvy.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wffpzwcj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3jlzeumvu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wndyiszw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3rwbzyrpm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3nbasbfcz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3qlmwkuzh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3dqjplsum.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fmmonddf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ialrkijg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3lgzqtxbh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3utkftzpo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3nnsdtumo.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xhkuzctn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3olwkvbio.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hkbbxvgr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3srodznes.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3pypwrnys.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3anfiqloe.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3qvksijac.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3xyuoylns.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3pdrmljbu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3noxcwuvd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yczumnbf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kdtzspxr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3bmyasgyw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3pncloyyj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3scotzrfl.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3msojjbkk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3rndbtyeo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3urlivrgt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3xtbopike.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3dgofxzwo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qtksbftc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3gpkmampw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3tngveqwk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ynymcvww.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3bmtjjdtp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3sabaaknh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yfvzbgcm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nvikkpxh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3zenicrny.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3bcjcjxle.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3npdjjiig.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jqpambii.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bjrsyjpz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3oqzgoegg.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3glldjitj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vkbxvegf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3eveansmy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3lhkxbsfo.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3auxfotea.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xjvnhxqg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ixrjewmc.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3hefpbhzz.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3frlodace.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3umgiwxtm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3yogbpclm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mpdbzryu.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ezlfoqaz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wduhdoif.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3toaulola.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wufwdqcs.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xnwunzqv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3lpxggzkd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3srlusabe.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3oehxgpbh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3hcfgwfkp.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3svbutuyk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3gleigtnq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3dlhmmjat.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jjmdehfa.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cdfdjjjj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3xaocjanq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nafctxsh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hbgmesuj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3vtpviegy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3kuifcrin.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3wcdhlwwf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rdatysmk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3onzykass.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3vbmpbsga.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3gczkuvxa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3nqbfcirx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3znpvjxdw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3yslszram.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wrwpgcdr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3zkgcibzo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3wvpdvasc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3nbmjbtvn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3uruyikqw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3gzapnapc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3iqpovkul.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jrlwjket.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3mgssyqxt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3riyjftrg.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3yqheriav.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3dvmsftaj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3vqoomfho.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3dvgmyqac.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3cbnhzjok.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3inojmnpv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vozepwmc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cntbudpv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3oaiudclq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ffmkckmp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3moohrzec.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rfdggwjw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3qrsahfmx.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ubstypdl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qgaknnny.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3wlaaqmxy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3sxdkuhtj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3iiowwbrr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bpdhnhvd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3hfekkuru.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3pnvpydke.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jlzldtaa.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3sabpkhrp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3afahyjei.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nmikgyjk.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3urkiwwxs.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pkponzxx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bsvpirrz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3zepnmrvw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nipaqhjg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yhcjjdgo.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xnlarxfe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3goagbpca.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yabdgpii.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jpvalxvd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3viwneeoo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3cxhwhddg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3zzhqphff.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3visveoek.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3psieynkg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3vaiqtkct.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dqvfhrwg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dpwblcry.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3gkxaoovm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mtwrxioa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3yzbbkumo.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3qywtwwvt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lamdtvuv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3hrezqhrd.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hylsdapd.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nenhufkp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3xvbptjvz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3rmdwniwb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3dnxvggpo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3yssrpauf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mhoyulrc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3opgwibrd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ollrfnfl.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3qjrkffyx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3kzaatkuy.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3tkymdcao.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3befozihs.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3wsrlsjri.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dpxrkwie.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ykpvzhkx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ragpjvba.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cscizvub.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ttlrubzi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3rxjinyym.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3szqndwet.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3patzqzws.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vixzwzzv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ayqnnqri.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3cyqrqnqe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3rwvolyjz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3qaaeldqg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ovrlfjzb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3imawqcbz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fymdhyrn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3resbxtbd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jdzhzwat.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3gjaifxuj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3qsktmygo.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3owysanvq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3zdwwjryq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3hknglmis.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3elfpufns.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nmganytr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yvapxtnk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nuuairum.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lhtcxayh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dsmsorqy.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3kqdkpwqb.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cxnxyewi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3gkqcimlx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ernwemvs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3fgsqkbuw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ecezitdg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3jjqiwmmz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3jdrwqpac.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3piuwcrsh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3qrgczfgs.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jbemigmz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3nybvvesc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tvsfqnnv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3stulxuif.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3bklavrwc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3gjbirtix.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3aybszgei.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ocikdegb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3hxlsppal.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3hlohqeiy.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3gcgoxpxx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3dcxequla.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3zriuzddd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3irqhilnh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3czfoneyk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3outrtsld.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3bpwdlfet.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3gmrhawle.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3lhbgsfqk.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3zpjweoun.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3jyazgjkf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3beueundl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3clgksaub.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3qqyeknyn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ebkiphbh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3yilmjgom.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3iwylxzuj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3epzvbwpd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3uxbjdnic.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3hcyiigjk.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ecriovge.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mcmqxstt.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3egsxrzsq.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3aqoskdxu.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fcpstcub.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hzcrehkk.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3cqrizxcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xcaqvwij.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3zofwcssh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3potufiug.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3aaigtbok.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3xylupwkq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kdwhdguc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ldvqzrlw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lghuleuq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3avrbliof.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mjfrmcvj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3sphfrzar.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ciqewoqp.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3cuzczvna.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mxqsybfl.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ovvzkflx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ycgpwyly.html


<!-- 参考信息 -->