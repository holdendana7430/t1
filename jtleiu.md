代发 wailian999

find . -name "*.log" -type f
来源：http://hz.nwbrower.top/gtinflhmnv.html

[R44] 按修改时间查找
来源：http://hz.zhiwuduotai.top/gtgkzwccvp.html

find . -mtime -7 -type f
来源：http://hz.zhongyouzk.top/gtvtidceeq.html

[R45] 批量删除
来源：http://hz.snrcjt.cn/gtbirmljdm.html

find . -name "*.tmp" -delete
来源：http://hz.zhaomingkeji.xyz/gtobefzset.html

[R46] 递归替换文件内容
来源：http://hz.316326.xyz/gtxmjufmxf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hfpthk.cn/gtkthzwnao.html

[R47] sed 单行替换
来源：http://hz.yuanzhike.top/gttaijgxyb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.andypj.xyz/gtobdzdykb.html

[R48] awk 取指定列
来源：http://hz.gotoacloud.top/gttbrurtlc.html

awk '{print $1, $3}' a.txt
来源：http://hz.xylfe.cn/gtgpnlaray.html

[R49] awk 带条件
来源：http://hz.cheryme.top/gtpyrrjwva.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ehwqpu.com/gtmicobgmn.html

[R50] awk 求和
来源：http://hz.zycfv.cn/gtfqoabzkz.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yuxming.cn/gtcitssxpo.html

[R51] 排序去重取前几
来源：http://hz.316326.xyz/gtoxydfsio.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cdnleiting.top/gtptwdkbiu.html

[R52] 统计行数
来源：http://hz.fzhhl.top/gtreijmupq.html

wc -l a.txt
来源：http://hz.zhiwuduotai.top/gtbonewjqf.html

[R53] 查看文件头与实时尾
来源：http://hz.andypj.xyz/gtrcwnkfzf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gogol.net.cn/gtdmeytmpz.html

[R54] 比较两个文件
来源：http://hz.shzxlz.cn/gtmkyegpxv.html

diff a.txt b.txt
来源：http://hz.xingfuxueyuan.xyz/gtgncnzdeu.html

[R55] 压缩与解压
来源：http://hz.vqdsnc.cn/gtlpbiuiaf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.316326.xyz/gtklcesroe.html

[R56] 远程拷贝
来源：http://hz.guowangkeji.top/gtbvlwzidj.html

scp file user@host:/path/
来源：http://hz.haohaochexian.top/gtxdiejhlh.html

[R57] 远程执行命令
来源：http://hz.xingfuxueyuan.xyz/gtcpbhketq.html

ssh user@host 'uptime'
来源：http://hz.fengsongda.top/gtfglgvxyh.html

[R58] 下载文件
来源：http://hz.xuanzx.com/gtjthvliez.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhengqikj.top/gtznhhogrb.html

[R59] 发 POST JSON
来源：http://hz.aibaodan.cn/gtrrriaird.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yuanzhike.top/gtgngtevmf.html

[R60] 只看 HTTP 状态码
来源：http://hz.yonumen.top/gtnzoxcyfj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.birdmap.top/gtuywdceog.html

[R61] 磁盘占用
来源：http://hz.aibaodan.cn/gtlzuvytot.html

df -h;  du -sh *
来源：http://hz.cqqwz.cn/gtdbdwxcfz.html

[R62] 找最占空间的文件
来源：http://hz.hnqzz.top/gtwmemoylj.html

du -ah . | sort -rh | head -10
来源：http://hz.shanyushiyangtech.top/gtkbtwodgn.html

[R63] 内存与进程
来源：http://hz.nwbrower.top/gthhxvulgl.html

free -h;  ps aux | grep nginx
来源：http://hz.zhiwuduotai.top/gtzxasnxfg.html

[R64] 结束进程
来源：http://hz.bjfxy.top/gtcelzhbcw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ehwqpu.com/gtscrnhaxx.html

[R65] 查看端口占用
来源：http://hz.havefunace.top/gtydiyvhyx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hammf.cn/gtcavcrbjz.html

[R66] 定时任务
来源：http://hz.shuidangran.top/gtnpmyfzgf.html

crontab -e;  crontab -l
来源：http://hz.birdmap.top/gtlmcocqvv.html

[R67] 生成随机十六进制串
来源：http://hz.ehwqpu.com/gtlrqnnyjb.html

openssl rand -hex 16
来源：http://hz.cdnleiting.top/gtiqacrhmf.html

[R68] 计算文件校验值
来源：http://hz.kuanghao11.cn/gtazwnmvki.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ywan-chungtsiang.top/gtlmzggvzi.html

[R69] 生成随机密码
来源：http://hz.shanyushiyangkeji.top/gtfdqsuerd.html

head -c 16 /dev/urandom | base64
来源：http://hz.hnqzz.top/gtcgmawebh.html

[R70] 时间戳与互转
来源：http://hz.jianghu66.top/gtjbyriuor.html

date +%s;  date -d @1700000000
来源：http://hz.svipenyu.cn/gtqnyhzmmx.html

[R71] 日期格式化
来源：http://hz.sxryk.cn/gtmqygizjv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.birdmap.top/gthrmoxssx.html

[R72] 等待端口就绪
来源：http://hz.yangfankeji.com/gtgelodvhx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xuanzx.com/gtidejtund.html

[R73] 分割大日志
来源：http://hz.xylfe.cn/gtbuiddzxl.html

split -l 1000 big.log part_
来源：http://hz.nanxuanxn.top/gtehobhmeo.html

[R74] 批量重命名
来源：http://hz.kuanghao11.cn/gtwtmirkjr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.andypj.xyz/gttffryzvd.html

[R75] 导出环境变量
来源：http://hz.hnxiangtu.top/gtenslsypj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.chenlongwang.top/gtmlmmmbru.html

[R76] 使用临时文件
来源：http://hz.yuanzhike.top/gtfpwprtzb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhoulong.xyz/gtcxgvqgmo.html

[R77] 读取用户输入
来源：http://hz.cqqwz.cn/gtgpdxdutd.html

read -rp "请输入: " ans
来源：http://hz.birdmap.top/gtbroknjnz.html

[R78] 交互式菜单
来源：http://hz.chenjidiqi.icu/gtfdnvyjhk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.fengsongda.top/gtgrdeutau.html

[R79] 解析命令行选项
来源：http://hz.yongpay.top/gtagtiuaij.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jinghuilouyu.cn/gtigfrrqkq.html

[R80] 查看脚本执行耗时
来源：http://hz.c1oappe.top/gtpayugwzc.html

time ./run.sh
来源：http://hz.zycfv.cn/gtalnepbkp.html

================================================================================
来源：http://hz.sufxvd.cn/gthlcdpadi.html

S. C / C++ 专题
来源：http://hz.aizwys.cn/gtgciraqfw.html

================================================================================
来源：http://hz.yuanzhike.top/gtnbkfmfoj.html

[S01] C：Hello World
来源：http://hz.hfpthk.cn/gthrpcwgbw.html

#include <stdio.h>
来源：http://hz.haohaochexian.top/gttpdwbtpy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.chenjidiqi.icu/gtrskgqzzw.html

[S02] C：变量与格式化输出
来源：http://hz.pycfn.com/gtnbzpfhnn.html

int a = 10; printf("%d\n", a);
来源：http://hz.yuanzhike.top/gtxtgutppz.html

[S03] C：读入整数
来源：http://hz.wangshuangyany.cn/gtzpzmotjd.html

int x; scanf("%d", &x);
来源：http://hz.cqqwz.cn/gtfewxgqpd.html

[S04] C：字符串复制
来源：http://hz.hfpthk.cn/gtvfcoxvwy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.chenzaomai.com/gtuwvcldcc.html

[S05] C：字符串长度
来源：http://hz.zhengqikj.top/gtntwnnqet.html

strlen(s)
来源：http://hz.sxryk.cn/gtzmaqnrsz.html

[S06] C：字符串比较
来源：http://hz.bjfxy.top/gtqtsbhwbt.html

strcmp(a, b) == 0
来源：http://hz.bjfxy.top/gtjimybxej.html

[S07] C：数组遍历求和
来源：http://hz.yj20258.top/gtsnhmozbu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.aibaodan.cn/gteifuxypq.html

[S08] C：动态内存分配与释放
来源：http://hz.sxryk.cn/gtvdayxiob.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinqigfzy.top/gtvoopdhga.html

[S09] C：结构体定义与初始化
来源：http://hz.nanxinkj.top/gtgahosgou.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.pycfn.com/gteiruaejs.html

[S10] C：指针与解引用
来源：http://hz.xziqi.cn/gtdsgptlku.html

int *p = &a;  *p = 5;
来源：http://hz.aizwys.cn/gtujevymim.html

[S11] C：逐行读文件
来源：http://hz.yonumen.top/gtkskgyrng.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shzxlz.cn/gtgoquqkla.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.redwolf501.top/gtivphzbar.html

fclose(f);
来源：http://hz.fengsongda.top/gtrdvymjel.html

[S12] C：写文件
来源：http://hz.vqdsnc.cn/gtkyzesrzn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.fengsongda.top/gtwueziofj.html

[S13] C：宏定义
来源：http://hz.zhiwuduotai.top/gtuqmrqyqy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xziqi.cn/gtvxbhtfma.html

[S14] C：枚举
来源：http://hz.wangshuangyany.cn/gtehuvjvsi.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cheryme.top/gterkghmwi.html

[S15] C：类型转换
来源：http://hz.guannengcc.top/gtveambazz.html

(double) a / b
来源：http://hz.yj20258.top/gtbzhtkrwd.html

[S16] C：位操作置位
来源：http://hz.cheryme.top/gtylrbmvms.html

x |= (1 << 3);
来源：http://hz.guowangkeji.top/gtitcgphss.html

[S17] C：安全拼接字符串
来源：http://hz.jinghuilouyu.cn/gtklodifkp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.haohaochexian.top/gtkojemlse.html

[S18] C：命令行参数
来源：http://hz.ydjk.org.cn/gtgxwyohfc.html

int main(int argc, char **argv)
来源：http://hz.iojbl.cn/gtnufubhxq.html

[S19] C：快速排序
来源：http://hz.hysaishi.cn/gtmeieyinc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yuanzhike.top/gticfkvrhm.html

[S20] C：二分查找
来源：http://hz.dianchejie.cn/gtvjqjlrvb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.redwolf501.top/gtqlmjvcrp.html

[S21] C：字符类别判断
来源：http://hz.svipenyu.cn/gtartpzsky.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.pycfn.com/gttogejexd.html

[S22] C：字符串转数字
来源：http://hz.xuetiantiany.cn/gtegmduhpl.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhaomingkeji.xyz/gtxvctdmri.html

[S23] C：随机数
来源：http://hz.aibaodan.cn/gtzzbsppqm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.bjfxy.top/gtrbvxjmuo.html

[S24] C：获取本地时间
来源：http://hz.0kj1m.cn/gtuzpduqte.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ywan-chungtsiang.top/gtgaspxslr.html

[S25] C：内存拷贝
来源：http://hz.sysykeji.top/gtixrjwuzg.html

memcpy(dst, src, n);
来源：http://hz.shanyushiyangkeji.top/gtyktkwfeq.html

[S26] C：内存清零
来源：http://hz.vqdsnc.cn/gtnuhmfvpw.html

memset(a, 0, sizeof a);
来源：http://hz.daxiang520.top/gtxcojcqla.html

[S27] C：定义常量
来源：http://hz.shangyingyoupin.top/gtklijukhp.html

const double PI = 3.14159;
来源：http://hz.gaohongyu789.top/gtdpnqdcho.html

[S28] C：静态变量
来源：http://hz.hysaishi.cn/gtbavbwbtx.html

static int counter = 0;
来源：http://hz.aibaodan.cn/gtkgwzgibr.html

[S29] C：变参函数
来源：http://hz.gotoacloud.top/gttofyqfsz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinqigufen.top/gtobrwagml.html

[S30] C：头文件保护
来源：http://hz.shuidangran.top/gtphwbnkpt.html

#ifndef X_H
来源：http://hz.vqdsnc.cn/gtappqitgg.html

#define X_H
来源：http://hz.chenlongwang.top/gtzdyimtct.html

#endif
来源：http://hz.xingfuxueyuan.xyz/gttjuujzjb.html

[S31] C++：Hello World
来源：http://hz.meibo888.top/gtldyltcrn.html

#include <iostream>
来源：http://hz.xinyue.icu/gteyvrthbi.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.daxiang520.top/gtjfqmndco.html

[S32] C++：字符串
来源：http://hz.nanxinkj.top/gtsuwabnmi.html

std::string s = "hi";  s += "!";
来源：http://hz.jqgfzy.top/gtfiriixza.html

[S33] C++：vector 增删
来源：http://hz.mhx1999.top/gtbyncucsf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.snrcjt.cn/gtjmjneqxr.html

[S34] C++：遍历 vector
来源：http://hz.meibo888.top/gtqbypfjot.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ybcxt.top/gtblzlwqdn.html

[S35] C++：map
来源：http://hz.smart0.xyz/gtrniaevzn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sxryk.cn/gtkifzzwqr.html

[S36] C++：unordered_map
来源：http://hz.xylfe.cn/gtohqfucob.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.daxiang520.top/gtrdvgzxbj.html

[S37] C++：set
来源：http://hz.xuanzx.com/gtolubqhom.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jianghu66.top/gtmdiztgfp.html

[S38] C++：排序
来源：http://hz.zhijiandao.cn/gtmuytenzj.html

std::sort(v.begin(), v.end());
来源：http://hz.tian-w.cn/gtgnmqtadb.html

[S39] C++：自定义比较器排序
来源：http://hz.zhoulong.xyz/gtauojsuxr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.mhx1999.top/gtfbkuedmk.html

[S40] C++：查找元素
来源：http://hz.xuetiantiany.cn/gtlktddwqb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yj20258.top/gtqxydfpcq.html

[S41] C++：类与构造函数
来源：http://hz.shuidangran.top/gtqlrjrqdj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jqgufenzy.top/gtagrhcmsz.html

[S42] C++：继承与虚函数
来源：http://hz.jinqigufen.top/gtnazjhzbz.html

class B : public Base { public: void f() override {} };
来源：http://hz.wangdashe.top/gtcwmpekmv.html

[S43] C++：智能指针
来源：http://hz.hnxiangtu.top/gtaohchswd.html

auto p = std::make_unique<int>(5);
来源：http://hz.jianghu66.top/gtqffouqga.html

[S44] C++：引用传参
来源：http://hz.yuanzhike.top/gtdxgyoavu.html

void inc(int &x) { ++x; }
来源：http://hz.gzhubu.top/gtdpwinmyg.html

[S45] C++：lambda
来源：http://hz.shanyushiyangkeji.top/gtnetqsqtz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhaomingkeji.xyz/gtciqqoyym.html

[S46] C++：函数模板
来源：http://hz.jiagoushi.top/gtotiqjlll.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.bjfxy.top/gtzntkdonp.html

[S47] C++：结构化绑定遍历
来源：http://hz.wangdashe.top/gttjabvoen.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hnqzz.top/gttrsoynos.html

[S48] C++：逐行读文件
来源：http://hz.birdmap.top/gthxjeglnt.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenjidiqi.icu/gtsleeunay.html

while (std::getline(in, line)) { }
来源：http://hz.xuanzx.com/gtrmqbckzl.html

[S49] C++：写文件
来源：http://hz.shzxlz.cn/gtymwotkkz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jqgfzy.top/gtlujsebhh.html

[S50] C++：格式化数字
来源：http://hz.mhx1999.top/gthxibufks.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.chenjidiqi.icu/gtpbmnupel.html

[S51] C++：显式类型转换
来源：http://hz.316326.xyz/gtgkxbgdwe.html

static_cast<double>(a) / b
来源：http://hz.sweek.top/gtvxomwupn.html

[S52] C++：const 与 noexcept
来源：http://hz.hfpthk.cn/gtnadoqbgi.html

int size() const noexcept { return n_; }
来源：http://hz.smart0.xyz/gtqvrgmisj.html

[S53] C++：移动语义
来源：http://hz.iojbl.cn/gthnhpeicl.html

std::vector<int> w = std::move(v);
来源：http://hz.ybcxt.top/gtzwjlpmyb.html

[S54] C++：异常处理
来源：http://hz.cqqwz.cn/gtbyamctca.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jqgufenzy.top/gtdzwgpxyl.html

[S55] C++：结构化绑定
来源：http://hz.fzhhl.top/gtlibbaxhs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gogol.net.cn/gthetzeerq.html

[S56] C++：optional
来源：http://hz.fengsongda.top/gtdewiamyf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zycfv.cn/gtpejqurwb.html

[S57] C++：编译期常量
来源：http://hz.xziqi.cn/gtibnyicra.html

constexpr int N = 10;
来源：http://hz.c1oappe.top/gteoldfqzn.html

[S58] C++：命名空间
来源：http://hz.sufxvd.cn/gtqwjjkdrt.html

namespace ns { int f() { return 1; } }
来源：http://hz.xuetiantiany.cn/gtmvdopgqi.html

[S59] C++：静态断言
来源：http://hz.zdqjudy.top/gtswrenodf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yj20258888.top/gtbabxcelt.html

[S60] C++：遍历并删除元素
来源：http://hz.jqgfzy.top/gtkwfizkis.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.fengsongda.top/gtvmosukkq.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtkphiizqb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.52xcode.cn/gtpfzppdzn.html

================================================================================
来源：http://hz.tianlin.xyz/gtovtqgwcl.html

[T01] Kotlin：Hello World
来源：http://hz.52xcode.cn/gtyzdznwft.html

println("Hello")
来源：http://hz.yangfankeji.com/gtsizgtbpc.html

[T02] Kotlin：变量
来源：http://hz.hnqzz.top/gtotaguydt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.52xcode.cn/gthgjoncdp.html

[T03] Kotlin：字符串模板
来源：http://hz.gzhubu.top/gtarxolgil.html

"值: $b"
来源：http://hz.sufxvd.cn/gtrgbuoojy.html

[T04] Kotlin：空安全
来源：http://hz.dashuyun.cn/gtxonupyuz.html

val n: String? = null;  n?.length
来源：http://hz.daxiang520.top/gtizolgnnr.html

[T05] Kotlin：when 表达式
来源：http://hz.nanxinkj.top/gtpowhvbpo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinqigufen.top/gtlkjlhfsx.html

[T06] Kotlin：集合映射
来源：http://hz.birdmap.top/gttqahbrog.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gogol.net.cn/gtnpalfsto.html

[T07] Kotlin：集合过滤
来源：http://hz.sysykeji.top/gtilwsjcvq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.52xcode.cn/gtszzmidfe.html

[T08] Kotlin：数据类
来源：http://hz.zhiwuduotai.top/gtqitkwpvn.html

data class User(val name: String, val age: Int)
来源：http://hz.ydzc1.top/gtygydqtju.html

[T09] Kotlin：扩展函数
来源：http://hz.andypj.xyz/gtoojlpzjf.html

fun String.exclaim() = this + "!"
来源：http://hz.kuanghao11.cn/gtpapgtiof.html

[T10] Kotlin：默认参数
来源：http://hz.xylfe.cn/gtlpmidfhz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinqigufen.top/gtwgnqzccd.html

[T11] Kotlin：协程
来源：http://hz.yj202588.top/gtewsjftaz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.tian-w.cn/gttpukpupq.html

[T12] Kotlin：解构声明
来源：http://hz.yongpay.top/gtshtpcxlm.html

val (a, b) = Pair(1, 2)
来源：http://hz.snrcjt.cn/gtokqyttnp.html

[T13] Kotlin：只读 Map
来源：http://hz.mhx1999.top/gtxydxwiwj.html

val m = mapOf("a" to 1)
来源：http://hz.sufxvd.cn/gtacdpfltu.html

[T14] Kotlin：循环
来源：http://hz.chenzaomai.com/gtfjlepjyg.html

for (i in 1..10) println(i)
来源：http://hz.316326.xyz/gtbkmahbgk.html

[T15] Kotlin：接口
来源：http://hz.xinyue.icu/gtnfhjznzv.html

interface Shape { fun area(): Double }
来源：http://hz.yj20258888.top/gtzybsmnlj.html

[T16] Swift：Hello World
来源：http://hz.0kj1m.cn/gtoipcqrfq.html

print("Hello")
来源：http://hz.nanxinkj.top/gtdfxcwyhx.html

[T17] Swift：变量与常量
来源：http://hz.sweek.top/gtjsvclgof.html

var a = 1;  let b = 2
来源：http://hz.dashuyun.cn/gthcmznjgy.html

[T18] Swift：字符串插值
来源：http://hz.ehwqpu.com/gtvmbxloyi.html

"值: \(b)"
来源：http://hz.gotoacloud.top/gtwrqbarkd.html

[T19] Swift：可选绑定
来源：http://hz.yangfankeji.com/gtzutyynff.html

if let n = opt { print(n) }
来源：http://hz.wangdashe.top/gtmauxtxiz.html

[T20] Swift：数组操作
来源：http://hz.mhx1999.top/gttjbwvjuw.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sysykeji.top/gthpzhiivh.html

[T21] Swift：遍历
来源：http://hz.jiagoushi.top/gtmdzebjws.html

for x in a { print(x) }
来源：http://hz.snrcjt.cn/gtflrwgvtl.html

[T22] Swift：字典
来源：http://hz.xingfuxueyuan.xyz/gtpldzegja.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.feifeiyinyue.top/gtgmwlqaxi.html

[T23] Swift：函数
来源：http://hz.yvedp.cn/gtrxnhqklo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.guowangkeji.top/gtuolscbhr.html

[T24] Swift：闭包
来源：http://hz.ydjk.org.cn/gtkdhjfosc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cucudq.cn/gtkkrrtihq.html

[T25] Swift：结构体
来源：http://hz.andypj.xyz/gtdmxsiwkv.html

struct P { var x: Int }
来源：http://hz.jlsjyb.cn/gtxcthgjyh.html

[T26] Swift：类与重写
来源：http://hz.nanxuanxn.top/gtatiqmkss.html

class A: Base { override func f() {} }
来源：http://hz.pengpengdd.cyou/gtjmwcbeca.html

[T27] Swift：错误处理
来源：http://hz.0kj1m.cn/gtnufmgmnt.html

do { try f() } catch { print(error) }
来源：http://hz.sweek.top/gthfevwxvb.html

[T28] Swift：枚举
来源：http://hz.52xcode.cn/gthkocxoav.html

enum Color { case red, green }
来源：http://hz.xziqi.cn/gtxjhrmllc.html

[T29] Swift：guard 提前返回
来源：http://hz.sysykeji.top/gtwsxewxby.html

guard let x = opt else { return }
来源：http://hz.cdnleiting.top/gtwuswygcp.html

[T30] Swift：协议
来源：http://hz.xinyue.icu/gtbsnxalyo.html

protocol Shape { func area() -> Double }
来源：http://hz.cqqwz.cn/gtfvomosag.html

[T31] Lua：Hello World
来源：http://hz.zycfv.cn/gtqfsacysp.html

print("Hello")
来源：http://hz.zhaomingkeji.xyz/gtjfeaecyi.html

[T32] Lua：局部变量
来源：http://hz.yuanzhike.top/gtqervjjgp.html

local a = 1
来源：http://hz.xziqi.cn/gttrrutugq.html

[T33] Lua：表（数组）
来源：http://hz.pengpengdd.cyou/gtpkptpjod.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.andypj.xyz/gthlreorpk.html

[T34] Lua：遍历表
来源：http://hz.shangyingyoupin.top/gtsgosxivg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hysaishi.cn/gtwviwddjn.html

[T35] Lua：字典表
来源：http://hz.tian-w.cn/gtquemzynu.html

local d = { a = 1 };  d.b = 2
来源：http://hz.shzxlz.cn/gttdyddzkg.html

[T36] Lua：函数
来源：http://hz.hysaishi.cn/gtjjkyfebg.html

function add(a, b) return a + b end
来源：http://hz.ppjwa.cn/gtdudhvrtu.html

[T37] Lua：字符串拼接
来源：http://hz.aibaodan.cn/gthepytnsp.html

"a" .. "b"
来源：http://hz.hnqzz.top/gtwpdnfcom.html

[T38] Lua：条件
来源：http://hz.jinghuilouyu.cn/gtcxtarecs.html

if x > 0 then print("正") end
来源：http://hz.yonumen.top/gtdzdvnwfv.html

[T39] Lua：模式匹配
来源：http://hz.gotoacloud.top/gtzevqwlju.html

string.find(s, "%d+")
来源：http://hz.yueranfly.top/gtosvutxcj.html

[T40] Lua：元表
来源：http://hz.yuxming.cn/gtrmifrsrp.html

setmetatable({}, { __index = base })
来源：http://hz.52xcode.cn/gtbsyyvjfd.html

[T41] Perl：Hello World
来源：http://hz.nanxinkj.top/gtjgeryggm.html

print "Hello\n";
来源：http://hz.shanyushiyangkeji.top/gttbplhbha.html

[T42] Perl：变量类型
来源：http://hz.dashuyun.cn/gtrjuwuuuc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yj20258.top/gtsgtkmdar.html

[T43] Perl：字符串插值
来源：http://hz.shangyingyoupin.top/gtoyshppsa.html

"值: $a"
来源：http://hz.hfpthk.cn/gtssnbhawe.html

[T44] Perl：条件
来源：http://hz.svipenyu.cn/gtnewpstpa.html

if ($a > 0) { print "正"; }
来源：http://hz.zhaomingkeji.xyz/gtvtiujlwd.html

[T45] Perl：数组遍历
来源：http://hz.cheryme.top/gtoeozvgat.html

for my $x (@arr) { print $x; }
来源：http://hz.zhixingplan.top/gtuykqvqfh.html

[T46] Perl：哈希操作
来源：http://hz.jinqigfzy.top/gtfvlfpzim.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.cucudq.cn/gtgsxywovn.html


<!-- 参考信息 -->