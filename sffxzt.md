代发 wailian999

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3otfcjeku.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3bnexikrk.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3nfdqmfyj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3waeeqyvt.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3atoxyher.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3eylzodiq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ipggctdh.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3wgcchvxv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3mzymnqyk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ppljenan.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ixpymcqm.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3qgumnovu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ywcwwigy.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3smzoxquc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zduvtnry.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ffqlbibb.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3mpppnhyf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3cqofzdkp.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3mvrtffjf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pgljxjjy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3kqhovbpl.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3larwulvc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3gzqnsrkm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3vsgucsow.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3hwrhftet.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3fwknlhjm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lzwjnlft.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ejqzrkar.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3qlrsyoak.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3nvsbwblx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pzwkvwwm.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3motgyymy.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3unnfwqbb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3xlgwppmv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3tejzudpo.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3gsfogqjl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3uocoqwts.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3dhkvmjou.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3pscfwtrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rulbcsln.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xooqfeea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nhplsqqu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ddotkusf.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ghkvtnly.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3okeiqpfk.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3erpmolju.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3dyttgvdl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3vkmjvjfc.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3inqrbhlx.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3tlggzpfm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gforizpw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ubrwcuxp.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ghntptli.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yfvoorpd.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ekuwjfjf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3zxfggfge.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ybweylhi.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ulrdqlgu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3pkcpfdsz.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3rvnbvhfk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ucliptxv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3eqadhafh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3phcgmuig.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xemivxuo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ugvvorvs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3hdahdlsv.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3biphudpb.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3leivafvc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jxymcuyx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3fvcgpbcy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3zatjspqk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sikohcps.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3uercnkwc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3usaafnhm.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3osbtbsvw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3hrubaggm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3pjsqvddl.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tducmblo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3nenqjzon.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bbvhmujr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3bstdmmfc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3thidbyre.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rcpsojju.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3jtdylvhs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3beqlzuxo.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ikfsedmi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3xvteqklw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hcwthzko.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ymlkqzjs.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3cxnlfirk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3wdlowvqu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3hzzxcogw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3xbhhzgtp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3syjouvpz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3sdlpptsu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3wqbwwuaq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3yiefddrq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ysjccfpv.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ymwyaokw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3bxehjukv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3wgppppxf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3exuvdrzg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3udkahhuh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ogyyzitn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3obncnhgm.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3oheqdowc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3hlsdiqdy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bgjvnnsw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3nyaaqgyi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmjaxiks.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lmszfaif.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3jbyyzgnm.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3cthdtohu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3wvxszwlw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3zdkzhmux.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3zbkheoih.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3irxbjhlz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rvyqvnst.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3yyvodkvn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3epvxbkab.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3lphpnhzi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pyabnnwc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3swpgmecf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3sakjcgpg.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3fvlqbofu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ctntmrkj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3hqyszgff.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dixkfvgn.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3kaqpgfsk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3kjpgkmsk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3dggipxix.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3mbmhpjkg.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3pizwnxir.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3clmleskj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3anupqjfi.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybrnxgab.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3rgijgdca.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3dtosgzpu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3rxgxdyts.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kndftsrt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3pvwltpcp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkibkxmm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xhxjxvgx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3onjznsfk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zcoxlxqu.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3rwtimfan.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zeboaqqy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3oencntwa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pimwiwii.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3zdhqqpju.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3wtwouabs.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3hxhjqpyv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ofemtuys.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3wamgpojp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3tatekxbo.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3sjaudhrf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3sbacnuxq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nyesdmcv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3vfxncxon.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3lxqupbhc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3grbmfsdp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3nuknmfoe.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3pjyvziqy.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3supfspzf.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3onaalkue.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ctvmmlrg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3nyrlpncv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3onvzcjyi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qpzbhlgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqzucmse.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3mwrjafyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vhpwnvga.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oncmprri.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ifxcvijg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3hmzzvftb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3rruoyxhs.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3xdakbzrt.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xdncuifg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3wvrijubc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3mxjlqcym.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3eocqvqlx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3fovddeuj.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3unntjnnc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ohrleqcu.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3znhslphh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3uyywxszs.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3pmxyzqom.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xlsgmbix.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3nmpfnitl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3zhajkmxg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3wgnclttx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3dydfincy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3mjcbkhbc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3canbnfrg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3npijxrlq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3joacdrdf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3iymzilpq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cpmvdnnv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gwikguwe.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hfhdqamj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3bzkjwvbd.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jypjzuhk.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cgtqckaf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ephyveip.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3clffnonx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3tmzcfgln.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gfkgkldt.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3kazciptu.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3uwueljzd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3qyblexxn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3higxurxo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3kfyhojsk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3vwhkzeho.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3pkrudtdz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3eqtldabg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3gientoyy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cuvewghq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3jbcotnat.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3wkhollis.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3htnrscjk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3yjjsjtpp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3fcitsrtn.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3boxngsim.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3fmqgnebg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wednlngz.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3fdzqsacr.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3tlwllase.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3flxekhbt.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3cfknsitp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3laxvholc.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3hwqlrgnv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3olldubjd.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bblbwxzo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fjwtzqsg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3sbupjffm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mtngeivd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vlkcrvgu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3xijjkvsb.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3lgnfqvni.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3npfgdveu.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3dhtwiueo.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dglshvcv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tjqplrtw.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3dfsqqbcl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rvwmbcas.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3spyhfula.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3wxprgymr.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3lukmsvrc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hvwzfqdk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3gecivnvn.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3rilqdoxf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3jmqtretu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jrozqvkw.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ngstrxdi.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3tpnicmrp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mgdcttal.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uehoruln.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3eupqphsi.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pakkwljz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqcldnxm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3olerjxqb.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmdrevrq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3cwqofpzk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjsgodra.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3zfmrjwjb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3wjhomiww.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3vvvwekdy.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3srxdlgvn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uwbvayga.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pcfyiaii.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nulmoizs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3gjgkhzzi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3fayhfnop.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fneftvfj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3shcaaixr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3wslnwext.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tilhlffb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gflmkolj.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ackstufj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lvajrqtm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xdtvfuta.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3upljofnp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nfxsvfrv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3fjrmphaq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mthsbkef.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qkecmfpd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3huhwapod.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ubpeudgl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3rjftrtlk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vggtyfvj.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3mxbnqjsp.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3sormoohn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3zssjluvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3szvsuwct.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3wcvmfmoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zezzayez.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3siqygefk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3vefnnbee.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3qhaxnpio.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tclmwqjt.html


<!-- 参考信息 -->