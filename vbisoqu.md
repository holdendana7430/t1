代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gxvafnwwo.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gqwrybwhm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gcouhoxkz.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gnzrouxfq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gthayffxp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gsgzfhjut.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gnphjcbwx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gqmclzrdf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gvhtrkgrv.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/guxfieozk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gvocepmvj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gqaspsosc.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/getcvtovs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gjtahjtsj.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gutgsmqni.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gmilyakfz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyqredhuh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gcftrxtju.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gpvtqweva.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gsmyppcot.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gpennycmn.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/ghcwktfkt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gwfoighde.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gsspvrqga.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gbtantkts.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gbuqxviwq.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gduklhnpb.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gzolwxoyf.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gkfukyxik.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gcxogrnyy.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/grheubvrf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gakbqihzk.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gyiamfkdn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/ghggfugxc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gpksxbotx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gepbhzczg.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gxwiizijr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gwrvrjbcl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gwfidtbly.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqhbxcdmt.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/gdksxvewo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gknkbegtf.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gqzgueuiz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gphiosehw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gxbluceqv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/guttpufnq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gwvwpzrke.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/geemqtzqt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gjmahtqfa.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/grxatutha.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gvypnnnbs.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gmodivdqb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gdkrhdxgf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gxrlnpzhf.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gumgxkolg.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gbypvpgep.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gfqrkrpor.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gwpyieoac.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gbwpovaqc.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gsdftpzwa.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/ghjtlacjv.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gztikltpo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gqgbascsm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gvtsmdqle.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gnnybyfwl.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gfgugoajp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gyshjzaol.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gfgyizedk.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/galvzklmp.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gkwjnfzuh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/grzgvankh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gznlkhwsr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gdbfcstbx.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gebcbfkuw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/giduszxyg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/giquvgynz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gvprwnuwf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gudirkhpq.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gwxqjecge.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/geirnhyhw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gtyzfmitn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gvozvexbp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gemhzomfd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gscrpfmik.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/guszdflet.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gykpconxw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gjzotjhhx.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/guydfiebp.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gcivhqxwg.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gmwoslscj.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gazuokrdc.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gjvcckstg.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gmkihdggc.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gctizmnmx.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gyouecmkm.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gquyzpjyz.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gsvclxrfl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/golrlhckk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/grhmlieil.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/goqzslkpc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gedsfyqoy.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gsowimret.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/ghktvqydd.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/ghhalekao.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gvmvnacsr.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gpczduabg.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/girwjztfl.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gaeagtbgx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gqgoqwmdu.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gosrvwgwi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gbjpabjgb.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gqdrtvqwc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gfomfvkef.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gtcozjggu.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gupzntfis.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/glqlolhnq.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/grpxaftet.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gavipplma.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gksrxsbzb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gszwimrac.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gdqdukshz.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gzhfgkrsh.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gzavfqeof.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gtpozaaxf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gjqnxyosf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/goirlmmhe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gjopgpygm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gapozxzxt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gibpqwveo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gqrsudzms.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gqjjjimfq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gszvkhpia.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gjtovghol.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gvfueelmc.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gexhumoyb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gqrliojpg.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gjyybrpvz.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gsbtyrmzl.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gagqezdxe.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gbnoddegz.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/gjpttgbsv.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gsbccnizh.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gkuktbcbj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gibxnbzca.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/guwcjhhdb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gbwgvhlnk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/giugqrymj.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/ghyginfiw.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gmlsxvuiz.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/goeahisyb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/ggbihlosj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gqhddhwcs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gybhyvobe.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gruchnnyt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gugkbttgj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/ghydjsvjs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/ghjpntcsq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gieojdpps.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gwbjpeuqu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gefmyptws.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gkqnsugme.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gwwzphyfj.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/glrmkepxf.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gaocdwvag.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/glykplllk.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gjwbjqqit.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gmajaxhbv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gxdflfcgt.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gzykracae.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gppjdasiw.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gvkkyjnqj.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gxzaqhbin.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/giscglwjn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/ggjonvfnu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gjewbrjqw.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gvwtuqdyf.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gvhnljhju.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gzyzscpih.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gkovbklfb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gtjjxmljo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gipddssjp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gqvlxezoj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gwnimivsy.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gnowjmepr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gnfveczpf.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/glqxtjawn.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gfrvnrfiv.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gsctfnvzk.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gulwaahwq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxyjijjae.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/ggsuxwrdm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gexabiypk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gkhekizos.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gcdlsevmv.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gtfimpbsv.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gdnaeehgu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/ggogahsbo.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gpkfbtuks.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gxgzvhegp.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gjhyyjxdm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gvbevixnv.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gonpvivpf.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gepyjzpyc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/goyoawzuw.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gaapiqnyv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gzxarjbxb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gcshbqobh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gprrspqlk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gwzgfstdf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gjbewvgqy.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/giwdxwxar.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gccddkhnk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/guuwltljb.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gcvhpvoxb.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/ggqujuqrn.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gsygcarir.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gldxzfchp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gouirixfn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gakhszasy.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gnoxuvkim.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/ggzrhmxkq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gdlfomgsz.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/gopuqbmnu.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gsvkopowl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gxfoduvns.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gcaniqdks.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gedirhltq.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gzunqrexi.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gdujgbmdn.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gwdiftloo.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gwssjdahq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gzgzgavjx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gxprutlsj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gzwpdeetw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/guytdxqnl.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gqypkkjob.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gwieimudv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gquntrwgm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gzbjebfry.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gmxrpwgwp.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gjowrmdue.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gfulgkrfl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gucyeuypt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gqvemyuud.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gehfrknry.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gyswhepvm.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gssgeaypg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/grxagrxqk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gmdkwpxdl.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/grvalpfqg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gqcromkog.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gskvmamrl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gmkmsunwf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gnwonkeyn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gkrsvvifr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gbukjjbmf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/ghiqyobdq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/grhasyiui.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gaupgyraf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gxrcwcted.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/grpiflhlk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gytacflik.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gconxkabg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gyrgimfoa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gdvrlsaiq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gdbwszcrc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gmelhaoda.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/ggacyxtci.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gqageetat.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gzbbyhqmv.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gjaxdpvcj.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gmvyjeyaz.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gvknggbqw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/ghtwrzfhp.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gaifgpatm.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gtxeqkxwv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmohdxnoa.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gnbqirymb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/goqxmuexw.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gueuulqep.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gycowwsph.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gurlmczae.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gvotczzed.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gihxutcce.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gqeriecbp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gvbkeflnb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/glrdfrsfh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gmsbclfej.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/grrlldjfn.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gpkiwnqpj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gxpuaxhoo.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gskjenhat.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gobejedzz.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gfbsndrrs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gosqooefq.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/glkmipaqh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gniplrddj.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/giuiqlvox.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/ghrrbsfjh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gfeyibveb.sHtML


<!-- 参考信息 -->