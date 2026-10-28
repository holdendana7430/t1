代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xziqi.cn/gtpmjetokg.html

[R50] awk 求和
来源：http://hz.ywan-chungtsiang.top/gtgpaxwdku.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hysaishi.cn/gtywyyfxwg.html

[R51] 排序去重取前几
来源：http://hz.jinghuilouyu.cn/gtmczbfbrp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shuidangran.top/gtgppykkon.html

[R52] 统计行数
来源：http://hz.zycfv.cn/gtxrcfkrqx.html

wc -l a.txt
来源：http://hz.sweek.top/gtyugmchea.html

[R53] 查看文件头与实时尾
来源：http://hz.zdqjudy.top/gtztymzstm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sweek.top/gtlosugmhu.html

[R54] 比较两个文件
来源：http://hz.zdqjudy.top/gtvsawhkbd.html

diff a.txt b.txt
来源：http://hz.shzxlz.cn/gtzhajfusi.html

[R55] 压缩与解压
来源：http://hz.yuxming.cn/gtocrxhqsf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.kuanghao11.cn/gthhdvqvhm.html

[R56] 远程拷贝
来源：http://hz.bjfxy.top/gtvwfeieoe.html

scp file user@host:/path/
来源：http://hz.ywan-chungtsiang.top/gtxpxfxqpg.html

[R57] 远程执行命令
来源：http://hz.hfpthk.cn/gtzuhdmgkq.html

ssh user@host 'uptime'
来源：http://hz.svipenyu.cn/gtuckxfntf.html

[R58] 下载文件
来源：http://hz.sxryk.cn/gtevbhzqsq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jiagoushi.top/gtkdqzenew.html

[R59] 发 POST JSON
来源：http://hz.fzhhl.top/gtchtyzcql.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.pengpengdd.cyou/gtyzcmoicf.html

[R60] 只看 HTTP 状态码
来源：http://hz.hongshengwenyu.top/gtblosdzof.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xuanzx.com/gtzgqjinip.html

[R61] 磁盘占用
来源：http://hz.zhaomingkeji.xyz/gtnxaanpxl.html

df -h;  du -sh *
来源：http://hz.aibaodan.cn/gtogstglzv.html

[R62] 找最占空间的文件
来源：http://hz.zycfv.cn/gtqyeshbfi.html

du -ah . | sort -rh | head -10
来源：http://hz.daria6918.cn/gtbptxmimh.html

[R63] 内存与进程
来源：http://hz.yvedp.cn/gtshyzylwc.html

free -h;  ps aux | grep nginx
来源：http://hz.zhixingplan.top/gtwoquyldk.html

[R64] 结束进程
来源：http://hz.pycfn.com/gtbfpsgydv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yongpay.top/gthhdrwmxa.html

[R65] 查看端口占用
来源：http://hz.yueranfly.top/gtlzzslblj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhengqikj.top/gtbjhsxftl.html

[R66] 定时任务
来源：http://hz.yonumen.top/gtgifaiuzh.html

crontab -e;  crontab -l
来源：http://hz.chenlongwang.top/gtwvjxpevr.html

[R67] 生成随机十六进制串
来源：http://hz.vqdsnc.cn/gtbcejjycv.html

openssl rand -hex 16
来源：http://hz.zhaomingkeji.xyz/gtqxzihbda.html

[R68] 计算文件校验值
来源：http://hz.meibo888.top/gthoypswym.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zdqjudy.top/gtvqbsbcvz.html

[R69] 生成随机密码
来源：http://hz.tian-w.cn/gtithayatp.html

head -c 16 /dev/urandom | base64
来源：http://hz.gaohongyu789.top/gtbzuxhgty.html

[R70] 时间戳与互转
来源：http://hz.gzhubu.top/gtnrrylefo.html

date +%s;  date -d @1700000000
来源：http://hz.dianchejie.cn/gtypskhalz.html

[R71] 日期格式化
来源：http://hz.jyoumei.cn/gtxkrmuxvc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhongyouzk.top/gtdoacrcjg.html

[R72] 等待端口就绪
来源：http://hz.nwbrower.top/gtinburqes.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.pengpengdd.cyou/gtktuggcln.html

[R73] 分割大日志
来源：http://hz.chenjidiqi.icu/gtqyetxmuq.html

split -l 1000 big.log part_
来源：http://hz.redwolf501.top/gtettxvium.html

[R74] 批量重命名
来源：http://hz.shuidangran.top/gtalffvake.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yueranfly.top/gtwhabmawm.html

[R75] 导出环境变量
来源：http://hz.chenjidiqi.icu/gtwkywdlut.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.chenzaomai.com/gtezfjdutr.html

[R76] 使用临时文件
来源：http://hz.sxryk.cn/gthvplplfa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ivvv.top/gtgtcqmmle.html

[R77] 读取用户输入
来源：http://hz.xuetiantiany.cn/gtiypocthh.html

read -rp "请输入: " ans
来源：http://hz.aizwys.cn/gtbxqncsvh.html

[R78] 交互式菜单
来源：http://hz.havefunace.top/gtjptniazd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhongyouzk.top/gteaddbdch.html

[R79] 解析命令行选项
来源：http://hz.ywan-chungtsiang.top/gtlboklydt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gogol.net.cn/gtwnrmsfny.html

[R80] 查看脚本执行耗时
来源：http://hz.zycfv.cn/gtfwgitlqa.html

time ./run.sh
来源：http://hz.smart0.xyz/gtswtwdtwo.html

================================================================================
来源：http://hz.yangfankeji.com/gtbrudgzqx.html

S. C / C++ 专题
来源：http://hz.yonumen.top/gtengfoolq.html

================================================================================
来源：http://hz.redwolf501.top/gtrwpxxanf.html

[S01] C：Hello World
来源：http://hz.hywenlv.cn/gtarvesxmu.html

#include <stdio.h>
来源：http://hz.jinqigufen.top/gtsztwfidz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gzhubu.top/gtjfkdzdng.html

[S02] C：变量与格式化输出
来源：http://hz.0kj1m.cn/gtgdkuxzoo.html

int a = 10; printf("%d\n", a);
来源：http://hz.yueranfly.top/gtubtnwgzg.html

[S03] C：读入整数
来源：http://hz.vqdsnc.cn/gtqrhsuifm.html

int x; scanf("%d", &x);
来源：http://hz.dashuyun.cn/gteradniff.html

[S04] C：字符串复制
来源：http://hz.cheryme.top/gtgdvowsjp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hysaishi.cn/gtrjldeowy.html

[S05] C：字符串长度
来源：http://hz.gaohongyu789.top/gtmcaxpksn.html

strlen(s)
来源：http://hz.0kj1m.cn/gtntwraclp.html

[S06] C：字符串比较
来源：http://hz.zhengqikj.top/gtcavecwxp.html

strcmp(a, b) == 0
来源：http://hz.ywan-chungtsiang.top/gtfwclqmyb.html

[S07] C：数组遍历求和
来源：http://hz.hnxiangtu.top/gtejkzozur.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jyoumei.cn/gtlueegrtq.html

[S08] C：动态内存分配与释放
来源：http://hz.9152youxi.cn/gtkewestya.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yanxiufei.cn/gtqjhnrjss.html

[S09] C：结构体定义与初始化
来源：http://hz.shangyingyoupin.top/gtdjynwdnb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.sysykeji.top/gtqraczgjk.html

[S10] C：指针与解引用
来源：http://hz.316326.xyz/gtcdzwbkse.html

int *p = &a;  *p = 5;
来源：http://hz.gaohongyu789.top/gtfznhfbyu.html

[S11] C：逐行读文件
来源：http://hz.gzhubu.top/gtxbhdlynq.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhiwuduotai.top/gtbiicpvex.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.chenzaomai.com/gtibnctibz.html

fclose(f);
来源：http://hz.sxryk.cn/gtlbswrszv.html

[S12] C：写文件
来源：http://hz.jqgfzy.top/gtdytuzwfc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xinyue.icu/gtnlqacjnr.html

[S13] C：宏定义
来源：http://hz.meibo888.top/gtbunqbzbn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.feifeiyinyue.top/gtixlknsbw.html

[S14] C：枚举
来源：http://hz.hongshengwenyu.top/gtyhrwjbyf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.havefunace.top/gtskeziaqy.html

[S15] C：类型转换
来源：http://hz.haohaochexian.top/gtlejgyacb.html

(double) a / b
来源：http://hz.zhijiandao.cn/gtwmdxxwto.html

[S16] C：位操作置位
来源：http://hz.guannengcc.top/gtnolwxxal.html

x |= (1 << 3);
来源：http://hz.zhongyouzk.top/gtnvxwnmlb.html

[S17] C：安全拼接字符串
来源：http://hz.nanxuanxn.top/gtgdvuufau.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.52xcode.cn/gtwfeexghi.html

[S18] C：命令行参数
来源：http://hz.chenlongwang.top/gtjrvgvedx.html

int main(int argc, char **argv)
来源：http://hz.yj20258.top/gtbhclnkzu.html

[S19] C：快速排序
来源：http://hz.zycfv.cn/gtwoipfalv.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hnxiangtu.top/gtqvhvqhwq.html

[S20] C：二分查找
来源：http://hz.wangdashe.top/gtmeveuzvb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhaomingkeji.xyz/gtmwucmnqm.html

[S21] C：字符类别判断
来源：http://hz.xuanzx.com/gtlugaxhtv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.0kj1m.cn/gtcybvlknc.html

[S22] C：字符串转数字
来源：http://hz.zhoulong.xyz/gtnltciitz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.sxryk.cn/gtenhknnfb.html

[S23] C：随机数
来源：http://hz.xylfe.cn/gtlchxzvdv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cdnleiting.top/gtyvfgshhn.html

[S24] C：获取本地时间
来源：http://hz.pycfn.com/gtobzvqdwk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.aibaodan.cn/gtvymawjyy.html

[S25] C：内存拷贝
来源：http://hz.xuanzx.com/gtxainbzxe.html

memcpy(dst, src, n);
来源：http://hz.jqgufenzy.top/gtzbuzmmkl.html

[S26] C：内存清零
来源：http://hz.ywan-chungtsiang.top/gtrpxvsyaf.html

memset(a, 0, sizeof a);
来源：http://hz.xziqi.cn/gtilaogliw.html

[S27] C：定义常量
来源：http://hz.dianchejie.cn/gtcaaemxgd.html

const double PI = 3.14159;
来源：http://hz.dianchejie.cn/gtutcsuxed.html

[S28] C：静态变量
来源：http://hz.nanxuanxn.top/gtlviyarko.html

static int counter = 0;
来源：http://hz.snrcjt.cn/gtqqqfhktm.html

[S29] C：变参函数
来源：http://hz.jiagoushi.top/gtvrbuiira.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cqqwz.cn/gtnpqojebq.html

[S30] C：头文件保护
来源：http://hz.ehwqpu.com/gtpctyomee.html

#ifndef X_H
来源：http://hz.zhongyouzk.top/gtvtkzgyke.html

#define X_H
来源：http://hz.zhaomingkeji.xyz/gtznkbtent.html

#endif
来源：http://hz.zhijiandao.cn/gtejymhqzt.html

[S31] C++：Hello World
来源：http://hz.chenlongwang.top/gtopcebngd.html

#include <iostream>
来源：http://hz.hfpthk.cn/gtyztnodsj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jinghuilouyu.cn/gtruhgdvtv.html

[S32] C++：字符串
来源：http://hz.dianchejie.cn/gtglrpnidz.html

std::string s = "hi";  s += "!";
来源：http://hz.zhengqikj.top/gttkchtaid.html

[S33] C++：vector 增删
来源：http://hz.vqdsnc.cn/gtuhhpprqs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gaohongyu789.top/gtlaepgsdf.html

[S34] C++：遍历 vector
来源：http://hz.shanyushiyangkeji.top/gtjakdabqc.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.tian-w.cn/gtvpmfcfsi.html

[S35] C++：map
来源：http://hz.jinyuanbaomall.cn/gtxdcuwgtr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ehwqpu.com/gtjzjtddnu.html

[S36] C++：unordered_map
来源：http://hz.316326.xyz/gtkugnobsm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sysykeji.top/gtdxbkeeub.html

[S37] C++：set
来源：http://hz.birdmap.top/gtbgxusgsf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhongyouzk.top/gtvwovitce.html

[S38] C++：排序
来源：http://hz.zycfv.cn/gtnnjwxrnp.html

std::sort(v.begin(), v.end());
来源：http://hz.snrcjt.cn/gttdvthtya.html

[S39] C++：自定义比较器排序
来源：http://hz.smart0.xyz/gtxeuutzby.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.andypj.xyz/gtwsjxrxna.html

[S40] C++：查找元素
来源：http://hz.hnqzz.top/gtoowomtqu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.sxryk.cn/gtqcofrwjx.html

[S41] C++：类与构造函数
来源：http://hz.havefunace.top/gtyvdvcxta.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.aibaodan.cn/gtygxqfqmt.html

[S42] C++：继承与虚函数
来源：http://hz.zhoulong.xyz/gtunlnrvqg.html

class B : public Base { public: void f() override {} };
来源：http://hz.xinyue.icu/gtgfstyjer.html

[S43] C++：智能指针
来源：http://hz.yvedp.cn/gtghdtrxbz.html

auto p = std::make_unique<int>(5);
来源：http://hz.tianlin.xyz/gtxhmdlurt.html

[S44] C++：引用传参
来源：http://hz.gzhubu.top/gtmflojqyo.html

void inc(int &x) { ++x; }
来源：http://hz.chenzaomai.com/gtzlsqxytu.html

[S45] C++：lambda
来源：http://hz.gogol.net.cn/gtdchcrkzq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cucudq.cn/gtcmnjeokz.html

[S46] C++：函数模板
来源：http://hz.fzhhl.top/gtodfrukqa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hnqzz.top/gtwpecgwtb.html

[S47] C++：结构化绑定遍历
来源：http://hz.jlsjyb.cn/gtmjvdmfub.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shanyushiyangtech.top/gtarlmndlg.html

[S48] C++：逐行读文件
来源：http://hz.cheryme.top/gthnreipre.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.quarkkingdee.top/gtotrpfaxy.html

while (std::getline(in, line)) { }
来源：http://hz.jinyuanbaomall.cn/gtachehhdh.html

[S49] C++：写文件
来源：http://hz.shzxlz.cn/gtpjmzvjyb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yanxiufei.cn/gtbrkzzeuw.html

[S50] C++：格式化数字
来源：http://hz.shangyingyoupin.top/gtrwvmqhea.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yangfankeji.com/gtrzfobgzh.html

[S51] C++：显式类型转换
来源：http://hz.jlsjyb.cn/gtwtoobcev.html

static_cast<double>(a) / b
来源：http://hz.dashuyun.cn/gtirlyrmqg.html

[S52] C++：const 与 noexcept
来源：http://hz.hnqzz.top/gtkgtokiri.html

int size() const noexcept { return n_; }
来源：http://hz.xziqi.cn/gtwaggqrsy.html

[S53] C++：移动语义
来源：http://hz.jqgufenzy.top/gtcdkcvkkv.html

std::vector<int> w = std::move(v);
来源：http://hz.yj20258888.top/gtzzprqsit.html

[S54] C++：异常处理
来源：http://hz.shzxlz.cn/gttgylsovo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yvedp.cn/gtapghqlms.html

[S55] C++：结构化绑定
来源：http://hz.sufxvd.cn/gthuhwjgdq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jianghu66.top/gtagtkhciv.html

[S56] C++：optional
来源：http://hz.feifeiyinyue.top/gtwgbztxwb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ppjwa.cn/gtcidcukmo.html

[S57] C++：编译期常量
来源：http://hz.yj202588.top/gtcyldywsh.html

constexpr int N = 10;
来源：http://hz.hysaishi.cn/gtsbqsvgic.html

[S58] C++：命名空间
来源：http://hz.guannengcc.top/gtchfznkxd.html

namespace ns { int f() { return 1; } }
来源：http://hz.haohaochexian.top/gtfppzxseh.html

[S59] C++：静态断言
来源：http://hz.ehwqpu.com/gtebeudtun.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.snrcjt.cn/gtcszlcmsj.html

[S60] C++：遍历并删除元素
来源：http://hz.tianlin.xyz/gtnxjdezci.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jianghu66.top/gtnvsnmdwt.html

================================================================================
来源：http://hz.daxiang520.top/gtwinszdru.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.bjfxy.top/gtwnaoftug.html

================================================================================
来源：http://hz.hongshengwenyu.top/gttpauvzjs.html

[T01] Kotlin：Hello World
来源：http://hz.bjfxy.top/gtjurvtfyh.html

println("Hello")
来源：http://hz.snrcjt.cn/gtpqswijgz.html

[T02] Kotlin：变量
来源：http://hz.ywan-chungtsiang.top/gtmoiwtxtv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.bjfxy.top/gtgoazaloz.html

[T03] Kotlin：字符串模板
来源：http://hz.daria6918.cn/gtzjgtcgvh.html

"值: $b"
来源：http://hz.yuanzhike.top/gtiypdeieu.html

[T04] Kotlin：空安全
来源：http://hz.shanyushiyangkeji.top/gtanwkcxgz.html

val n: String? = null;  n?.length
来源：http://hz.yj202588.top/gtbjqlhsvb.html

[T05] Kotlin：when 表达式
来源：http://hz.daria6918.cn/gtalahldxh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.smart0.xyz/gtmhjsjzni.html

[T06] Kotlin：集合映射
来源：http://hz.sysykeji.top/gtdgyjqcvw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jiagoushi.top/gtgbylbuei.html

[T07] Kotlin：集合过滤
来源：http://hz.pycfn.com/gtgojkylpx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.havefunace.top/gtrylkhhaj.html

[T08] Kotlin：数据类
来源：http://hz.yuanzhike.top/gtgowzjjfd.html

data class User(val name: String, val age: Int)
来源：http://hz.redwolf501.top/gtvqajbsgj.html

[T09] Kotlin：扩展函数
来源：http://hz.shuidangran.top/gteuipahhd.html

fun String.exclaim() = this + "!"
来源：http://hz.shanyushiyangtech.top/gtdhnihubl.html

[T10] Kotlin：默认参数
来源：http://hz.fengsongda.top/gtfufpgzkj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhongyouzk.top/gtzqilbrnn.html

[T11] Kotlin：协程
来源：http://hz.dashuyun.cn/gtqyydspuj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhaomingkeji.xyz/gthgnxjhrd.html

[T12] Kotlin：解构声明
来源：http://hz.yj202588.top/gtkrmyeean.html

val (a, b) = Pair(1, 2)
来源：http://hz.ydjk.org.cn/gtxlhpdcsl.html

[T13] Kotlin：只读 Map
来源：http://hz.hysaishi.cn/gttlpljrhe.html

val m = mapOf("a" to 1)
来源：http://hz.shanyushiyangtech.top/gtdtfrhvvw.html

[T14] Kotlin：循环
来源：http://hz.haohaochexian.top/gtafiztrbl.html

for (i in 1..10) println(i)
来源：http://hz.shangyingyoupin.top/gtltodhofz.html

[T15] Kotlin：接口
来源：http://hz.shzxlz.cn/gtwbbfnsjd.html

interface Shape { fun area(): Double }
来源：http://hz.andypj.xyz/gtlcwsicgc.html

[T16] Swift：Hello World
来源：http://hz.jinyuanbaomall.cn/gtkjvspifv.html

print("Hello")
来源：http://hz.chenjidiqi.icu/gtmbowqbqr.html

[T17] Swift：变量与常量
来源：http://hz.chenjidiqi.icu/gthhjkutne.html

var a = 1;  let b = 2
来源：http://hz.smart0.xyz/gtqmrzxrdb.html

[T18] Swift：字符串插值
来源：http://hz.guannengcc.top/gtdxkcgruz.html

"值: \(b)"
来源：http://hz.xziqi.cn/gthxemieeg.html

[T19] Swift：可选绑定
来源：http://hz.zhoulong.xyz/gtnwwewwak.html

if let n = opt { print(n) }
来源：http://hz.guannengcc.top/gtedkiakpt.html

[T20] Swift：数组操作
来源：http://hz.zycfv.cn/gtweldvikt.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ybcxt.top/gtlljsalwe.html

[T21] Swift：遍历
来源：http://hz.fzhhl.top/gtoooctxmp.html

for x in a { print(x) }
来源：http://hz.ydzc1.top/gtaocfgjuo.html

[T22] Swift：字典
来源：http://hz.316326.xyz/gtatxplnwj.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hongshengwenyu.top/gtqtqrykin.html

[T23] Swift：函数
来源：http://hz.mhx1999.top/gtclzurjqk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.316326.xyz/gtriwyfcng.html

[T24] Swift：闭包
来源：http://hz.ivvv.top/gtjuqpviel.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.fzhhl.top/gtczfhsobi.html

[T25] Swift：结构体
来源：http://hz.xziqi.cn/gtzssjfdoa.html

struct P { var x: Int }
来源：http://hz.316326.xyz/gtsatzrwwd.html

[T26] Swift：类与重写
来源：http://hz.guowangkeji.top/gtplxfisut.html

class A: Base { override func f() {} }
来源：http://hz.svipenyu.cn/gteujvsgov.html

[T27] Swift：错误处理
来源：http://hz.hnxiangtu.top/gtoyskzorp.html

do { try f() } catch { print(error) }
来源：http://hz.cucudq.cn/gtlwhbtcll.html

[T28] Swift：枚举
来源：http://hz.jqgfzy.top/gtvykhupkx.html

enum Color { case red, green }
来源：http://hz.yuxming.cn/gtxpfhvzxz.html

[T29] Swift：guard 提前返回
来源：http://hz.yj20258.top/gtaapflxrp.html

guard let x = opt else { return }
来源：http://hz.tianlin.xyz/gtpfqxepce.html

[T30] Swift：协议
来源：http://hz.cashguo.top/gtkepmpidd.html

protocol Shape { func area() -> Double }
来源：http://hz.0kj1m.cn/gtymfsdfhv.html

[T31] Lua：Hello World
来源：http://hz.guannengcc.top/gtnycbleer.html

print("Hello")
来源：http://hz.havefunace.top/gtwvavimku.html

[T32] Lua：局部变量
来源：http://hz.tanke756.top/gtqmbheqbm.html

local a = 1
来源：http://hz.svipenyu.cn/gtkqyzijgv.html

[T33] Lua：表（数组）
来源：http://hz.gaohongyu789.top/gtojnkjojd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xuanzx.com/gtucewmoky.html

[T34] Lua：遍历表
来源：http://hz.nwbrower.top/gtewvufknw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.316326.xyz/gtevgpupak.html

[T35] Lua：字典表
来源：http://hz.redwolf501.top/gtcuvsziti.html

local d = { a = 1 };  d.b = 2
来源：http://hz.tanke756.top/gtiepbwysq.html

[T36] Lua：函数
来源：http://hz.hysaishi.cn/gtxaawrmgx.html

function add(a, b) return a + b end
来源：http://hz.jinghuilouyu.cn/gtnhevpdmk.html

[T37] Lua：字符串拼接
来源：http://hz.yj20258888.top/gttwgrgvmi.html

"a" .. "b"
来源：http://hz.aibaodan.cn/gtojehnqde.html

[T38] Lua：条件
来源：http://hz.c1oappe.top/gtzihlsbtn.html

if x > 0 then print("正") end
来源：http://hz.dashuyun.cn/gtzuwnqemc.html

[T39] Lua：模式匹配
来源：http://hz.daxiang520.top/gtlxvppxvo.html

string.find(s, "%d+")
来源：http://hz.jinqigfzy.top/gtnxrnzrew.html

[T40] Lua：元表
来源：http://hz.hongshengwenyu.top/gtvunhuyrs.html

setmetatable({}, { __index = base })
来源：http://hz.sysykeji.top/gtfqvniplh.html

[T41] Perl：Hello World
来源：http://hz.ydjk.org.cn/gtqawwteti.html

print "Hello\n";
来源：http://hz.ydjk.org.cn/gtzuoqgmkf.html

[T42] Perl：变量类型
来源：http://hz.cdnleiting.top/gtyvkuhvxa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hnqzz.top/gtdxyszbro.html

[T43] Perl：字符串插值
来源：http://hz.0kj1m.cn/gtgcqiejjm.html

"值: $a"
来源：http://hz.guannengcc.top/gtsfhqeqks.html

[T44] Perl：条件
来源：http://hz.jlsjyb.cn/gtxxiduxlf.html

if ($a > 0) { print "正"; }
来源：http://hz.xuanzx.com/gtgskcujlz.html

[T45] Perl：数组遍历
来源：http://hz.pycfn.com/gtnbpjilsz.html

for my $x (@arr) { print $x; }
来源：http://hz.xuetiantiany.cn/gtkmypnuzc.html

[T46] Perl：哈希操作
来源：http://hz.hysaishi.cn/gtrgtzhbaw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.bjfxy.top/gttogpcnil.html

[T47] Perl：正则捕获
来源：http://hz.hnxiangtu.top/gteosnzmbh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jyoumei.cn/gtvgivvctm.html

[T48] Perl：正则替换
来源：http://hz.jlsjyb.cn/gtkkmowbmu.html

$s =~ s/old/new/g;
来源：http://hz.52xcode.cn/gtvdavdami.html

[T49] Perl：函数
来源：http://hz.gaohongyu789.top/gtsgjgldwd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.gaohongyu789.top/gtpgtckazj.html

[T50] Perl：逐行读文件
来源：http://hz.hnqzz.top/gtbosixpck.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.redwolf501.top/gtzatkkmnd.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.wangshuangyany.cn/gtjlgdorbo.html

[T51] Scala：Hello World
来源：http://hz.shanyushiyangkeji.top/gtgtmohaeo.html

println("Hello")
来源：http://hz.yanxiufei.cn/gtrhkcygal.html

[T52] Scala：变量
来源：http://hz.jqgfzy.top/gtkwoelbho.html


<!-- 参考信息 -->