代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhiwuduotai.top/gtvnaoyuth.html

[R54] 比较两个文件
来源：http://hz.yongpay.top/gtuowqbrix.html

diff a.txt b.txt
来源：http://hz.aizwys.cn/gtraoixsfe.html

[R55] 压缩与解压
来源：http://hz.mhx1999.top/gtpzfovcmd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhengqikj.top/gtbrgazvup.html

[R56] 远程拷贝
来源：http://hz.yuanzhike.top/gturnysmwm.html

scp file user@host:/path/
来源：http://hz.shuidangran.top/gttptshloq.html

[R57] 远程执行命令
来源：http://hz.yangfankeji.com/gthqvgisms.html

ssh user@host 'uptime'
来源：http://hz.sufxvd.cn/gtmlmwztym.html

[R58] 下载文件
来源：http://hz.ppjwa.cn/gteznztuae.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.tianlin.xyz/gtnefxrgij.html

[R59] 发 POST JSON
来源：http://hz.sufxvd.cn/gtpgjsewcr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shanyushiyangtech.top/gthodxbenk.html

[R60] 只看 HTTP 状态码
来源：http://hz.bjfxy.top/gtsysdcgms.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhixingplan.top/gtcfqehvcu.html

[R61] 磁盘占用
来源：http://hz.jqgfzy.top/gtxhjdiypz.html

df -h;  du -sh *
来源：http://hz.zhoulong.xyz/gtmavjraba.html

[R62] 找最占空间的文件
来源：http://hz.zhixingplan.top/gtaqibcvpq.html

du -ah . | sort -rh | head -10
来源：http://hz.vqdsnc.cn/gtapyofwkq.html

[R63] 内存与进程
来源：http://hz.yj20258.top/gtexhfiesg.html

free -h;  ps aux | grep nginx
来源：http://hz.guowangkeji.top/gtperoexsb.html

[R64] 结束进程
来源：http://hz.ydzc1.top/gtccliivsf.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yj20258888.top/gtvatstmuv.html

[R65] 查看端口占用
来源：http://hz.snrcjt.cn/gtrzytkinq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yvedp.cn/gtuwbtllei.html

[R66] 定时任务
来源：http://hz.ywan-chungtsiang.top/gtcqqfeavo.html

crontab -e;  crontab -l
来源：http://hz.hnqzz.top/gtjujdsced.html

[R67] 生成随机十六进制串
来源：http://hz.yuxming.cn/gtkqsqumca.html

openssl rand -hex 16
来源：http://hz.aizwys.cn/gtrvbvsqea.html

[R68] 计算文件校验值
来源：http://hz.yj20258.top/gtobapezhe.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.dianchejie.cn/gtebpijicq.html

[R69] 生成随机密码
来源：http://hz.pycfn.com/gtnxzhfbrw.html

head -c 16 /dev/urandom | base64
来源：http://hz.wangshuangyany.cn/gtketjdykh.html

[R70] 时间戳与互转
来源：http://hz.hywenlv.cn/gtkjsqatuq.html

date +%s;  date -d @1700000000
来源：http://hz.jqgfzy.top/gtdcabsitd.html

[R71] 日期格式化
来源：http://hz.wangdashe.top/gtfydyprar.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xuetiantiany.cn/gtwkhulxre.html

[R72] 等待端口就绪
来源：http://hz.haohaochexian.top/gtoapgjjjc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yongpay.top/gtfzhqfprh.html

[R73] 分割大日志
来源：http://hz.iojbl.cn/gtvakrmbkj.html

split -l 1000 big.log part_
来源：http://hz.chenjidiqi.icu/gtolcfbukn.html

[R74] 批量重命名
来源：http://hz.yvedp.cn/gtfclzakzj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.guannengcc.top/gtdkprljet.html

[R75] 导出环境变量
来源：http://hz.wangdashe.top/gtbgtqywvr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.redwolf501.top/gtqihkmwbz.html

[R76] 使用临时文件
来源：http://hz.iojbl.cn/gtbekecwal.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.feifeiyinyue.top/gtolgsusbe.html

[R77] 读取用户输入
来源：http://hz.iojbl.cn/gtdhlgaygu.html

read -rp "请输入: " ans
来源：http://hz.havefunace.top/gtytmimrsa.html

[R78] 交互式菜单
来源：http://hz.jinqigfzy.top/gtmnfbsebj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sufxvd.cn/gtiaxmsjel.html

[R79] 解析命令行选项
来源：http://hz.tian-w.cn/gtvrkbeeku.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.wangshuangyany.cn/gtwegkpoow.html

[R80] 查看脚本执行耗时
来源：http://hz.cdnleiting.top/gtuazkapbz.html

time ./run.sh
来源：http://hz.hywenlv.cn/gtyrttlzzw.html

================================================================================
来源：http://hz.ybcxt.top/gtfwqzqcol.html

S. C / C++ 专题
来源：http://hz.yuanzhike.top/gtubditady.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtbowtzpzq.html

[S01] C：Hello World
来源：http://hz.ivvv.top/gtarwwwdre.html

#include <stdio.h>
来源：http://hz.guannengcc.top/gtribidgjb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shuidangran.top/gtjumdijpx.html

[S02] C：变量与格式化输出
来源：http://hz.yangfankeji.com/gtghayuyko.html

int a = 10; printf("%d\n", a);
来源：http://hz.hfpthk.cn/gtqlranuci.html

[S03] C：读入整数
来源：http://hz.xylfe.cn/gtukwtejmo.html

int x; scanf("%d", &x);
来源：http://hz.mhx1999.top/gtkfowejyd.html

[S04] C：字符串复制
来源：http://hz.jinqigfzy.top/gtclkqwide.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hongshengwenyu.top/gtyhkulahh.html

[S05] C：字符串长度
来源：http://hz.hnxiangtu.top/gtaflawtgt.html

strlen(s)
来源：http://hz.wangshuangyany.cn/gtsegzwnty.html

[S06] C：字符串比较
来源：http://hz.jinyuanbaomall.cn/gtjxlutbfl.html

strcmp(a, b) == 0
来源：http://hz.sxryk.cn/gtpdljmbjj.html

[S07] C：数组遍历求和
来源：http://hz.shzxlz.cn/gtweaxrwpf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gzhubu.top/gtypqwabhm.html

[S08] C：动态内存分配与释放
来源：http://hz.guannengcc.top/gtplzggyoi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yj20258.top/gtstlindya.html

[S09] C：结构体定义与初始化
来源：http://hz.xuanzx.com/gtmjzphybj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zdqjudy.top/gtrlnmrvpj.html

[S10] C：指针与解引用
来源：http://hz.fzhhl.top/gtfdymdtyk.html

int *p = &a;  *p = 5;
来源：http://hz.sysykeji.top/gtkfzcicoh.html

[S11] C：逐行读文件
来源：http://hz.hfpthk.cn/gtpteuqwdr.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yj202588.top/gtyjeczbtw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.sysykeji.top/gtniuucnep.html

fclose(f);
来源：http://hz.yongpay.top/gtoqdfnuwx.html

[S12] C：写文件
来源：http://hz.tanke756.top/gtmaxcmkvx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ydzc1.top/gtvgxwxuxl.html

[S13] C：宏定义
来源：http://hz.jianghu66.top/gtewamgjyk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ehwqpu.com/gtgumszjdy.html

[S14] C：枚举
来源：http://hz.zhixingplan.top/gtxgqraxzc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.chenlongwang.top/gtlnypwszb.html

[S15] C：类型转换
来源：http://hz.316326.xyz/gtnlsumeuu.html

(double) a / b
来源：http://hz.hysaishi.cn/gtoomkinlu.html

[S16] C：位操作置位
来源：http://hz.9152youxi.cn/gtzeslrxch.html

x |= (1 << 3);
来源：http://hz.jinghuilouyu.cn/gtiswikxgc.html

[S17] C：安全拼接字符串
来源：http://hz.chenzaomai.com/gtggrmieox.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.pengpengdd.cyou/gtwvmvjktk.html

[S18] C：命令行参数
来源：http://hz.mhx1999.top/gtrynshdkx.html

int main(int argc, char **argv)
来源：http://hz.daria6918.cn/gtjvcefwjb.html

[S19] C：快速排序
来源：http://hz.ydzc1.top/gtjswhbwfp.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.gogol.net.cn/gtsclyrkxs.html

[S20] C：二分查找
来源：http://hz.wangdashe.top/gtamlcmsfr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhijiandao.cn/gtntzmndga.html

[S21] C：字符类别判断
来源：http://hz.wangshuangyany.cn/gtwpjdiamf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.daxiang520.top/gtewlwzikz.html

[S22] C：字符串转数字
来源：http://hz.redwolf501.top/gtwpfptzec.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.vqdsnc.cn/gtngfmpecp.html

[S23] C：随机数
来源：http://hz.yj20258.top/gtuejsmyez.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.nwbrower.top/gtoujjlzlp.html

[S24] C：获取本地时间
来源：http://hz.gaohongyu789.top/gtxfobhmxj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhixingplan.top/gtxsnugcvg.html

[S25] C：内存拷贝
来源：http://hz.nanxinkj.top/gtxtgzcdny.html

memcpy(dst, src, n);
来源：http://hz.gogol.net.cn/gtvprrjoww.html

[S26] C：内存清零
来源：http://hz.aibaodan.cn/gtyrucmovh.html

memset(a, 0, sizeof a);
来源：http://hz.zhengqikj.top/gtnunmxura.html

[S27] C：定义常量
来源：http://hz.yanxiufei.cn/gtfagmidme.html

const double PI = 3.14159;
来源：http://hz.birdmap.top/gtphppkiwz.html

[S28] C：静态变量
来源：http://hz.daxiang520.top/gtqphaknyy.html

static int counter = 0;
来源：http://hz.pengpengdd.cyou/gthnnkujlv.html

[S29] C：变参函数
来源：http://hz.wangdashe.top/gtnxzjbvvv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.tianlin.xyz/gtewzueosi.html

[S30] C：头文件保护
来源：http://hz.zhoulong.xyz/gttyhxzedq.html

#ifndef X_H
来源：http://hz.tanke756.top/gtxtaxghmr.html

#define X_H
来源：http://hz.nwbrower.top/gtjvpftpak.html

#endif
来源：http://hz.jianghu66.top/gtrliuztvu.html

[S31] C++：Hello World
来源：http://hz.chenjidiqi.icu/gtuplljnad.html

#include <iostream>
来源：http://hz.iojbl.cn/gtcpsagnzm.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jinghuilouyu.cn/gtmtihphmy.html

[S32] C++：字符串
来源：http://hz.jlsjyb.cn/gtiohzhywz.html

std::string s = "hi";  s += "!";
来源：http://hz.jqgufenzy.top/gtrbdoxsfy.html

[S33] C++：vector 增删
来源：http://hz.svipenyu.cn/gtsinkhaui.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yj20258.top/gttidnlniq.html

[S34] C++：遍历 vector
来源：http://hz.fengsongda.top/gtyhbzggyz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.daria6918.cn/gtclcilwmi.html

[S35] C++：map
来源：http://hz.mhx1999.top/gtrksmymnd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gtkwdlftxu.html

[S36] C++：unordered_map
来源：http://hz.yueranfly.top/gtgusqauhg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.316326.xyz/gtphzkpqfm.html

[S37] C++：set
来源：http://hz.yangfankeji.com/gtlfkhtqyw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shanyushiyangkeji.top/gthvyjsyzt.html

[S38] C++：排序
来源：http://hz.xuanzx.com/gtpvsplphp.html

std::sort(v.begin(), v.end());
来源：http://hz.zdqjudy.top/gtudxrmgmj.html

[S39] C++：自定义比较器排序
来源：http://hz.ydzc1.top/gtqzhflgir.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ydjk.org.cn/gtdyrgmlqn.html

[S40] C++：查找元素
来源：http://hz.wangdashe.top/gtlcfpbxvm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.tianlin.xyz/gtxfvhydkw.html

[S41] C++：类与构造函数
来源：http://hz.hywenlv.cn/gtuybxcukc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.c1oappe.top/gtgreuvuyg.html

[S42] C++：继承与虚函数
来源：http://hz.zhiwuduotai.top/gtykonassd.html

class B : public Base { public: void f() override {} };
来源：http://hz.ydzc1.top/gtuthlvonw.html

[S43] C++：智能指针
来源：http://hz.9152youxi.cn/gtouqoigfk.html

auto p = std::make_unique<int>(5);
来源：http://hz.cheryme.top/gtbsypwmie.html

[S44] C++：引用传参
来源：http://hz.zhaomingkeji.xyz/gthupijrjm.html

void inc(int &x) { ++x; }
来源：http://hz.redwolf501.top/gtleitgnlb.html

[S45] C++：lambda
来源：http://hz.zdqjudy.top/gtnsbuqhxz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.wangshuangyany.cn/gtvzjklwec.html

[S46] C++：函数模板
来源：http://hz.yj20258.top/gtfbzuofex.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.tian-w.cn/gteodyvrox.html

[S47] C++：结构化绑定遍历
来源：http://hz.yvedp.cn/gtscqitgrt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.aibaodan.cn/gtxfdpotfh.html

[S48] C++：逐行读文件
来源：http://hz.yj20258888.top/gtdlvgjxey.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yanxiufei.cn/gtuzqwzsav.html

while (std::getline(in, line)) { }
来源：http://hz.ivvv.top/gttnkjipxf.html

[S49] C++：写文件
来源：http://hz.pengpengdd.cyou/gtlmnuxdab.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.birdmap.top/gtzticetna.html

[S50] C++：格式化数字
来源：http://hz.wangshuangyany.cn/gtvuzwfhxu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xziqi.cn/gtnmflasia.html

[S51] C++：显式类型转换
来源：http://hz.zhaomingkeji.xyz/gtwvgwlzdr.html

static_cast<double>(a) / b
来源：http://hz.gzhubu.top/gtfwgmhheg.html

[S52] C++：const 与 noexcept
来源：http://hz.xziqi.cn/gtimoztevv.html

int size() const noexcept { return n_; }
来源：http://hz.jinyuanbaomall.cn/gttchoorye.html

[S53] C++：移动语义
来源：http://hz.hnxiangtu.top/gtzkefszbs.html

std::vector<int> w = std::move(v);
来源：http://hz.yj20258.top/gtfwgsavly.html

[S54] C++：异常处理
来源：http://hz.daxiang520.top/gtynnxlxxu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinqigfzy.top/gtftfynwou.html

[S55] C++：结构化绑定
来源：http://hz.ywan-chungtsiang.top/gtoqdsfhal.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhengqikj.top/gtomonwjkt.html

[S56] C++：optional
来源：http://hz.zhixingplan.top/gtpholctnq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cucudq.cn/gtrmygtgxw.html

[S57] C++：编译期常量
来源：http://hz.tanke756.top/gthnggwlvo.html

constexpr int N = 10;
来源：http://hz.hongshengwenyu.top/gtlxvgoadu.html

[S58] C++：命名空间
来源：http://hz.xingfuxueyuan.xyz/gtzwmzoxci.html

namespace ns { int f() { return 1; } }
来源：http://hz.wangdashe.top/gtyaciirdb.html

[S59] C++：静态断言
来源：http://hz.jlsjyb.cn/gtsscxcyjr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.gotoacloud.top/gtvltzsssj.html

[S60] C++：遍历并删除元素
来源：http://hz.yuxming.cn/gtwiiqnatv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gaohongyu789.top/gtfgabzagj.html

================================================================================
来源：http://hz.shuidangran.top/gtzalyiclw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xuanzx.com/gtjhxgmnxq.html

================================================================================
来源：http://hz.jqgufenzy.top/gtpwvahiqy.html

[T01] Kotlin：Hello World
来源：http://hz.cucudq.cn/gtnmdcpfbk.html

println("Hello")
来源：http://hz.tian-w.cn/gttkodwnpv.html

[T02] Kotlin：变量
来源：http://hz.vqdsnc.cn/gtfrjpkcfu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yj20258.top/gtfjkpfebm.html

[T03] Kotlin：字符串模板
来源：http://hz.hfpthk.cn/gtvchaivfa.html

"值: $b"
来源：http://hz.nanxinkj.top/gtaiawhowq.html

[T04] Kotlin：空安全
来源：http://hz.yueranfly.top/gtminukedp.html

val n: String? = null;  n?.length
来源：http://hz.dianchejie.cn/gtshfcnihh.html

[T05] Kotlin：when 表达式
来源：http://hz.jlsjyb.cn/gtlvpowgep.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xylfe.cn/gtqyffletk.html

[T06] Kotlin：集合映射
来源：http://hz.smart0.xyz/gtwxidgafb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zycfv.cn/gtyogwbqqx.html

[T07] Kotlin：集合过滤
来源：http://hz.c1oappe.top/gtpeurtaun.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.sufxvd.cn/gtjikzwsyl.html

[T08] Kotlin：数据类
来源：http://hz.dianchejie.cn/gtjcqpixpu.html

data class User(val name: String, val age: Int)
来源：http://hz.tianlin.xyz/gtpyarpebe.html

[T09] Kotlin：扩展函数
来源：http://hz.zhoulong.xyz/gtcitridcf.html

fun String.exclaim() = this + "!"
来源：http://hz.hfpthk.cn/gtjhnyeltq.html

[T10] Kotlin：默认参数
来源：http://hz.tianlin.xyz/gtjlueqhxy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.redwolf501.top/gtttkuxkzp.html

[T11] Kotlin：协程
来源：http://hz.guowangkeji.top/gtpubywdom.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.dianchejie.cn/gtlhaeaujg.html

[T12] Kotlin：解构声明
来源：http://hz.yuxming.cn/gtyouxcrgu.html

val (a, b) = Pair(1, 2)
来源：http://hz.gogol.net.cn/gtvulmtlqj.html

[T13] Kotlin：只读 Map
来源：http://hz.tianlin.xyz/gtwklfvnio.html

val m = mapOf("a" to 1)
来源：http://hz.svipenyu.cn/gtsnouhnfb.html

[T14] Kotlin：循环
来源：http://hz.chenjidiqi.icu/gtgdoyiysq.html

for (i in 1..10) println(i)
来源：http://hz.daria6918.cn/gtaxomxakq.html

[T15] Kotlin：接口
来源：http://hz.shuidangran.top/gtmgxwyjer.html

interface Shape { fun area(): Double }
来源：http://hz.cucudq.cn/gtvyzoeman.html

[T16] Swift：Hello World
来源：http://hz.xylfe.cn/gtphcpvgyl.html

print("Hello")
来源：http://hz.guowangkeji.top/gtutzlszar.html

[T17] Swift：变量与常量
来源：http://hz.xuanzx.com/gtuyiarsay.html

var a = 1;  let b = 2
来源：http://hz.vqdsnc.cn/gtxuhgdkkw.html

[T18] Swift：字符串插值
来源：http://hz.sysykeji.top/gthzdiierr.html

"值: \(b)"
来源：http://hz.guannengcc.top/gtbryenbpy.html

[T19] Swift：可选绑定
来源：http://hz.xinyue.icu/gthtoekivc.html

if let n = opt { print(n) }
来源：http://hz.guowangkeji.top/gtnfualuzc.html

[T20] Swift：数组操作
来源：http://hz.zycfv.cn/gtzssxwvgk.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.snrcjt.cn/gtuxfffxtb.html

[T21] Swift：遍历
来源：http://hz.316326.xyz/gtneponbax.html

for x in a { print(x) }
来源：http://hz.ivvv.top/gtzqirnafe.html

[T22] Swift：字典
来源：http://hz.sxryk.cn/gtsdshoiwu.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hongshengwenyu.top/gtwlynlhvq.html

[T23] Swift：函数
来源：http://hz.mhx1999.top/gtzrwbgcuc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xinyue.icu/gtgsfaaykq.html

[T24] Swift：闭包
来源：http://hz.fengsongda.top/gtqjlfzozn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.aizwys.cn/gtmslytzzm.html

[T25] Swift：结构体
来源：http://hz.shanyushiyangtech.top/gtgsbgvomg.html

struct P { var x: Int }
来源：http://hz.daria6918.cn/gtxhkmfbqq.html

[T26] Swift：类与重写
来源：http://hz.zdqjudy.top/gtjiiefumn.html

class A: Base { override func f() {} }
来源：http://hz.daxiang520.top/gttexnjzti.html

[T27] Swift：错误处理
来源：http://hz.0kj1m.cn/gtegorzsnk.html

do { try f() } catch { print(error) }
来源：http://hz.cqqwz.cn/gtwcqjfhnq.html

[T28] Swift：枚举
来源：http://hz.jianghu66.top/gtkdkmgnca.html

enum Color { case red, green }
来源：http://hz.tianlin.xyz/gtwvpniyxf.html

[T29] Swift：guard 提前返回
来源：http://hz.hnqzz.top/gtunydxmgj.html

guard let x = opt else { return }
来源：http://hz.zhoulong.xyz/gtragtyfzs.html

[T30] Swift：协议
来源：http://hz.xingfuxueyuan.xyz/gtrjyyffxn.html

protocol Shape { func area() -> Double }
来源：http://hz.hnqzz.top/gtfxjhbkxp.html

[T31] Lua：Hello World
来源：http://hz.zhiwuduotai.top/gtjrrkibgr.html

print("Hello")
来源：http://hz.svipenyu.cn/gtiofdtuwj.html

[T32] Lua：局部变量
来源：http://hz.tianlin.xyz/gtaswrsocs.html

local a = 1
来源：http://hz.nanxinkj.top/gtxqvdjuuj.html

[T33] Lua：表（数组）
来源：http://hz.zhijiandao.cn/gtxahgbvet.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yongpay.top/gtdziydcyp.html

[T34] Lua：遍历表
来源：http://hz.chenzaomai.com/gtcjuysqwx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhaomingkeji.xyz/gthdilcjgs.html

[T35] Lua：字典表
来源：http://hz.tian-w.cn/gtsunobndn.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xuanzx.com/gtisolqlkv.html

[T36] Lua：函数
来源：http://hz.sysykeji.top/gtvscydgyg.html

function add(a, b) return a + b end
来源：http://hz.chenzaomai.com/gtmxlwjdot.html

[T37] Lua：字符串拼接
来源：http://hz.pycfn.com/gtflkjgyax.html

"a" .. "b"
来源：http://hz.guannengcc.top/gtyqpdablt.html

[T38] Lua：条件
来源：http://hz.cheryme.top/gtnfftsqba.html

if x > 0 then print("正") end
来源：http://hz.chenzaomai.com/gtgkbfiudi.html

[T39] Lua：模式匹配
来源：http://hz.sysykeji.top/gtruzurxir.html

string.find(s, "%d+")
来源：http://hz.zhixingplan.top/gtqcokexfu.html

[T40] Lua：元表
来源：http://hz.xuetiantiany.cn/gtyigkxnvp.html

setmetatable({}, { __index = base })
来源：http://hz.0kj1m.cn/gtetlijtir.html

[T41] Perl：Hello World
来源：http://hz.andypj.xyz/gtpbdtezoa.html

print "Hello\n";
来源：http://hz.xziqi.cn/gtkkkcekyy.html

[T42] Perl：变量类型
来源：http://hz.yvedp.cn/gtizwozhok.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.tianlin.xyz/gtymgzbowe.html

[T43] Perl：字符串插值
来源：http://hz.vqdsnc.cn/gtfrryixbh.html

"值: $a"
来源：http://hz.yj20258888.top/gtgnouucte.html

[T44] Perl：条件
来源：http://hz.jqgufenzy.top/gtwfipyfkk.html

if ($a > 0) { print "正"; }
来源：http://hz.tian-w.cn/gtijlgepes.html

[T45] Perl：数组遍历
来源：http://hz.meibo888.top/gtkfcmiydp.html

for my $x (@arr) { print $x; }
来源：http://hz.yangfankeji.com/gtbxttstid.html

[T46] Perl：哈希操作
来源：http://hz.yongpay.top/gthnispewb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.cheryme.top/gtvrwplwwq.html

[T47] Perl：正则捕获
来源：http://hz.xylfe.cn/gtadgskfmh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.iojbl.cn/gtnjfiqwax.html

[T48] Perl：正则替换
来源：http://hz.snrcjt.cn/gtmeylueja.html

$s =~ s/old/new/g;
来源：http://hz.ydjk.org.cn/gtlbtdzgbo.html

[T49] Perl：函数
来源：http://hz.xylfe.cn/gttnxrbseq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhiwuduotai.top/gtgegjfsuo.html

[T50] Perl：逐行读文件
来源：http://hz.jyoumei.cn/gteedgawgz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cqqwz.cn/gtybpjosmw.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.shuidangran.top/gtjhicoipc.html

[T51] Scala：Hello World
来源：http://hz.cqqwz.cn/gtibuxihss.html

println("Hello")
来源：http://hz.hnxiangtu.top/gtgadzeves.html

[T52] Scala：变量
来源：http://hz.ydjk.org.cn/gttphwgebp.html

val a = 1;  var b = 2
来源：http://hz.xingfuxueyuan.xyz/gtoxyfwzvy.html

[T53] Scala：字符串插值
来源：http://hz.pycfn.com/gtcgqnqzuu.html

s"值: $b"
来源：http://hz.ydzc1.top/gtptngzizl.html

[T54] Scala：集合映射
来源：http://hz.zhiwuduotai.top/gtcsvfjovd.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yuxming.cn/gtxiakexkc.html

[T55] Scala：集合过滤
来源：http://hz.zhongyouzk.top/gtmrdhkdvw.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.xylfe.cn/gtxfbylljd.html

[T56] Scala：样例类
来源：http://hz.birdmap.top/gtblqnyhut.html


<!-- 参考信息 -->