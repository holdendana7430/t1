代发 wailian999

cmd >/dev/null 2>&1
来源：http://hz.jinqigufen.top/gtaajzfmpt.html

[R42] 输入重定向
来源：http://hz.sufxvd.cn/gtzuhswasa.html

wc -l < a.txt
来源：http://hz.316326.xyz/gtmdaftsda.html

[R43] 按名字查找文件
来源：http://hz.chenzaomai.com/gtdjhvveov.html

find . -name "*.log" -type f
来源：http://hz.daxiang520.top/gtwxsxubau.html

[R44] 按修改时间查找
来源：http://hz.yangfankeji.com/gtjskwlikj.html

find . -mtime -7 -type f
来源：http://hz.gaohongyu789.top/gthaezhyab.html

[R45] 批量删除
来源：http://hz.yangfankeji.com/gtbzybnurd.html

find . -name "*.tmp" -delete
来源：http://hz.tanke756.top/gtitczaneb.html

[R46] 递归替换文件内容
来源：http://hz.tanke756.top/gtmghmuduq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.kuanghao11.cn/gtayegfilv.html

[R47] sed 单行替换
来源：http://hz.dianchejie.cn/gtqcgajvfc.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yvedp.cn/gtqieobdbx.html

[R48] awk 取指定列
来源：http://hz.ydjk.org.cn/gthulozshw.html

awk '{print $1, $3}' a.txt
来源：http://hz.316326.xyz/gtmvartulq.html

[R49] awk 带条件
来源：http://hz.guannengcc.top/gtueugsytt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cqqwz.cn/gtfcmupwkn.html

[R50] awk 求和
来源：http://hz.zhengqikj.top/gteylommzu.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.smart0.xyz/gtqnyutykd.html

[R51] 排序去重取前几
来源：http://hz.jianghu66.top/gtoicmdmpq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.iojbl.cn/gttfzogeez.html

[R52] 统计行数
来源：http://hz.cqqwz.cn/gtzglweigy.html

wc -l a.txt
来源：http://hz.sweek.top/gtdjflmcrl.html

[R53] 查看文件头与实时尾
来源：http://hz.yuanzhike.top/gtgouesapg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.redwolf501.top/gtsvohgxkh.html

[R54] 比较两个文件
来源：http://hz.yanxiufei.cn/gtjcagkigt.html

diff a.txt b.txt
来源：http://hz.zhoulong.xyz/gtnxsobiwf.html

[R55] 压缩与解压
来源：http://hz.sufxvd.cn/gtbuhlnfws.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.havefunace.top/gthmmweqvf.html

[R56] 远程拷贝
来源：http://hz.yj202588.top/gttkdsthtx.html

scp file user@host:/path/
来源：http://hz.kuanghao11.cn/gtuqauflql.html

[R57] 远程执行命令
来源：http://hz.feifeiyinyue.top/gtmdjcqnpw.html

ssh user@host 'uptime'
来源：http://hz.cdnleiting.top/gtvepafqae.html

[R58] 下载文件
来源：http://hz.zhongyouzk.top/gtvoyijzif.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yangfankeji.com/gtnknseiav.html

[R59] 发 POST JSON
来源：http://hz.jianghu66.top/gttbuzradw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinyuanbaomall.cn/gtbajafmso.html

[R60] 只看 HTTP 状态码
来源：http://hz.gogol.net.cn/gtppdnfjvh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hfpthk.cn/gtdvjxlrev.html

[R61] 磁盘占用
来源：http://hz.zhongyouzk.top/gtcknmtnqy.html

df -h;  du -sh *
来源：http://hz.hnqzz.top/gtyxajeaxf.html

[R62] 找最占空间的文件
来源：http://hz.316326.xyz/gtzgkufegk.html

du -ah . | sort -rh | head -10
来源：http://hz.zhixingplan.top/gtylpnhjjw.html

[R63] 内存与进程
来源：http://hz.smart0.xyz/gtfmcxzngn.html

free -h;  ps aux | grep nginx
来源：http://hz.yj20258888.top/gtyfwnpibc.html

[R64] 结束进程
来源：http://hz.cucudq.cn/gtxxdsqpmp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.dashuyun.cn/gtbuxzbioj.html

[R65] 查看端口占用
来源：http://hz.quarkkingdee.top/gtdwrjcycf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hysaishi.cn/gtmuibwfzv.html

[R66] 定时任务
来源：http://hz.feifeiyinyue.top/gttdvmbmfc.html

crontab -e;  crontab -l
来源：http://hz.pycfn.com/gtacfuelep.html

[R67] 生成随机十六进制串
来源：http://hz.yonumen.top/gtmsyzbptk.html

openssl rand -hex 16
来源：http://hz.ppjwa.cn/gtwmixbhnv.html

[R68] 计算文件校验值
来源：http://hz.pycfn.com/gtsgdnpvjj.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.chenzaomai.com/gtttnfhyfi.html

[R69] 生成随机密码
来源：http://hz.jlsjyb.cn/gtxyginvrx.html

head -c 16 /dev/urandom | base64
来源：http://hz.svipenyu.cn/gtxvuiaipk.html

[R70] 时间戳与互转
来源：http://hz.ivvv.top/gttkuejxrm.html

date +%s;  date -d @1700000000
来源：http://hz.yj20258.top/gtuutqzsgr.html

[R71] 日期格式化
来源：http://hz.hongshengwenyu.top/gtbpqmkpoz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.andypj.xyz/gthhakmnke.html

[R72] 等待端口就绪
来源：http://hz.yuanzhike.top/gtjotonmxe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.bjfxy.top/gtzcwwvlyp.html

[R73] 分割大日志
来源：http://hz.ivvv.top/gtgoqeqzdq.html

split -l 1000 big.log part_
来源：http://hz.smart0.xyz/gtdtizsesq.html

[R74] 批量重命名
来源：http://hz.pycfn.com/gtgikuuofl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jqgufenzy.top/gtsriogyjw.html

[R75] 导出环境变量
来源：http://hz.nanxuanxn.top/gtlvlekxww.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jianghu66.top/gtruiijoto.html

[R76] 使用临时文件
来源：http://hz.zhiwuduotai.top/gttnnjucah.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangtech.top/gtslpwbkaf.html

[R77] 读取用户输入
来源：http://hz.jinqigufen.top/gtlvkogotk.html

read -rp "请输入: " ans
来源：http://hz.guannengcc.top/gtfrfzoztb.html

[R78] 交互式菜单
来源：http://hz.shzxlz.cn/gtbrlcirhz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhiwuduotai.top/gtkeichrmh.html

[R79] 解析命令行选项
来源：http://hz.shzxlz.cn/gtsqdphnnj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ybcxt.top/gtjkbdatgh.html

[R80] 查看脚本执行耗时
来源：http://hz.yj20258.top/gtmvhliwao.html

time ./run.sh
来源：http://hz.jqgufenzy.top/gtolifhxql.html

================================================================================
来源：http://hz.fengsongda.top/gtslbtmkzg.html

S. C / C++ 专题
来源：http://hz.quarkkingdee.top/gtwhxbkhbt.html

================================================================================
来源：http://hz.sysykeji.top/gtdelftqvc.html

[S01] C：Hello World
来源：http://hz.smart0.xyz/gtglerijhx.html

#include <stdio.h>
来源：http://hz.316326.xyz/gtjjrslapa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xziqi.cn/gteiwdtamv.html

[S02] C：变量与格式化输出
来源：http://hz.sxryk.cn/gtutluxjua.html

int a = 10; printf("%d\n", a);
来源：http://hz.cqqwz.cn/gtbuimyvwg.html

[S03] C：读入整数
来源：http://hz.ppjwa.cn/gtlsgaakyi.html

int x; scanf("%d", &x);
来源：http://hz.hnqzz.top/gtcpsvfjgw.html

[S04] C：字符串复制
来源：http://hz.pengpengdd.cyou/gtsazwvurt.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.daria6918.cn/gtycwwmayr.html

[S05] C：字符串长度
来源：http://hz.hywenlv.cn/gtozxoijpc.html

strlen(s)
来源：http://hz.haohaochexian.top/gtepcataem.html

[S06] C：字符串比较
来源：http://hz.bjfxy.top/gtoiyirvax.html

strcmp(a, b) == 0
来源：http://hz.ivvv.top/gtccojyzlg.html

[S07] C：数组遍历求和
来源：http://hz.zhaomingkeji.xyz/gtbkdsasgu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.havefunace.top/gtacbpswjz.html

[S08] C：动态内存分配与释放
来源：http://hz.xingfuxueyuan.xyz/gtdmprkujo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.316326.xyz/gtxmqzqknd.html

[S09] C：结构体定义与初始化
来源：http://hz.jinqigufen.top/gtbpveuuhk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shangyingyoupin.top/gtsrxjerrk.html

[S10] C：指针与解引用
来源：http://hz.guowangkeji.top/gtjbkhywfi.html

int *p = &a;  *p = 5;
来源：http://hz.hywenlv.cn/gtakrznurp.html

[S11] C：逐行读文件
来源：http://hz.sxryk.cn/gtpiuigcdq.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cheryme.top/gttvklewqj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gaohongyu789.top/gtzwwkebes.html

fclose(f);
来源：http://hz.shzxlz.cn/gtryoqonqc.html

[S12] C：写文件
来源：http://hz.jyoumei.cn/gttckysbos.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.havefunace.top/gtoyddtwfv.html

[S13] C：宏定义
来源：http://hz.aizwys.cn/gtjvwocqea.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.wangdashe.top/gtjvqitskv.html

[S14] C：枚举
来源：http://hz.hongshengwenyu.top/gtmyodixsg.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.0kj1m.cn/gtfrlrzxoi.html

[S15] C：类型转换
来源：http://hz.wangdashe.top/gtyvkgryyd.html

(double) a / b
来源：http://hz.zdqjudy.top/gtmescxvns.html

[S16] C：位操作置位
来源：http://hz.zhixingplan.top/gtneoorgas.html

x |= (1 << 3);
来源：http://hz.nanxuanxn.top/gtwinlqflg.html

[S17] C：安全拼接字符串
来源：http://hz.quarkkingdee.top/gtbiwzwoov.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yuanzhike.top/gthhgzsujz.html

[S18] C：命令行参数
来源：http://hz.gzhubu.top/gtueaprbbt.html

int main(int argc, char **argv)
来源：http://hz.aizwys.cn/gtzhztlvaw.html

[S19] C：快速排序
来源：http://hz.aibaodan.cn/gtygndrnzs.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.pycfn.com/gtwgvdkffa.html

[S20] C：二分查找
来源：http://hz.jiagoushi.top/gtoiyrsjvl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hongshengwenyu.top/gtxgbotjho.html

[S21] C：字符类别判断
来源：http://hz.zycfv.cn/gtzobpvlbn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.daria6918.cn/gtsqinflkv.html

[S22] C：字符串转数字
来源：http://hz.316326.xyz/gthdycdqil.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.wangshuangyany.cn/gtimnlzfzu.html

[S23] C：随机数
来源：http://hz.aibaodan.cn/gtnpfepkmd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.nwbrower.top/gtozeeycgz.html

[S24] C：获取本地时间
来源：http://hz.cdnleiting.top/gtxziruewn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ydzc1.top/gtuaxzhtkl.html

[S25] C：内存拷贝
来源：http://hz.ybcxt.top/gtjbhclqtg.html

memcpy(dst, src, n);
来源：http://hz.shangyingyoupin.top/gttuhfwics.html

[S26] C：内存清零
来源：http://hz.cdnleiting.top/gtlrbumpym.html

memset(a, 0, sizeof a);
来源：http://hz.fengsongda.top/gtcwslbkao.html

[S27] C：定义常量
来源：http://hz.chenjidiqi.icu/gtowjbhmnt.html

const double PI = 3.14159;
来源：http://hz.yuxming.cn/gtxrypqkcp.html

[S28] C：静态变量
来源：http://hz.jlsjyb.cn/gttzknzxuj.html

static int counter = 0;
来源：http://hz.tianlin.xyz/gtddktyumm.html

[S29] C：变参函数
来源：http://hz.nanxinkj.top/gtavjzgzvi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zdqjudy.top/gtiwoiwhcm.html

[S30] C：头文件保护
来源：http://hz.pengpengdd.cyou/gtqjbarrhf.html

#ifndef X_H
来源：http://hz.zhiwuduotai.top/gtmpqjodyh.html

#define X_H
来源：http://hz.feifeiyinyue.top/gtqkshfuqv.html

#endif
来源：http://hz.yangfankeji.com/gtnfranxno.html

[S31] C++：Hello World
来源：http://hz.xziqi.cn/gtkygwhgqb.html

#include <iostream>
来源：http://hz.cqqwz.cn/gtmbeneisq.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cdnleiting.top/gtpdarqwra.html

[S32] C++：字符串
来源：http://hz.cashguo.top/gtpqoyenmk.html

std::string s = "hi";  s += "!";
来源：http://hz.xinyue.icu/gtxzmmwjkz.html

[S33] C++：vector 增删
来源：http://hz.sysykeji.top/gtviuxyifl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xuanzx.com/gtgltymxds.html

[S34] C++：遍历 vector
来源：http://hz.sweek.top/gtmwluexvk.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xziqi.cn/gtfpobjccz.html

[S35] C++：map
来源：http://hz.ppjwa.cn/gtzxwrzkfh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhongyouzk.top/gtrpppvacb.html

[S36] C++：unordered_map
来源：http://hz.smart0.xyz/gthmkyqlbh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnqzz.top/gtyrwurvyz.html

[S37] C++：set
来源：http://hz.birdmap.top/gtqjdfnxst.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.pycfn.com/gtpyeyaugy.html

[S38] C++：排序
来源：http://hz.ydjk.org.cn/gtsidnfygs.html

std::sort(v.begin(), v.end());
来源：http://hz.yuanzhike.top/gthdqfqtib.html

[S39] C++：自定义比较器排序
来源：http://hz.yj20258.top/gtuijbbauq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.bjfxy.top/gtxnrdunjz.html

[S40] C++：查找元素
来源：http://hz.hnxiangtu.top/gtltvtpsux.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.bjfxy.top/gtsrlrpter.html

[S41] C++：类与构造函数
来源：http://hz.ydzc1.top/gtenkmhohz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.haohaochexian.top/gtpofvyucl.html

[S42] C++：继承与虚函数
来源：http://hz.yuanzhike.top/gtndwvrmpe.html

class B : public Base { public: void f() override {} };
来源：http://hz.tanke756.top/gtsmslzfck.html

[S43] C++：智能指针
来源：http://hz.fengsongda.top/gtubfpdwmi.html

auto p = std::make_unique<int>(5);
来源：http://hz.dianchejie.cn/gtluaqfomd.html

[S44] C++：引用传参
来源：http://hz.ydzc1.top/gtltrbelri.html

void inc(int &x) { ++x; }
来源：http://hz.zycfv.cn/gthbfocoez.html

[S45] C++：lambda
来源：http://hz.52xcode.cn/gtjuqxlqut.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nanxuanxn.top/gtlakotjho.html

[S46] C++：函数模板
来源：http://hz.ydjk.org.cn/gtwbdtptjm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jlsjyb.cn/gtlvtvsuso.html

[S47] C++：结构化绑定遍历
来源：http://hz.jyoumei.cn/gtplnhzftz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sufxvd.cn/gteryzlslm.html

[S48] C++：逐行读文件
来源：http://hz.tianlin.xyz/gtqhrdrpyq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhoulong.xyz/gtdafboszq.html

while (std::getline(in, line)) { }
来源：http://hz.yanxiufei.cn/gtmfwcfodz.html

[S49] C++：写文件
来源：http://hz.zhiwuduotai.top/gtghykplze.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shangyingyoupin.top/gtjhdonfcq.html

[S50] C++：格式化数字
来源：http://hz.nwbrower.top/gttfeskjrj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yongpay.top/gtipldiwky.html

[S51] C++：显式类型转换
来源：http://hz.316326.xyz/gtrjlgekgo.html

static_cast<double>(a) / b
来源：http://hz.shanyushiyangtech.top/gtqviehvwh.html

[S52] C++：const 与 noexcept
来源：http://hz.tian-w.cn/gthrkdsigl.html

int size() const noexcept { return n_; }
来源：http://hz.316326.xyz/gtugmjffxz.html

[S53] C++：移动语义
来源：http://hz.yongpay.top/gtnmtkffhj.html

std::vector<int> w = std::move(v);
来源：http://hz.kuanghao11.cn/gttyjcqudd.html

[S54] C++：异常处理
来源：http://hz.yangfankeji.com/gtgghhgjxv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.chenlongwang.top/gtorsstvwz.html

[S55] C++：结构化绑定
来源：http://hz.jinqigfzy.top/gteohibygs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.mhx1999.top/gtnwjbangq.html

[S56] C++：optional
来源：http://hz.shanyushiyangtech.top/gtaonmtnej.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.aibaodan.cn/gtqwgooiti.html

[S57] C++：编译期常量
来源：http://hz.ywan-chungtsiang.top/gtuqlwuqvt.html

constexpr int N = 10;
来源：http://hz.zhoulong.xyz/gtguiiobzv.html

[S58] C++：命名空间
来源：http://hz.cqqwz.cn/gtcodlqdax.html

namespace ns { int f() { return 1; } }
来源：http://hz.fzhhl.top/gtbpuwilim.html

[S59] C++：静态断言
来源：http://hz.yangfankeji.com/gtgbgqncij.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hnqzz.top/gttyugjcrb.html

[S60] C++：遍历并删除元素
来源：http://hz.ybcxt.top/gtjqbftvsi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jianghu66.top/gtkbleuoyu.html

================================================================================
来源：http://hz.yj202588.top/gtsqwjrxrf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.andypj.xyz/gtlskksxyx.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gttvaeukie.html

[T01] Kotlin：Hello World
来源：http://hz.xinyue.icu/gtbgctwwrg.html

println("Hello")
来源：http://hz.xuetiantiany.cn/gtlyczelnp.html

[T02] Kotlin：变量
来源：http://hz.pengpengdd.cyou/gtngzdfmse.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jqgfzy.top/gtyxxarytu.html

[T03] Kotlin：字符串模板
来源：http://hz.ywan-chungtsiang.top/gtiurqpcur.html

"值: $b"
来源：http://hz.gogol.net.cn/gtppvajtyv.html

[T04] Kotlin：空安全
来源：http://hz.ybcxt.top/gtdwzadlyt.html

val n: String? = null;  n?.length
来源：http://hz.yj20258.top/gtlcyqidnx.html

[T05] Kotlin：when 表达式
来源：http://hz.ywan-chungtsiang.top/gtwsfepbbs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhongyouzk.top/gtqhemvbfn.html

[T06] Kotlin：集合映射
来源：http://hz.yj20258888.top/gteyhbbptt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jlsjyb.cn/gtojsrdauc.html

[T07] Kotlin：集合过滤
来源：http://hz.yvedp.cn/gtgdaontfc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.bjfxy.top/gtbhrvidvp.html

[T08] Kotlin：数据类
来源：http://hz.nanxuanxn.top/gtvclpofnl.html

data class User(val name: String, val age: Int)
来源：http://hz.daxiang520.top/gtwbdilutx.html

[T09] Kotlin：扩展函数
来源：http://hz.hnqzz.top/gtrtsnplat.html

fun String.exclaim() = this + "!"
来源：http://hz.bjfxy.top/gtntawttfn.html

[T10] Kotlin：默认参数
来源：http://hz.feifeiyinyue.top/gthzjiwphs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yvedp.cn/gtqpfvgnuc.html

[T11] Kotlin：协程
来源：http://hz.xuetiantiany.cn/gtmatainyq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.sxryk.cn/gtzxghmdlf.html

[T12] Kotlin：解构声明
来源：http://hz.shanyushiyangtech.top/gtiqupetgl.html

val (a, b) = Pair(1, 2)
来源：http://hz.jiagoushi.top/gtqemtottx.html

[T13] Kotlin：只读 Map
来源：http://hz.yangfankeji.com/gtxbgnjfof.html

val m = mapOf("a" to 1)
来源：http://hz.gogol.net.cn/gtfqxzqwle.html

[T14] Kotlin：循环
来源：http://hz.kuanghao11.cn/gtztyfprtc.html

for (i in 1..10) println(i)
来源：http://hz.iojbl.cn/gtukhnhyxc.html

[T15] Kotlin：接口
来源：http://hz.jiagoushi.top/gtznrhkgyb.html

interface Shape { fun area(): Double }
来源：http://hz.xingfuxueyuan.xyz/gtimnllpvd.html

[T16] Swift：Hello World
来源：http://hz.chenzaomai.com/gtwxktkglh.html

print("Hello")
来源：http://hz.haohaochexian.top/gtjazjqvvu.html

[T17] Swift：变量与常量
来源：http://hz.dashuyun.cn/gtsxhiopxc.html

var a = 1;  let b = 2
来源：http://hz.jianghu66.top/gtwparecqj.html

[T18] Swift：字符串插值
来源：http://hz.jinghuilouyu.cn/gtodhkuaoj.html

"值: \(b)"
来源：http://hz.hongshengwenyu.top/gtfwyealey.html

[T19] Swift：可选绑定
来源：http://hz.zhoulong.xyz/gtsfmuergj.html

if let n = opt { print(n) }
来源：http://hz.jyoumei.cn/gtzwneklay.html

[T20] Swift：数组操作
来源：http://hz.meibo888.top/gtqakgjbrx.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yueranfly.top/gtzpulfzqy.html

[T21] Swift：遍历
来源：http://hz.dashuyun.cn/gtpffpxjfx.html

for x in a { print(x) }
来源：http://hz.yueranfly.top/gtqrvyeigs.html

[T22] Swift：字典
来源：http://hz.jqgfzy.top/gtmdfczsbd.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yj20258.top/gtaqlddxxm.html

[T23] Swift：函数
来源：http://hz.gogol.net.cn/gtzcwdzizj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.havefunace.top/gtqfyzetgf.html

[T24] Swift：闭包
来源：http://hz.jinghuilouyu.cn/gtcwvmfghe.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.gzhubu.top/gtflqpblug.html

[T25] Swift：结构体
来源：http://hz.zdqjudy.top/gttggcjlgr.html

struct P { var x: Int }
来源：http://hz.chenjidiqi.icu/gtgsbukswm.html

[T26] Swift：类与重写
来源：http://hz.ydzc1.top/gtdxnatisu.html

class A: Base { override func f() {} }
来源：http://hz.nwbrower.top/gtkkbjnyka.html

[T27] Swift：错误处理
来源：http://hz.zhengqikj.top/gtycqeghna.html

do { try f() } catch { print(error) }
来源：http://hz.jyoumei.cn/gtgbkzalvk.html

[T28] Swift：枚举
来源：http://hz.ppjwa.cn/gtkxksaxud.html

enum Color { case red, green }
来源：http://hz.daria6918.cn/gtxajwjhql.html

[T29] Swift：guard 提前返回
来源：http://hz.quarkkingdee.top/gtjoabwbrj.html

guard let x = opt else { return }
来源：http://hz.aizwys.cn/gtdyjuytmq.html

[T30] Swift：协议
来源：http://hz.chenjidiqi.icu/gtarzlelat.html

protocol Shape { func area() -> Double }
来源：http://hz.shzxlz.cn/gtarubajar.html

[T31] Lua：Hello World
来源：http://hz.xinyue.icu/gtifdpykcu.html

print("Hello")
来源：http://hz.daxiang520.top/gtspmeiqie.html

[T32] Lua：局部变量
来源：http://hz.cucudq.cn/gtxctvssxm.html

local a = 1
来源：http://hz.jyoumei.cn/gtziyteols.html

[T33] Lua：表（数组）
来源：http://hz.nanxinkj.top/gtrsnmuaso.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xuanzx.com/gtroyxhmpm.html

[T34] Lua：遍历表
来源：http://hz.gotoacloud.top/gtktbbbppq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.nwbrower.top/gtgjvuplyl.html

[T35] Lua：字典表
来源：http://hz.sufxvd.cn/gtikvhzifq.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhengqikj.top/gtzmiseyji.html

[T36] Lua：函数
来源：http://hz.nwbrower.top/gtimhtihba.html

function add(a, b) return a + b end
来源：http://hz.cqqwz.cn/gtqizdytbs.html

[T37] Lua：字符串拼接
来源：http://hz.tianlin.xyz/gtaiiyztzi.html

"a" .. "b"
来源：http://hz.sweek.top/gtwnkicovz.html

[T38] Lua：条件
来源：http://hz.hammf.cn/gthftqvkry.html

if x > 0 then print("正") end
来源：http://hz.yj20258.top/gtxlljppxc.html

[T39] Lua：模式匹配
来源：http://hz.yuxming.cn/gtrpqjwjyc.html

string.find(s, "%d+")
来源：http://hz.hnqzz.top/gtlkrfmjdz.html

[T40] Lua：元表
来源：http://hz.sxryk.cn/gtjegnmwzc.html

setmetatable({}, { __index = base })
来源：http://hz.jiagoushi.top/gtvuwrzjvi.html

[T41] Perl：Hello World
来源：http://hz.yongpay.top/gtiwlnnvmt.html

print "Hello\n";
来源：http://hz.yj20258888.top/gtzlufhpkq.html

[T42] Perl：变量类型
来源：http://hz.cqqwz.cn/gterpgmtak.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.nanxuanxn.top/gtlehbpuxb.html

[T43] Perl：字符串插值
来源：http://hz.svipenyu.cn/gtopzhztqw.html

"值: $a"
来源：http://hz.bjfxy.top/gtjkpbszki.html

[T44] Perl：条件
来源：http://hz.yangfankeji.com/gteuzkfxyj.html

if ($a > 0) { print "正"; }
来源：http://hz.yonumen.top/gtnpbgkfng.html


<!-- 参考信息 -->