代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sysykeji.top/gtwptulvca.html

[R56] 远程拷贝
来源：http://hz.zhijiandao.cn/gtlhvpzotz.html

scp file user@host:/path/
来源：http://hz.cqqwz.cn/gtxxesfeos.html

[R57] 远程执行命令
来源：http://hz.xuetiantiany.cn/gtzfiiktcl.html

ssh user@host 'uptime'
来源：http://hz.daxiang520.top/gtpbwyuxhg.html

[R58] 下载文件
来源：http://hz.fengsongda.top/gtdufawrjx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shangyingyoupin.top/gtmfyjetlv.html

[R59] 发 POST JSON
来源：http://hz.shangyingyoupin.top/gtkorexfiq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xuetiantiany.cn/gtcwvzasmv.html

[R60] 只看 HTTP 状态码
来源：http://hz.shuidangran.top/gtwlwokhmk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.mhx1999.top/gttlqailkd.html

[R61] 磁盘占用
来源：http://hz.yj20258888.top/gtysrczewy.html

df -h;  du -sh *
来源：http://hz.wangdashe.top/gtdsvjkrib.html

[R62] 找最占空间的文件
来源：http://hz.0kj1m.cn/gtchemqnve.html

du -ah . | sort -rh | head -10
来源：http://hz.yvedp.cn/gthezhjtic.html

[R63] 内存与进程
来源：http://hz.shzxlz.cn/gtcvuofyzj.html

free -h;  ps aux | grep nginx
来源：http://hz.nanxinkj.top/gtsqbniczu.html

[R64] 结束进程
来源：http://hz.zhiwuduotai.top/gtrwmjqwvt.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yuxming.cn/gtrrvbxxuf.html

[R65] 查看端口占用
来源：http://hz.shzxlz.cn/gtmioiurbf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.mhx1999.top/gtqzykcakc.html

[R66] 定时任务
来源：http://hz.guowangkeji.top/gtrdszsjsu.html

crontab -e;  crontab -l
来源：http://hz.kuanghao11.cn/gtojaubvxr.html

[R67] 生成随机十六进制串
来源：http://hz.cqqwz.cn/gthkvkqwdb.html

openssl rand -hex 16
来源：http://hz.yj20258888.top/gtiibdsjno.html

[R68] 计算文件校验值
来源：http://hz.zhiwuduotai.top/gthssqrjvv.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhaomingkeji.xyz/gtlqkovarc.html

[R69] 生成随机密码
来源：http://hz.52xcode.cn/gtkojoyrxo.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhaomingkeji.xyz/gtwdpyguzc.html

[R70] 时间戳与互转
来源：http://hz.hfpthk.cn/gtvirkzapz.html

date +%s;  date -d @1700000000
来源：http://hz.aibaodan.cn/gtwbtxwicp.html

[R71] 日期格式化
来源：http://hz.birdmap.top/gtyvnjszde.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yuxming.cn/gtqllizobe.html

[R72] 等待端口就绪
来源：http://hz.shanyushiyangkeji.top/gtitsrttee.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.vqdsnc.cn/gtiqxsngqm.html

[R73] 分割大日志
来源：http://hz.zycfv.cn/gtxtevhabk.html

split -l 1000 big.log part_
来源：http://hz.yongpay.top/gteantpzyk.html

[R74] 批量重命名
来源：http://hz.guannengcc.top/gtrathumcs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.guowangkeji.top/gtylwuxfyk.html

[R75] 导出环境变量
来源：http://hz.gaohongyu789.top/gthkjgfkiv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cucudq.cn/gtiiwtqyvt.html

[R76] 使用临时文件
来源：http://hz.ywan-chungtsiang.top/gtzeujnvvg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ydjk.org.cn/gtdynzebjf.html

[R77] 读取用户输入
来源：http://hz.guowangkeji.top/gtijfufnil.html

read -rp "请输入: " ans
来源：http://hz.9152youxi.cn/gtxodpdmgz.html

[R78] 交互式菜单
来源：http://hz.ydzc1.top/gtcrivwnml.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.aizwys.cn/gtiyqmrmdl.html

[R79] 解析命令行选项
来源：http://hz.yonumen.top/gtcycjexyk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.birdmap.top/gtoxxetvit.html

[R80] 查看脚本执行耗时
来源：http://hz.hammf.cn/gtichaaklx.html

time ./run.sh
来源：http://hz.shuidangran.top/gtcyayiypx.html

================================================================================
来源：http://hz.yangfankeji.com/gtbyuwjsaf.html

S. C / C++ 专题
来源：http://hz.shuidangran.top/gtoqryuitt.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtykavsznz.html

[S01] C：Hello World
来源：http://hz.fengsongda.top/gteibdiavb.html

#include <stdio.h>
来源：http://hz.yj202588.top/gtqlhciznd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gaohongyu789.top/gtygardrez.html

[S02] C：变量与格式化输出
来源：http://hz.shanyushiyangkeji.top/gtdcqasbtl.html

int a = 10; printf("%d\n", a);
来源：http://hz.sysykeji.top/gtekmnkdjo.html

[S03] C：读入整数
来源：http://hz.svipenyu.cn/gtlxtjtmpr.html

int x; scanf("%d", &x);
来源：http://hz.hywenlv.cn/gttzvhswvr.html

[S04] C：字符串复制
来源：http://hz.hywenlv.cn/gtwvsodfts.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinqigufen.top/gtisephyhx.html

[S05] C：字符串长度
来源：http://hz.yuxming.cn/gtaxqctqjm.html

strlen(s)
来源：http://hz.zhongyouzk.top/gtfrvuidxl.html

[S06] C：字符串比较
来源：http://hz.yueranfly.top/gtrmgajdhx.html

strcmp(a, b) == 0
来源：http://hz.hfpthk.cn/gtfaxhkkic.html

[S07] C：数组遍历求和
来源：http://hz.xuanzx.com/gtdjsqqwmv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xuetiantiany.cn/gtmnzejrhe.html

[S08] C：动态内存分配与释放
来源：http://hz.yvedp.cn/gtnlffgpkg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yuxming.cn/gtctoikztv.html

[S09] C：结构体定义与初始化
来源：http://hz.hfpthk.cn/gtucdidulu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gaohongyu789.top/gtfdlcbiai.html

[S10] C：指针与解引用
来源：http://hz.kuanghao11.cn/gtmxeejiqw.html

int *p = &a;  *p = 5;
来源：http://hz.svipenyu.cn/gtehyyucqh.html

[S11] C：逐行读文件
来源：http://hz.guowangkeji.top/gtiwkrzerz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.chenzaomai.com/gtkvzakcvr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shuidangran.top/gtxxtbnaje.html

fclose(f);
来源：http://hz.shuidangran.top/gttqhagnfp.html

[S12] C：写文件
来源：http://hz.zhijiandao.cn/gtddrphzrj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xuanzx.com/gtlxwbdche.html

[S13] C：宏定义
来源：http://hz.hammf.cn/gttlvkntlh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cheryme.top/gthyvhrlsk.html

[S14] C：枚举
来源：http://hz.quarkkingdee.top/gtuszxiesf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.kuanghao11.cn/gtqbyaothn.html

[S15] C：类型转换
来源：http://hz.mhx1999.top/gtltmoacde.html

(double) a / b
来源：http://hz.52xcode.cn/gtjghcvijp.html

[S16] C：位操作置位
来源：http://hz.bjfxy.top/gtmoenmwpg.html

x |= (1 << 3);
来源：http://hz.hnqzz.top/gtuxfrvzpg.html

[S17] C：安全拼接字符串
来源：http://hz.yj202588.top/gthhbpwbxb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cashguo.top/gtirqhbiiu.html

[S18] C：命令行参数
来源：http://hz.pengpengdd.cyou/gtthkzqaig.html

int main(int argc, char **argv)
来源：http://hz.ydjk.org.cn/gtomuggpwa.html

[S19] C：快速排序
来源：http://hz.feifeiyinyue.top/gtvqyjeqli.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.0kj1m.cn/gtdvhsocpt.html

[S20] C：二分查找
来源：http://hz.xuanzx.com/gtsrajucdr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.guowangkeji.top/gtcazaaoeu.html

[S21] C：字符类别判断
来源：http://hz.quarkkingdee.top/gtiupeqpvi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.svipenyu.cn/gtspbxggva.html

[S22] C：字符串转数字
来源：http://hz.zhixingplan.top/gtyvptyjsk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jianghu66.top/gtyofkeubz.html

[S23] C：随机数
来源：http://hz.c1oappe.top/gtkofwijvd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinyuanbaomall.cn/gtngaobfiz.html

[S24] C：获取本地时间
来源：http://hz.zhengqikj.top/gtgecqxzly.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xuanzx.com/gtlikznver.html

[S25] C：内存拷贝
来源：http://hz.0kj1m.cn/gtvzikxndo.html

memcpy(dst, src, n);
来源：http://hz.svipenyu.cn/gtujdspufb.html

[S26] C：内存清零
来源：http://hz.svipenyu.cn/gteocpyrpt.html

memset(a, 0, sizeof a);
来源：http://hz.fengsongda.top/gtzcqhpyry.html

[S27] C：定义常量
来源：http://hz.yuxming.cn/gtsjlnjtfl.html

const double PI = 3.14159;
来源：http://hz.jinqigfzy.top/gtbiugzxdv.html

[S28] C：静态变量
来源：http://hz.jqgufenzy.top/gtcikwjydh.html

static int counter = 0;
来源：http://hz.shanyushiyangtech.top/gtvrnhvedq.html

[S29] C：变参函数
来源：http://hz.ehwqpu.com/gtiyuctekf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.pengpengdd.cyou/gtjhgkclnn.html

[S30] C：头文件保护
来源：http://hz.birdmap.top/gtszuxuyee.html

#ifndef X_H
来源：http://hz.ivvv.top/gtlvdtshlz.html

#define X_H
来源：http://hz.zhoulong.xyz/gtpppkztrl.html

#endif
来源：http://hz.jinyuanbaomall.cn/gtqpkayodl.html

[S31] C++：Hello World
来源：http://hz.jlsjyb.cn/gtpxzxemnd.html

#include <iostream>
来源：http://hz.dianchejie.cn/gtbwncrwld.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.sysykeji.top/gtulrzfwwk.html

[S32] C++：字符串
来源：http://hz.sweek.top/gthidkpzvn.html

std::string s = "hi";  s += "!";
来源：http://hz.daria6918.cn/gtmonsbhiz.html

[S33] C++：vector 增删
来源：http://hz.fzhhl.top/gtpxgdtvsi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.fzhhl.top/gtwqqbqodp.html

[S34] C++：遍历 vector
来源：http://hz.guannengcc.top/gtsmdcusuw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.tianlin.xyz/gtdsycurxi.html

[S35] C++：map
来源：http://hz.vqdsnc.cn/gtfszdydnp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.birdmap.top/gtjcicawnx.html

[S36] C++：unordered_map
来源：http://hz.snrcjt.cn/gtdzivcogk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnxiangtu.top/gtfolwavue.html

[S37] C++：set
来源：http://hz.hongshengwenyu.top/gtqeriksiq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.9152youxi.cn/gtkoilukiz.html

[S38] C++：排序
来源：http://hz.jqgfzy.top/gtnbltpsyl.html

std::sort(v.begin(), v.end());
来源：http://hz.yuanzhike.top/gtlsztcekb.html

[S39] C++：自定义比较器排序
来源：http://hz.jqgfzy.top/gtxcyabxcq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj20258.top/gtniwmahdd.html

[S40] C++：查找元素
来源：http://hz.ppjwa.cn/gtpjmfbtyb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zdqjudy.top/gtvsbiacmg.html

[S41] C++：类与构造函数
来源：http://hz.nwbrower.top/gtasrgdnpa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.chenjidiqi.icu/gtsdreikpv.html

[S42] C++：继承与虚函数
来源：http://hz.ywan-chungtsiang.top/gtwylbjzhp.html

class B : public Base { public: void f() override {} };
来源：http://hz.shangyingyoupin.top/gtqbylldrt.html

[S43] C++：智能指针
来源：http://hz.aibaodan.cn/gtcuvwohgx.html

auto p = std::make_unique<int>(5);
来源：http://hz.shangyingyoupin.top/gtszbrjydo.html

[S44] C++：引用传参
来源：http://hz.yj20258.top/gtkbirdvbx.html

void inc(int &x) { ++x; }
来源：http://hz.jiagoushi.top/gtzcrgzeld.html

[S45] C++：lambda
来源：http://hz.ehwqpu.com/gtyeuraack.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhengqikj.top/gtwotwppep.html

[S46] C++：函数模板
来源：http://hz.zhijiandao.cn/gteimxjyuj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhiwuduotai.top/gtodcpsrzr.html

[S47] C++：结构化绑定遍历
来源：http://hz.tian-w.cn/gtekthbtbl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhaomingkeji.xyz/gtxknzhekw.html

[S48] C++：逐行读文件
来源：http://hz.shanyushiyangkeji.top/gtanttgzlt.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tanke756.top/gtcxwvlxva.html

while (std::getline(in, line)) { }
来源：http://hz.pycfn.com/gtlfqfzwdy.html

[S49] C++：写文件
来源：http://hz.nanxinkj.top/gtcspjwqwr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hysaishi.cn/gtnuioswnh.html

[S50] C++：格式化数字
来源：http://hz.ivvv.top/gtkcslprmr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shuidangran.top/gtxfwewtow.html

[S51] C++：显式类型转换
来源：http://hz.yvedp.cn/gthabpqjws.html

static_cast<double>(a) / b
来源：http://hz.wangshuangyany.cn/gtfzaaadze.html

[S52] C++：const 与 noexcept
来源：http://hz.havefunace.top/gtirkxfrmj.html

int size() const noexcept { return n_; }
来源：http://hz.hywenlv.cn/gtogfptaxl.html

[S53] C++：移动语义
来源：http://hz.hongshengwenyu.top/gtnpysugwx.html

std::vector<int> w = std::move(v);
来源：http://hz.xylfe.cn/gtmrntmchx.html

[S54] C++：异常处理
来源：http://hz.smart0.xyz/gtokgauzsx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.svipenyu.cn/gthblkuind.html

[S55] C++：结构化绑定
来源：http://hz.jqgfzy.top/gtwxubcjrd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhijiandao.cn/gtmevczlkc.html

[S56] C++：optional
来源：http://hz.xylfe.cn/gtnzuisphg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhixingplan.top/gtavsfyhuo.html

[S57] C++：编译期常量
来源：http://hz.ppjwa.cn/gtcknvfvpj.html

constexpr int N = 10;
来源：http://hz.iojbl.cn/gtomrawvbc.html

[S58] C++：命名空间
来源：http://hz.xylfe.cn/gtaauxpskn.html

namespace ns { int f() { return 1; } }
来源：http://hz.316326.xyz/gtznfdtcre.html

[S59] C++：静态断言
来源：http://hz.zhoulong.xyz/gtfavlefxo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shangyingyoupin.top/gtgepbjiqs.html

[S60] C++：遍历并删除元素
来源：http://hz.andypj.xyz/gtdmmpyiny.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.aibaodan.cn/gtmtwarcff.html

================================================================================
来源：http://hz.yuxming.cn/gtfvivfkfx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yvedp.cn/gtkzxqlgpj.html

================================================================================
来源：http://hz.yj20258888.top/gtbdobjzvd.html

[T01] Kotlin：Hello World
来源：http://hz.jinyuanbaomall.cn/gtkyyiagyg.html

println("Hello")
来源：http://hz.hnqzz.top/gtuorguffq.html

[T02] Kotlin：变量
来源：http://hz.zhoulong.xyz/gtmxzqmpya.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhaomingkeji.xyz/gtfumxmqef.html

[T03] Kotlin：字符串模板
来源：http://hz.jianghu66.top/gtzqlrwgqo.html

"值: $b"
来源：http://hz.tian-w.cn/gtnwyhddqh.html

[T04] Kotlin：空安全
来源：http://hz.andypj.xyz/gtrqdhynqf.html

val n: String? = null;  n?.length
来源：http://hz.sxryk.cn/gtwzxicdyj.html

[T05] Kotlin：when 表达式
来源：http://hz.jlsjyb.cn/gtqwitjyxc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.bjfxy.top/gtqkvbkeeo.html

[T06] Kotlin：集合映射
来源：http://hz.shanyushiyangtech.top/gtesuwyyte.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.guowangkeji.top/gttksmlfia.html

[T07] Kotlin：集合过滤
来源：http://hz.fzhhl.top/gtqnddgvto.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shangyingyoupin.top/gtlbbafqfz.html

[T08] Kotlin：数据类
来源：http://hz.hnqzz.top/gtuhujikby.html

data class User(val name: String, val age: Int)
来源：http://hz.sysykeji.top/gtjzlplqgt.html

[T09] Kotlin：扩展函数
来源：http://hz.tian-w.cn/gtkaikhvlw.html

fun String.exclaim() = this + "!"
来源：http://hz.tanke756.top/gtjmchfulj.html

[T10] Kotlin：默认参数
来源：http://hz.jiagoushi.top/gtjelwqrer.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.sufxvd.cn/gtksvppant.html

[T11] Kotlin：协程
来源：http://hz.yanxiufei.cn/gtevpqjnrj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ehwqpu.com/gtgsrfijzl.html

[T12] Kotlin：解构声明
来源：http://hz.yj20258888.top/gtiordwsxt.html

val (a, b) = Pair(1, 2)
来源：http://hz.fzhhl.top/gtjvwwplvx.html

[T13] Kotlin：只读 Map
来源：http://hz.zhixingplan.top/gtktwhtras.html

val m = mapOf("a" to 1)
来源：http://hz.jiagoushi.top/gtaevpehxj.html

[T14] Kotlin：循环
来源：http://hz.yanxiufei.cn/gtgbdazaad.html

for (i in 1..10) println(i)
来源：http://hz.jinqigufen.top/gtdfgxjuxy.html

[T15] Kotlin：接口
来源：http://hz.yuanzhike.top/gtccqjyhnd.html

interface Shape { fun area(): Double }
来源：http://hz.ppjwa.cn/gtkxnxfaep.html

[T16] Swift：Hello World
来源：http://hz.yongpay.top/gtiicfadjs.html

print("Hello")
来源：http://hz.hywenlv.cn/gthttdgjtu.html

[T17] Swift：变量与常量
来源：http://hz.ywan-chungtsiang.top/gttwwybibg.html

var a = 1;  let b = 2
来源：http://hz.svipenyu.cn/gteixstfyq.html

[T18] Swift：字符串插值
来源：http://hz.shangyingyoupin.top/gtkxhwfyct.html

"值: \(b)"
来源：http://hz.yj20258888.top/gtlykqcrvt.html

[T19] Swift：可选绑定
来源：http://hz.c1oappe.top/gtsiqlzhxa.html

if let n = opt { print(n) }
来源：http://hz.c1oappe.top/gtzwfjsjea.html

[T20] Swift：数组操作
来源：http://hz.9152youxi.cn/gtdbfrnwwz.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hnxiangtu.top/gtmlnvhysf.html

[T21] Swift：遍历
来源：http://hz.haohaochexian.top/gtalwueevt.html

for x in a { print(x) }
来源：http://hz.jinghuilouyu.cn/gtrfwrmcnc.html

[T22] Swift：字典
来源：http://hz.snrcjt.cn/gtffhomocb.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.xylfe.cn/gtgntcyblf.html

[T23] Swift：函数
来源：http://hz.yj20258888.top/gthewfvqpp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhengqikj.top/gtuuyhwkec.html

[T24] Swift：闭包
来源：http://hz.zhixingplan.top/gtqqwdjsya.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.chenjidiqi.icu/gtnrqzwrar.html

[T25] Swift：结构体
来源：http://hz.iojbl.cn/gttatwlitf.html

struct P { var x: Int }
来源：http://hz.gzhubu.top/gtljcnwrei.html

[T26] Swift：类与重写
来源：http://hz.iojbl.cn/gtvlunxcqz.html

class A: Base { override func f() {} }
来源：http://hz.daria6918.cn/gttirgfpuh.html

[T27] Swift：错误处理
来源：http://hz.sxryk.cn/gtkjkojwfq.html

do { try f() } catch { print(error) }
来源：http://hz.ehwqpu.com/gtnltgkjck.html

[T28] Swift：枚举
来源：http://hz.nanxinkj.top/gtxenehsns.html

enum Color { case red, green }
来源：http://hz.xingfuxueyuan.xyz/gtbkbhmewq.html

[T29] Swift：guard 提前返回
来源：http://hz.haohaochexian.top/gtriycitrm.html

guard let x = opt else { return }
来源：http://hz.kuanghao11.cn/gtqdoktbgi.html

[T30] Swift：协议
来源：http://hz.yuxming.cn/gthhyqozpw.html

protocol Shape { func area() -> Double }
来源：http://hz.pycfn.com/gtiqrdsndx.html

[T31] Lua：Hello World
来源：http://hz.chenlongwang.top/gtqzrznzls.html

print("Hello")
来源：http://hz.jinyuanbaomall.cn/gtfbkgjkgb.html

[T32] Lua：局部变量
来源：http://hz.fzhhl.top/gtwgevaomk.html

local a = 1
来源：http://hz.gotoacloud.top/gtqwyhscqp.html

[T33] Lua：表（数组）
来源：http://hz.tanke756.top/gtwqintreo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xuanzx.com/gtvccxqcqg.html

[T34] Lua：遍历表
来源：http://hz.jlsjyb.cn/gtcablllfj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yangfankeji.com/gtsxmkpnxr.html

[T35] Lua：字典表
来源：http://hz.meibo888.top/gtykmselws.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yuanzhike.top/gtbdrwotrd.html

[T36] Lua：函数
来源：http://hz.zhaomingkeji.xyz/gtogxfjcri.html

function add(a, b) return a + b end
来源：http://hz.jyoumei.cn/gtkzqqeizb.html

[T37] Lua：字符串拼接
来源：http://hz.daxiang520.top/gtfsehdywl.html

"a" .. "b"
来源：http://hz.jlsjyb.cn/gtyoheqwsd.html

[T38] Lua：条件
来源：http://hz.xinyue.icu/gtploulznq.html

if x > 0 then print("正") end
来源：http://hz.9152youxi.cn/gtxblrwdmk.html

[T39] Lua：模式匹配
来源：http://hz.xziqi.cn/gtjhrbxoqn.html

string.find(s, "%d+")
来源：http://hz.zhoulong.xyz/gtuflgdqti.html

[T40] Lua：元表
来源：http://hz.cheryme.top/gtvuvbqubp.html

setmetatable({}, { __index = base })
来源：http://hz.nanxuanxn.top/gthrfaflnc.html

[T41] Perl：Hello World
来源：http://hz.0kj1m.cn/gtmoxpsckm.html

print "Hello\n";
来源：http://hz.hongshengwenyu.top/gtacaddpmo.html

[T42] Perl：变量类型
来源：http://hz.gotoacloud.top/gtutwapluk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.nanxinkj.top/gtqjmdeewy.html

[T43] Perl：字符串插值
来源：http://hz.kuanghao11.cn/gtknvaelft.html

"值: $a"
来源：http://hz.jiagoushi.top/gtpqozeniy.html

[T44] Perl：条件
来源：http://hz.jqgfzy.top/gtquqvsgxb.html

if ($a > 0) { print "正"; }
来源：http://hz.yvedp.cn/gtsugbiczt.html

[T45] Perl：数组遍历
来源：http://hz.shanyushiyangtech.top/gthaskwnzs.html

for my $x (@arr) { print $x; }
来源：http://hz.meibo888.top/gtdbwagcxh.html

[T46] Perl：哈希操作
来源：http://hz.guannengcc.top/gtsarotjhd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yj20258888.top/gtsbhrzpbl.html

[T47] Perl：正则捕获
来源：http://hz.yueranfly.top/gtluqcekoz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.mhx1999.top/gtszoozsxs.html

[T48] Perl：正则替换
来源：http://hz.guannengcc.top/gttvhgtkqc.html

$s =~ s/old/new/g;
来源：http://hz.jiagoushi.top/gtzfglflkp.html

[T49] Perl：函数
来源：http://hz.zhoulong.xyz/gtgnatebik.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.daria6918.cn/gtysmiurwa.html

[T50] Perl：逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtlccvwcmc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.quarkkingdee.top/gthlziohnl.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jyoumei.cn/gtiuqlxmfm.html

[T51] Scala：Hello World
来源：http://hz.shuidangran.top/gtxgbdkvub.html

println("Hello")
来源：http://hz.yvedp.cn/gtsoksoeom.html

[T52] Scala：变量
来源：http://hz.dianchejie.cn/gtuqqgpcbq.html

val a = 1;  var b = 2
来源：http://hz.havefunace.top/gtasrnqyyr.html

[T53] Scala：字符串插值
来源：http://hz.redwolf501.top/gtwfacpaed.html

s"值: $b"
来源：http://hz.yonumen.top/gtgwbkkkoz.html

[T54] Scala：集合映射
来源：http://hz.shuidangran.top/gtdddarbrs.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yj20258.top/gtguqkrrio.html

[T55] Scala：集合过滤
来源：http://hz.aibaodan.cn/gtbjwfdeot.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hfpthk.cn/gtifbysbms.html

[T56] Scala：样例类
来源：http://hz.ybcxt.top/gtzokiudbh.html

case class User(name: String, age: Int)
来源：http://hz.tian-w.cn/gtrzzudxxa.html

[T57] Scala：模式匹配
来源：http://hz.zhoulong.xyz/gtinnhtdan.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.fengsongda.top/gtkzmdylnt.html

[T58] Scala：函数定义
来源：http://hz.52xcode.cn/gtstfwydip.html


<!-- 参考信息 -->