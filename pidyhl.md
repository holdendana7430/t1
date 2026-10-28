代发 wailian999

cmd >/dev/null 2>&1
来源：http://hz.wangshuangyany.cn/gtzgbpwfdn.html

[R42] 输入重定向
来源：http://hz.yongpay.top/gtbfpsctxz.html

wc -l < a.txt
来源：http://hz.shanyushiyangtech.top/gtkspakufx.html

[R43] 按名字查找文件
来源：http://hz.ppjwa.cn/gtkdsqojzu.html

find . -name "*.log" -type f
来源：http://hz.smart0.xyz/gtqvtazmrz.html

[R44] 按修改时间查找
来源：http://hz.yvedp.cn/gtzdlgiqgl.html

find . -mtime -7 -type f
来源：http://hz.jinghuilouyu.cn/gtfhwzcdhv.html

[R45] 批量删除
来源：http://hz.jinyuanbaomall.cn/gtkbkgutsu.html

find . -name "*.tmp" -delete
来源：http://hz.mhx1999.top/gtgyklkvus.html

[R46] 递归替换文件内容
来源：http://hz.fzhhl.top/gtbccebgel.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sxryk.cn/gtyecwcbws.html

[R47] sed 单行替换
来源：http://hz.yueranfly.top/gtwvplfurc.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.kuanghao11.cn/gtczlvtzsc.html

[R48] awk 取指定列
来源：http://hz.52xcode.cn/gtdiqlxqlz.html

awk '{print $1, $3}' a.txt
来源：http://hz.tian-w.cn/gtjkvtaezx.html

[R49] awk 带条件
来源：http://hz.nanxinkj.top/gtvhrfoblm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.316326.xyz/gtfcxzypjq.html

[R50] awk 求和
来源：http://hz.chenjidiqi.icu/gtyifihcby.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yonumen.top/gtvmnbzotb.html

[R51] 排序去重取前几
来源：http://hz.cdnleiting.top/gtvnbfalzg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tian-w.cn/gtnowpvgtr.html

[R52] 统计行数
来源：http://hz.zdqjudy.top/gtenmogexa.html

wc -l a.txt
来源：http://hz.jyoumei.cn/gtjlcdyssh.html

[R53] 查看文件头与实时尾
来源：http://hz.yj202588.top/gtejxcjipa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cdnleiting.top/gtvdlahioz.html

[R54] 比较两个文件
来源：http://hz.c1oappe.top/gtetegmsgq.html

diff a.txt b.txt
来源：http://hz.ydjk.org.cn/gtogxdjozg.html

[R55] 压缩与解压
来源：http://hz.hywenlv.cn/gtivwubfzx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nanxuanxn.top/gtzzrfzruq.html

[R56] 远程拷贝
来源：http://hz.nanxinkj.top/gtlihsqyut.html

scp file user@host:/path/
来源：http://hz.chenlongwang.top/gtmpehwkin.html

[R57] 远程执行命令
来源：http://hz.xingfuxueyuan.xyz/gtrrtqrogm.html

ssh user@host 'uptime'
来源：http://hz.aibaodan.cn/gtimsrxpww.html

[R58] 下载文件
来源：http://hz.dianchejie.cn/gtowhmctss.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.fzhhl.top/gtflyvcjah.html

[R59] 发 POST JSON
来源：http://hz.gogol.net.cn/gtplwlvrtj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.sysykeji.top/gtxpvhunhl.html

[R60] 只看 HTTP 状态码
来源：http://hz.xingfuxueyuan.xyz/gtnewnmguu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ehwqpu.com/gtkfumoyjm.html

[R61] 磁盘占用
来源：http://hz.wangshuangyany.cn/gtrivkjrdd.html

df -h;  du -sh *
来源：http://hz.sysykeji.top/gtzmuvfpjw.html

[R62] 找最占空间的文件
来源：http://hz.mhx1999.top/gtatoummxp.html

du -ah . | sort -rh | head -10
来源：http://hz.tanke756.top/gtxvrrjwuq.html

[R63] 内存与进程
来源：http://hz.gogol.net.cn/gthuparefz.html

free -h;  ps aux | grep nginx
来源：http://hz.daria6918.cn/gtsmuqdqwu.html

[R64] 结束进程
来源：http://hz.zdqjudy.top/gtclmpztlf.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinghuilouyu.cn/gtlzdbunjd.html

[R65] 查看端口占用
来源：http://hz.bjfxy.top/gtfluqtalc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yj20258.top/gtnraovgzi.html

[R66] 定时任务
来源：http://hz.jiagoushi.top/gtcypifjwx.html

crontab -e;  crontab -l
来源：http://hz.ydjk.org.cn/gtvlaaqalb.html

[R67] 生成随机十六进制串
来源：http://hz.jlsjyb.cn/gtgmxmlrod.html

openssl rand -hex 16
来源：http://hz.zycfv.cn/gtjpgxfcuv.html

[R68] 计算文件校验值
来源：http://hz.jqgufenzy.top/gtmyqalzte.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.chenjidiqi.icu/gtsvhlvxom.html

[R69] 生成随机密码
来源：http://hz.daria6918.cn/gtdidxisln.html

head -c 16 /dev/urandom | base64
来源：http://hz.tianlin.xyz/gtlhnxcdgk.html

[R70] 时间戳与互转
来源：http://hz.316326.xyz/gtomfylvyi.html

date +%s;  date -d @1700000000
来源：http://hz.haohaochexian.top/gtiiulqord.html

[R71] 日期格式化
来源：http://hz.tianlin.xyz/gtyglpzqri.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.0kj1m.cn/gtzqpjpaow.html

[R72] 等待端口就绪
来源：http://hz.mhx1999.top/gtcrwyfair.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hongshengwenyu.top/gtrrlemvpc.html

[R73] 分割大日志
来源：http://hz.gaohongyu789.top/gtgupzovla.html

split -l 1000 big.log part_
来源：http://hz.guowangkeji.top/gttafxqwzn.html

[R74] 批量重命名
来源：http://hz.jlsjyb.cn/gtaivttiud.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zycfv.cn/gtgmypkwkl.html

[R75] 导出环境变量
来源：http://hz.cashguo.top/gtpgckztkk.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xuanzx.com/gtavyosxbn.html

[R76] 使用临时文件
来源：http://hz.jiagoushi.top/gtdtbhszcf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.c1oappe.top/gtzltseoos.html

[R77] 读取用户输入
来源：http://hz.shangyingyoupin.top/gtrioftjui.html

read -rp "请输入: " ans
来源：http://hz.jiagoushi.top/gtoumhjwpk.html

[R78] 交互式菜单
来源：http://hz.hnxiangtu.top/gtjyrpqlzx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ivvv.top/gtnvykwfek.html

[R79] 解析命令行选项
来源：http://hz.daxiang520.top/gttenzbloy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ppjwa.cn/gtruqpskew.html

[R80] 查看脚本执行耗时
来源：http://hz.yongpay.top/gtjqfdytzq.html

time ./run.sh
来源：http://hz.tianlin.xyz/gtmqkqimra.html

================================================================================
来源：http://hz.xinyue.icu/gtucgkhjdd.html

S. C / C++ 专题
来源：http://hz.aizwys.cn/gthhweqykm.html

================================================================================
来源：http://hz.jinqigfzy.top/gtwucsjyli.html

[S01] C：Hello World
来源：http://hz.52xcode.cn/gtmvwdqbsm.html

#include <stdio.h>
来源：http://hz.fengsongda.top/gtoqpdtloz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gaohongyu789.top/gticuedugu.html

[S02] C：变量与格式化输出
来源：http://hz.jlsjyb.cn/gthifkzuzu.html

int a = 10; printf("%d\n", a);
来源：http://hz.xylfe.cn/gtzqmaqofc.html

[S03] C：读入整数
来源：http://hz.zhengqikj.top/gtbrwcpofz.html

int x; scanf("%d", &x);
来源：http://hz.yueranfly.top/gtnjqqgryp.html

[S04] C：字符串复制
来源：http://hz.andypj.xyz/gtvnnssmsn.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cashguo.top/gtfrlgkdyq.html

[S05] C：字符串长度
来源：http://hz.vqdsnc.cn/gturchdegn.html

strlen(s)
来源：http://hz.hongshengwenyu.top/gtorxynmgj.html

[S06] C：字符串比较
来源：http://hz.hysaishi.cn/gtykerfrwq.html

strcmp(a, b) == 0
来源：http://hz.yongpay.top/gtdyahlwfc.html

[S07] C：数组遍历求和
来源：http://hz.jyoumei.cn/gttmxxqjfr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yangfankeji.com/gtzvexxvut.html

[S08] C：动态内存分配与释放
来源：http://hz.aibaodan.cn/gtsxsonqid.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.kuanghao11.cn/gtjpekgzet.html

[S09] C：结构体定义与初始化
来源：http://hz.xuanzx.com/gtxbtjzqxc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.dashuyun.cn/gtnvrqhelb.html

[S10] C：指针与解引用
来源：http://hz.jianghu66.top/gtgccjoqrc.html

int *p = &a;  *p = 5;
来源：http://hz.yvedp.cn/gtylwfgdrf.html

[S11] C：逐行读文件
来源：http://hz.316326.xyz/gtcruvqjiz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ydjk.org.cn/gtbbxwmhlp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.sweek.top/gtfkladijk.html

fclose(f);
来源：http://hz.hammf.cn/gtueumsioa.html

[S12] C：写文件
来源：http://hz.havefunace.top/gtrhzdduut.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yueranfly.top/gtvrjocrpj.html

[S13] C：宏定义
来源：http://hz.feifeiyinyue.top/gtmiwmujfe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ivvv.top/gtyapgcrlj.html

[S14] C：枚举
来源：http://hz.zhixingplan.top/gtswixvmqu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jlsjyb.cn/gtotehaiwg.html

[S15] C：类型转换
来源：http://hz.zhiwuduotai.top/gtcvoomccw.html

(double) a / b
来源：http://hz.havefunace.top/gtwsdxwqhq.html

[S16] C：位操作置位
来源：http://hz.gzhubu.top/gtchsfhfyv.html

x |= (1 << 3);
来源：http://hz.xuetiantiany.cn/gthxuwwfor.html

[S17] C：安全拼接字符串
来源：http://hz.pycfn.com/gtkiappqvo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.chenlongwang.top/gtdxxmvjde.html

[S18] C：命令行参数
来源：http://hz.cucudq.cn/gtiqilxwxp.html

int main(int argc, char **argv)
来源：http://hz.mhx1999.top/gtvzkhnpos.html

[S19] C：快速排序
来源：http://hz.nwbrower.top/gteqvmctvl.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yonumen.top/gtsvuthnzi.html

[S20] C：二分查找
来源：http://hz.iojbl.cn/gtjgzrixxf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jiagoushi.top/gthtxahuwo.html

[S21] C：字符类别判断
来源：http://hz.fengsongda.top/gtktpqtual.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gzhubu.top/gtovwjgxgx.html

[S22] C：字符串转数字
来源：http://hz.hongshengwenyu.top/gtucnwvntm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yongpay.top/gtmnnbknou.html

[S23] C：随机数
来源：http://hz.jqgfzy.top/gtcmylqrms.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.guannengcc.top/gtzvizosmw.html

[S24] C：获取本地时间
来源：http://hz.kuanghao11.cn/gtbynqxcqp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.sxryk.cn/gtfvaaovrl.html

[S25] C：内存拷贝
来源：http://hz.316326.xyz/gtkkbpbnka.html

memcpy(dst, src, n);
来源：http://hz.hnqzz.top/gtikwdidqz.html

[S26] C：内存清零
来源：http://hz.hfpthk.cn/gtkpwyxspm.html

memset(a, 0, sizeof a);
来源：http://hz.shangyingyoupin.top/gtnizlrqbk.html

[S27] C：定义常量
来源：http://hz.ivvv.top/gtmmpccyus.html

const double PI = 3.14159;
来源：http://hz.ppjwa.cn/gtvgmuyxqh.html

[S28] C：静态变量
来源：http://hz.52xcode.cn/gtnkbwowmf.html

static int counter = 0;
来源：http://hz.jinyuanbaomall.cn/gtjrexajmv.html

[S29] C：变参函数
来源：http://hz.yj20258.top/gtoogqunsp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.guannengcc.top/gtozuoiuyc.html

[S30] C：头文件保护
来源：http://hz.zdqjudy.top/gtckwfegtm.html

#ifndef X_H
来源：http://hz.jlsjyb.cn/gtnbbfiprr.html

#define X_H
来源：http://hz.pycfn.com/gtvmhwsbei.html

#endif
来源：http://hz.chenjidiqi.icu/gtadaofutc.html

[S31] C++：Hello World
来源：http://hz.sysykeji.top/gtaevzazlf.html

#include <iostream>
来源：http://hz.jyoumei.cn/gtfonjzhhq.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gaohongyu789.top/gtpibtkdig.html

[S32] C++：字符串
来源：http://hz.ywan-chungtsiang.top/gtanapmqsl.html

std::string s = "hi";  s += "!";
来源：http://hz.jiagoushi.top/gtqywayoxe.html

[S33] C++：vector 增删
来源：http://hz.ydjk.org.cn/gtjahlmgeb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zycfv.cn/gtkcwfntql.html

[S34] C++：遍历 vector
来源：http://hz.ywan-chungtsiang.top/gtwtxzxuuo.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yuanzhike.top/gteezeikao.html

[S35] C++：map
来源：http://hz.ydjk.org.cn/gtqjcpwgdn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenlongwang.top/gtohebmujp.html

[S36] C++：unordered_map
来源：http://hz.zycfv.cn/gthgfedwnp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dashuyun.cn/gthfxwuxse.html

[S37] C++：set
来源：http://hz.aibaodan.cn/gtgmmcfksa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hnqzz.top/gttimdmwud.html

[S38] C++：排序
来源：http://hz.birdmap.top/gtwwmgawkb.html

std::sort(v.begin(), v.end());
来源：http://hz.wangdashe.top/gtsczvvhky.html

[S39] C++：自定义比较器排序
来源：http://hz.bjfxy.top/gtchdyhmxc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhiwuduotai.top/gtjgzwqscw.html

[S40] C++：查找元素
来源：http://hz.guannengcc.top/gtjydlwryp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hammf.cn/gtoxtvrwsl.html

[S41] C++：类与构造函数
来源：http://hz.hywenlv.cn/gtlysqcjje.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.quarkkingdee.top/gtwtdwivbv.html

[S42] C++：继承与虚函数
来源：http://hz.xuetiantiany.cn/gtrnxjmmdm.html

class B : public Base { public: void f() override {} };
来源：http://hz.haohaochexian.top/gtmtylnrwh.html

[S43] C++：智能指针
来源：http://hz.redwolf501.top/gtruvgzbtq.html

auto p = std::make_unique<int>(5);
来源：http://hz.sxryk.cn/gtsgxodkua.html

[S44] C++：引用传参
来源：http://hz.xinyue.icu/gtembigxlx.html

void inc(int &x) { ++x; }
来源：http://hz.zhiwuduotai.top/gtyuwjcgly.html

[S45] C++：lambda
来源：http://hz.ehwqpu.com/gtwryuitsy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jqgufenzy.top/gtbhmysbsp.html

[S46] C++：函数模板
来源：http://hz.yj20258.top/gtsczcybku.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.cashguo.top/gtsddywweg.html

[S47] C++：结构化绑定遍历
来源：http://hz.tian-w.cn/gtvgdficsm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.quarkkingdee.top/gtfxefdtjs.html

[S48] C++：逐行读文件
来源：http://hz.xinyue.icu/gtefxtdsgw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.iojbl.cn/gtbfacsbvp.html

while (std::getline(in, line)) { }
来源：http://hz.iojbl.cn/gtpdmqtsui.html

[S49] C++：写文件
来源：http://hz.kuanghao11.cn/gtzveazyvx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zdqjudy.top/gtfjiqbfhm.html

[S50] C++：格式化数字
来源：http://hz.zhijiandao.cn/gtxrzpxgsi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hysaishi.cn/gtncigywyr.html

[S51] C++：显式类型转换
来源：http://hz.hfpthk.cn/gtrzwmwegu.html

static_cast<double>(a) / b
来源：http://hz.aibaodan.cn/gtplvjxjwd.html

[S52] C++：const 与 noexcept
来源：http://hz.nanxinkj.top/gtcimgjgca.html

int size() const noexcept { return n_; }
来源：http://hz.gotoacloud.top/gtawrergjr.html

[S53] C++：移动语义
来源：http://hz.fengsongda.top/gtuihmpiyv.html

std::vector<int> w = std::move(v);
来源：http://hz.nwbrower.top/gteazgibjf.html

[S54] C++：异常处理
来源：http://hz.jqgfzy.top/gtpfeydmro.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.0kj1m.cn/gthsxcqtwq.html

[S55] C++：结构化绑定
来源：http://hz.vqdsnc.cn/gtijwdvaro.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jianghu66.top/gtsmpwibbp.html

[S56] C++：optional
来源：http://hz.hywenlv.cn/gtsmeufqxf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yongpay.top/gtmcvgvwbk.html

[S57] C++：编译期常量
来源：http://hz.dashuyun.cn/gtkphoojfm.html

constexpr int N = 10;
来源：http://hz.dashuyun.cn/gtpuzaxvso.html

[S58] C++：命名空间
来源：http://hz.svipenyu.cn/gtecfahedf.html

namespace ns { int f() { return 1; } }
来源：http://hz.bjfxy.top/gtxgbswlxv.html

[S59] C++：静态断言
来源：http://hz.hysaishi.cn/gtyoyokckp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cashguo.top/gtwfyxqkzt.html

[S60] C++：遍历并删除元素
来源：http://hz.cdnleiting.top/gtlmalkxba.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhengqikj.top/gtiqiifomb.html

================================================================================
来源：http://hz.tianlin.xyz/gttkhvbpex.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cucudq.cn/gtjgahhjmu.html

================================================================================
来源：http://hz.tanke756.top/gtubfofzyg.html

[T01] Kotlin：Hello World
来源：http://hz.bjfxy.top/gtmmsyizzl.html

println("Hello")
来源：http://hz.jinyuanbaomall.cn/gterwrwnds.html

[T02] Kotlin：变量
来源：http://hz.guannengcc.top/gtgtxghytc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ivvv.top/gtmfujxoog.html

[T03] Kotlin：字符串模板
来源：http://hz.gogol.net.cn/gttecitlqp.html

"值: $b"
来源：http://hz.zycfv.cn/gtzhcndnqi.html

[T04] Kotlin：空安全
来源：http://hz.xuetiantiany.cn/gteilbhwyq.html

val n: String? = null;  n?.length
来源：http://hz.52xcode.cn/gtplmltdlz.html

[T05] Kotlin：when 表达式
来源：http://hz.9152youxi.cn/gtrrfgkquu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinqigufen.top/gtijkjomdn.html

[T06] Kotlin：集合映射
来源：http://hz.hfpthk.cn/gtnigusktc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hammf.cn/gtqxuczaxk.html

[T07] Kotlin：集合过滤
来源：http://hz.xuetiantiany.cn/gtzhapcohp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hnxiangtu.top/gtfwmxogow.html

[T08] Kotlin：数据类
来源：http://hz.jinqigufen.top/gtpvvbmmmo.html

data class User(val name: String, val age: Int)
来源：http://hz.cdnleiting.top/gtbjvbbneb.html

[T09] Kotlin：扩展函数
来源：http://hz.ywan-chungtsiang.top/gtsqbyxzcx.html

fun String.exclaim() = this + "!"
来源：http://hz.xinyue.icu/gtprtroecd.html

[T10] Kotlin：默认参数
来源：http://hz.feifeiyinyue.top/gtbgpvvpdx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zycfv.cn/gtfnxslyoe.html

[T11] Kotlin：协程
来源：http://hz.ybcxt.top/gtbnzcbeav.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xuetiantiany.cn/gtdmtzuitn.html

[T12] Kotlin：解构声明
来源：http://hz.gzhubu.top/gtkhgbnijh.html

val (a, b) = Pair(1, 2)
来源：http://hz.smart0.xyz/gtzpyctwvo.html

[T13] Kotlin：只读 Map
来源：http://hz.pengpengdd.cyou/gtveiypfwf.html

val m = mapOf("a" to 1)
来源：http://hz.316326.xyz/gtdkzkiukj.html

[T14] Kotlin：循环
来源：http://hz.jinqigufen.top/gtaqlaefdi.html

for (i in 1..10) println(i)
来源：http://hz.yangfankeji.com/gtjgbjvlgv.html

[T15] Kotlin：接口
来源：http://hz.meibo888.top/gtmipnqqbl.html

interface Shape { fun area(): Double }
来源：http://hz.316326.xyz/gtniciprwu.html

[T16] Swift：Hello World
来源：http://hz.xylfe.cn/gtjnyiwbys.html

print("Hello")
来源：http://hz.yonumen.top/gttfzcikrr.html

[T17] Swift：变量与常量
来源：http://hz.fzhhl.top/gtuxuzjuyr.html

var a = 1;  let b = 2
来源：http://hz.pycfn.com/gtzhoctheh.html

[T18] Swift：字符串插值
来源：http://hz.hongshengwenyu.top/gtyrjpsgee.html

"值: \(b)"
来源：http://hz.chenjidiqi.icu/gtwcryonsp.html

[T19] Swift：可选绑定
来源：http://hz.zhongyouzk.top/gthmgvzksz.html

if let n = opt { print(n) }
来源：http://hz.wangdashe.top/gtozbmqmmz.html

[T20] Swift：数组操作
来源：http://hz.yangfankeji.com/gtugofscxp.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yj20258888.top/gtovqaertv.html

[T21] Swift：遍历
来源：http://hz.shanyushiyangkeji.top/gtohqpkyfp.html

for x in a { print(x) }
来源：http://hz.316326.xyz/gtrzfuypbu.html

[T22] Swift：字典
来源：http://hz.316326.xyz/gtomkhubzr.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hywenlv.cn/gtnmptueqa.html

[T23] Swift：函数
来源：http://hz.xinyue.icu/gtgrpdxvfx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.dashuyun.cn/gttfdejrmr.html

[T24] Swift：闭包
来源：http://hz.birdmap.top/gtxtpbknpl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.mhx1999.top/gtilvheqbu.html

[T25] Swift：结构体
来源：http://hz.yuanzhike.top/gtowmygpxv.html

struct P { var x: Int }
来源：http://hz.tian-w.cn/gtphdjakiv.html

[T26] Swift：类与重写
来源：http://hz.shzxlz.cn/gtgtswovel.html

class A: Base { override func f() {} }
来源：http://hz.xuetiantiany.cn/gtvhuegukf.html

[T27] Swift：错误处理
来源：http://hz.hnxiangtu.top/gtfcgucmib.html

do { try f() } catch { print(error) }
来源：http://hz.aizwys.cn/gtxhtnafwe.html

[T28] Swift：枚举
来源：http://hz.havefunace.top/gtlaxwskiy.html

enum Color { case red, green }
来源：http://hz.jinqigufen.top/gtibcbtitb.html

[T29] Swift：guard 提前返回
来源：http://hz.meibo888.top/gtsmfbpqfg.html

guard let x = opt else { return }
来源：http://hz.sufxvd.cn/gtporqzdiy.html

[T30] Swift：协议
来源：http://hz.hnqzz.top/gtscmonpak.html

protocol Shape { func area() -> Double }
来源：http://hz.smart0.xyz/gtulyzcemp.html

[T31] Lua：Hello World
来源：http://hz.yueranfly.top/gtebuqhirb.html

print("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtzburnqsk.html

[T32] Lua：局部变量
来源：http://hz.meibo888.top/gtxghmqgmm.html

local a = 1
来源：http://hz.iojbl.cn/gtcihtkgeu.html

[T33] Lua：表（数组）
来源：http://hz.hnqzz.top/gtdrmwuviw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xuetiantiany.cn/gtnyigdtfu.html

[T34] Lua：遍历表
来源：http://hz.andypj.xyz/gtghyivqiv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.wangdashe.top/gtaqseceug.html

[T35] Lua：字典表
来源：http://hz.aizwys.cn/gtotuwdvdd.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hfpthk.cn/gtsxrvzzvr.html

[T36] Lua：函数
来源：http://hz.chenlongwang.top/gtqatiwmrq.html

function add(a, b) return a + b end
来源：http://hz.jqgufenzy.top/gtzsvfryte.html

[T37] Lua：字符串拼接
来源：http://hz.aibaodan.cn/gtyylkidso.html

"a" .. "b"
来源：http://hz.pycfn.com/gtqdfpevrz.html

[T38] Lua：条件
来源：http://hz.aibaodan.cn/gtgvenaxqf.html

if x > 0 then print("正") end
来源：http://hz.iojbl.cn/gtwaqjqznf.html

[T39] Lua：模式匹配
来源：http://hz.chenlongwang.top/gtkndmpirc.html

string.find(s, "%d+")
来源：http://hz.redwolf501.top/gtxwfovrsn.html

[T40] Lua：元表
来源：http://hz.xziqi.cn/gtqcgyuzhu.html

setmetatable({}, { __index = base })
来源：http://hz.ywan-chungtsiang.top/gtbhetlcwp.html

[T41] Perl：Hello World
来源：http://hz.bjfxy.top/gtwmghobjr.html

print "Hello\n";
来源：http://hz.shangyingyoupin.top/gtbwqpcbbj.html

[T42] Perl：变量类型
来源：http://hz.meibo888.top/gtopeixase.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.wangshuangyany.cn/gttiwfabhj.html

[T43] Perl：字符串插值
来源：http://hz.yonumen.top/gtkzbavtdv.html

"值: $a"
来源：http://hz.chenlongwang.top/gtmjjsihlg.html

[T44] Perl：条件
来源：http://hz.xinyue.icu/gtgopadilo.html

if ($a > 0) { print "正"; }
来源：http://hz.andypj.xyz/gtpffjmjlh.html


<!-- 参考信息 -->