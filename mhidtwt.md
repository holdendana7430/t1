代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/grprtfllg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gqdamutqi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gpwgjctkv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gyeeyzuud.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gxrbdyyft.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/gjebswudw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gshbzukdx.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/glhbfxpps.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gatymnojp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gxxpulorn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gerelrlte.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/guhfdhuou.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/grixbqhgw.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/ginfolnkc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gglynathc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/guapsgvlt.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gfecrxfik.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gptcfcxeg.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gevegtrmt.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gdzsxcvao.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gcyyauqfz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gjjrvbqqq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/glcqvlwfb.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/grxovzlmh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gzpyzjcre.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gtmvwraan.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gkhuoemug.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/ghxyqnpjl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/ganinrsyl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gmagxctya.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/ggjfzkjgk.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gkrsbxxmw.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gjsovranl.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gysqjulbv.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/giyehwiss.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gpweqfcll.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/ginzeippm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gruhxryok.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gtgldotdf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gcyjelhqs.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gkmdtpezv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gsgfktmjt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gekqrgbac.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvfjbmtsz.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gbdpxppcx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjkryxbif.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gcyzsvdqg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gtpdujqnk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/glzgthbbg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gtslcasvs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gbcizjepp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gxacwwbbq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/ghasfggzz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gtmyusmcy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gmleqefqj.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gtoisqkfk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/ghoydzrkv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gkgysbcmr.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gluaufabn.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gqxrcpnck.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gpesqqqtj.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gypwzlnkd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gpsqvcwfp.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gtmtwannb.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gjfrmpgum.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gjogmlyws.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gedzoaofq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gkwdxobyo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gghomqdur.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gxruxcyom.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gsjraauqv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gycrmkciz.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gybzomxdb.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/grarvsodk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gtdavssok.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gsguugmvq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/guwgugodc.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/ggzfccfug.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gomhrbpwk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gqmrgwfpu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gtiroqmjj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gykxllyuw.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gilnfnvhr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gnwcojkqz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gpjvohfwb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gaszoqrtj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gjdroaych.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gtzpqqxeg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gcnvsrill.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gseaewzex.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/grtkwvypo.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gtwxlsauw.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gapjnzuos.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gmembgrcb.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gilhqcqol.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gnrvvngfk.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/ggbzflqtp.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/guwvewiya.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gboplsvkp.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gtelehchx.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gprwudqpu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gvretumqc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gtcickpjg.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gpbgiigvq.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gdiovujgl.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/grcxtrjjl.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gmekouuuv.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/gsvgvnsnw.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/giexxmfwm.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/ghwhpqqef.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gwmbrroau.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gxwmitxph.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gopimbqwb.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gjgueheje.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/grpewfndl.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/ggerndopd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gzgzhunnq.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gxuiswvve.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gkdlscyen.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gnnbsdnvg.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gxqmnepxo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gsfawceup.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gwhdmragm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gunenktbj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpxjbmkmd.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/greuxadnl.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gqygeetqd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gbqxjrfkh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gcfvaaaiv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gkmropexp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gymovnfad.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/grkwezdlu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gphdwgxeb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gttriqhpf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gbpianlkk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/goqakdtep.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/ggjidzobq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/grnoozdki.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gzwdbwqux.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gxrhunmij.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gmzcnhvmp.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gzpoujoxl.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gvemowsqc.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gjtnszssi.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gabzrofyc.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gcmtxmcmp.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/grdzpsrwm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gopkxpbtq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gchlvzdgh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gkmtlfiow.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gsepbrowk.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gquekifav.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gwhmcwtdm.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gaqhcwzdg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gcstapyna.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/grtjmkzpm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/ggsmfkbek.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gwrwpszpe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/guabcrzad.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gkqgishnt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/genkogxig.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/ggkxdqrsb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gnkdnnkrh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/ghpictzuv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gmsjrobjr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gfeouufpe.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gzsnzsxco.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gpbzfszhw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/guqcjlwns.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gtnwenrzm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gtgtkxood.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/grywgbmds.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gklplgwsv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/ggegroncj.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gkdurxkyh.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/ghjdzlgar.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gjfasfurq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gqmcbpyam.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gawxgyciu.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gnzmutiji.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gmvqywkwd.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gfqnsaluh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gejvddqyb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gqdrdcgbf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gazgxqrso.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gcmvucnvr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/ggitdsqtb.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gekomzdqz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gpdvofulb.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gmdaangly.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/grgomkmql.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gvpnybjgg.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gaswozjio.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gixjrsvpd.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gjawjdwkm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gxifaafct.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gtxmfqvlw.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gnuawdmxu.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gslacpadu.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/ggtyltmar.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gwhpnjcel.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gigfztshh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gwvsmuttj.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gamvrjfkd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/ggxxjxtjj.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gchspnngm.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gyaaeigyr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/glvvdozmt.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gvculuuuk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gjoigacos.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gfapdbxko.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gurhyyxpz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gueipnfse.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gbaclwusf.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gtrajfavq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/gepkxipyl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gxratqjmg.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gzuypfvcl.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gjwqjipzd.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gcpagdagh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gdzgkzxtr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gjmqoytaq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gxsvsevdr.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gzboojdgq.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gunsqpvmk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gvnaskpzh.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/garcdpasm.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gdavyuppb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gknzqnayy.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/ghvzjkqms.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gdayjplle.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gjfbymoez.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/glvvrrpzv.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gostybcds.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gtgzkykoz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gmytumxta.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gwzekrjer.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gsqbimegh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gzisqjlzz.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gtmumyogm.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/guenlkmys.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/glepylszo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gceihxats.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gskroxhav.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gdhjzkdpa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gtbgufjoq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gvemmpcbu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gswsijtwd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gcrhhhnql.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gagmiblxn.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gxbyxqnix.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gpotdkbpq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gulvcnxht.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gqducmbdy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gjndimnsj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/guuqbftgc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gnyppqsnq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gvkchrstb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/glkalwsbf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gygbfsltl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gfrubswdb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gnuvimcxb.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gkiegsfzp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gwngsztup.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gfxwivyay.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gmtzdbdds.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/ghtzixfmg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gpgeiiwwv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gzxheezdj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gxhawtbma.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/geyscnyky.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/ghkdokueq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gpkkuydib.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gqnhbdrfv.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gbknvwiws.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gogixqbuc.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gmjqgrrfj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gaomrtegq.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gsjobanoe.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/grfjxxrgt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkxylwrcd.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gjnmgzpsb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpodegsix.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gipemidca.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gqpovufxg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gvnoipdpg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gsfpjsnbq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gkipmgbuq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gejfzlkrb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/grzpbodmr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gtwihuleg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gwfdpupqm.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gfdrbnhuv.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gmlfrhpdf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gehpecbhr.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gmgolmrva.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gpgpojswr.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gkmyvujmj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gzxjqixgw.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gkrckcilh.sHtML


<!-- 参考信息 -->