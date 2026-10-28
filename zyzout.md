代发 wailian999

files=$(ls -1)
来源：http://hz.yuanzhike.top/gttdqeiani.html

[R38] 管道串联
来源：http://hz.guannengcc.top/gtzcrutcxp.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhengqikj.top/gtqzyhppuv.html

[R39] 重定向标准输出与错误
来源：http://hz.gogol.net.cn/gtxcvmvmmh.html

cmd > out.log 2>&1
来源：http://hz.chenjidiqi.icu/gtgkxnjfog.html

[R40] 追加写日志
来源：http://hz.hongshengwenyu.top/gtqfvmphxi.html

echo "log" >> out.log
来源：http://hz.redwolf501.top/gtizkohopn.html

[R41] 丢弃输出
来源：http://hz.cucudq.cn/gtoscflsxa.html

cmd >/dev/null 2>&1
来源：http://hz.gzhubu.top/gtnqqoowsq.html

[R42] 输入重定向
来源：http://hz.gotoacloud.top/gtagrdznrd.html

wc -l < a.txt
来源：http://hz.zhengqikj.top/gtcprryfjt.html

[R43] 按名字查找文件
来源：http://hz.yongpay.top/gtbwolccjv.html

find . -name "*.log" -type f
来源：http://hz.ydzc1.top/gtfakjonkp.html

[R44] 按修改时间查找
来源：http://hz.tanke756.top/gtgyktfpmu.html

find . -mtime -7 -type f
来源：http://hz.nanxinkj.top/gtdnylvjdz.html

[R45] 批量删除
来源：http://hz.nwbrower.top/gtwrulylvu.html

find . -name "*.tmp" -delete
来源：http://hz.wangshuangyany.cn/gtyntndxwm.html

[R46] 递归替换文件内容
来源：http://hz.yuanzhike.top/gtgumitfpm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xylfe.cn/gtwxkjdimy.html

[R47] sed 单行替换
来源：http://hz.yonumen.top/gtxijcxpik.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yj20258888.top/gttyoprzio.html

[R48] awk 取指定列
来源：http://hz.sxryk.cn/gtsbokfnvq.html

awk '{print $1, $3}' a.txt
来源：http://hz.xziqi.cn/gtjcifuzlj.html

[R49] awk 带条件
来源：http://hz.yj20258.top/gtuwgtbnlj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cqqwz.cn/gtdhdepqko.html

[R50] awk 求和
来源：http://hz.shangyingyoupin.top/gtspiawmoj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhijiandao.cn/gtebaoenzg.html

[R51] 排序去重取前几
来源：http://hz.sysykeji.top/gtgnbpazke.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.redwolf501.top/gtdcktpsoc.html

[R52] 统计行数
来源：http://hz.xuetiantiany.cn/gtwatpgndi.html

wc -l a.txt
来源：http://hz.yueranfly.top/gtxyrylgiu.html

[R53] 查看文件头与实时尾
来源：http://hz.shanyushiyangtech.top/gtnlgnqvih.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cqqwz.cn/gtnqxjwzof.html

[R54] 比较两个文件
来源：http://hz.yangfankeji.com/gteckudjxm.html

diff a.txt b.txt
来源：http://hz.zhiwuduotai.top/gtfinyzhbw.html

[R55] 压缩与解压
来源：http://hz.meibo888.top/gtbqnvcqsu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinqigfzy.top/gtfbkxkvot.html

[R56] 远程拷贝
来源：http://hz.cucudq.cn/gtmhdkzqrq.html

scp file user@host:/path/
来源：http://hz.jinqigfzy.top/gtcfvuamcm.html

[R57] 远程执行命令
来源：http://hz.sysykeji.top/gthqcclvxp.html

ssh user@host 'uptime'
来源：http://hz.aizwys.cn/gtogtonuya.html

[R58] 下载文件
来源：http://hz.chenlongwang.top/gtbtmrgykf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.nanxuanxn.top/gtxqhvrion.html

[R59] 发 POST JSON
来源：http://hz.nanxuanxn.top/gthpuvsyom.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hnqzz.top/gtfyrxgivn.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhijiandao.cn/gtucsbbqbb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xziqi.cn/gtvylirfle.html

[R61] 磁盘占用
来源：http://hz.yueranfly.top/gtnugpbbtw.html

df -h;  du -sh *
来源：http://hz.yongpay.top/gtyzgplbwy.html

[R62] 找最占空间的文件
来源：http://hz.jinqigfzy.top/gtjzdjvqhk.html

du -ah . | sort -rh | head -10
来源：http://hz.guannengcc.top/gturzdwgvr.html

[R63] 内存与进程
来源：http://hz.jinyuanbaomall.cn/gtlcjedokr.html

free -h;  ps aux | grep nginx
来源：http://hz.yvedp.cn/gtogpnjqkz.html

[R64] 结束进程
来源：http://hz.yanxiufei.cn/gtpjwnxpwc.html

kill -9 $(pgrep -f app.py)
来源：http://hz.snrcjt.cn/gthptfqlws.html

[R65] 查看端口占用
来源：http://hz.jyoumei.cn/gtjytieaxw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zycfv.cn/gtrijsemxn.html

[R66] 定时任务
来源：http://hz.ydjk.org.cn/gtfuyragym.html

crontab -e;  crontab -l
来源：http://hz.daxiang520.top/gtjjjyznaa.html

[R67] 生成随机十六进制串
来源：http://hz.guowangkeji.top/gtggilcvik.html

openssl rand -hex 16
来源：http://hz.aibaodan.cn/gtxievpnvh.html

[R68] 计算文件校验值
来源：http://hz.zhengqikj.top/gtirblqxtk.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.guannengcc.top/gtatqwgafh.html

[R69] 生成随机密码
来源：http://hz.jianghu66.top/gtuzuhqpae.html

head -c 16 /dev/urandom | base64
来源：http://hz.yongpay.top/gtyxstyidy.html

[R70] 时间戳与互转
来源：http://hz.hysaishi.cn/gtiuakqmdp.html

date +%s;  date -d @1700000000
来源：http://hz.shanyushiyangkeji.top/gtwladaucw.html

[R71] 日期格式化
来源：http://hz.hammf.cn/gtjlvzdpht.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhaomingkeji.xyz/gtaqhrfeub.html

[R72] 等待端口就绪
来源：http://hz.zdqjudy.top/gtkdkrerdj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ivvv.top/gtamxiovwl.html

[R73] 分割大日志
来源：http://hz.wangdashe.top/gtkyftmrrc.html

split -l 1000 big.log part_
来源：http://hz.cqqwz.cn/gtkvykbyab.html

[R74] 批量重命名
来源：http://hz.zycfv.cn/gtisgoywdi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.0kj1m.cn/gtvymieqgk.html

[R75] 导出环境变量
来源：http://hz.gogol.net.cn/gtnafpucyf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.daria6918.cn/gthibwdfgg.html

[R76] 使用临时文件
来源：http://hz.cheryme.top/gthdldsrjf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigufen.top/gtosxjoctz.html

[R77] 读取用户输入
来源：http://hz.pycfn.com/gtlgtigdrf.html

read -rp "请输入: " ans
来源：http://hz.jinyuanbaomall.cn/gtppiiarav.html

[R78] 交互式菜单
来源：http://hz.yanxiufei.cn/gttalqlwvd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.wangshuangyany.cn/gtipuyawxt.html

[R79] 解析命令行选项
来源：http://hz.cheryme.top/gtkshhrpvq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xziqi.cn/gtemggtkqb.html

[R80] 查看脚本执行耗时
来源：http://hz.nanxuanxn.top/gtldvedfkg.html

time ./run.sh
来源：http://hz.quarkkingdee.top/gtyiuiucvg.html

================================================================================
来源：http://hz.bjfxy.top/gtgiddfbnz.html

S. C / C++ 专题
来源：http://hz.havefunace.top/gtcgbxlexj.html

================================================================================
来源：http://hz.cdnleiting.top/gtqbcmmeah.html

[S01] C：Hello World
来源：http://hz.xuanzx.com/gtftqgrlbi.html

#include <stdio.h>
来源：http://hz.zhiwuduotai.top/gtrntnpqsk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.vqdsnc.cn/gthjywibna.html

[S02] C：变量与格式化输出
来源：http://hz.hywenlv.cn/gtesaglege.html

int a = 10; printf("%d\n", a);
来源：http://hz.ydzc1.top/gtucujnuha.html

[S03] C：读入整数
来源：http://hz.yangfankeji.com/gtczlanxkm.html

int x; scanf("%d", &x);
来源：http://hz.vqdsnc.cn/gtahuxunhd.html

[S04] C：字符串复制
来源：http://hz.c1oappe.top/gtfwljlgre.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhixingplan.top/gtialqfdsh.html

[S05] C：字符串长度
来源：http://hz.gotoacloud.top/gtlytfocux.html

strlen(s)
来源：http://hz.pycfn.com/gtogrbtgfk.html

[S06] C：字符串比较
来源：http://hz.jiagoushi.top/gtnhzkftoh.html

strcmp(a, b) == 0
来源：http://hz.zhoulong.xyz/gtctookrgq.html

[S07] C：数组遍历求和
来源：http://hz.wangshuangyany.cn/gtxxruxhox.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ybcxt.top/gtvjsnoxde.html

[S08] C：动态内存分配与释放
来源：http://hz.sysykeji.top/gtqwmjfguh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.iojbl.cn/gtioeaudlu.html

[S09] C：结构体定义与初始化
来源：http://hz.tian-w.cn/gttirvfwkw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.chenzaomai.com/gtkpotxoee.html

[S10] C：指针与解引用
来源：http://hz.havefunace.top/gtxejlwtue.html

int *p = &a;  *p = 5;
来源：http://hz.zhengqikj.top/gtchonzrfh.html

[S11] C：逐行读文件
来源：http://hz.ydjk.org.cn/gtunpowzoe.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yj20258.top/gtysyymubj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.dianchejie.cn/gtfzfkqnlr.html

fclose(f);
来源：http://hz.jianghu66.top/gtygvrwewz.html

[S12] C：写文件
来源：http://hz.meibo888.top/gtwcbenzrp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinqigfzy.top/gtehvticpu.html

[S13] C：宏定义
来源：http://hz.ybcxt.top/gthdbdqnys.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.tian-w.cn/gtsyevgxvv.html

[S14] C：枚举
来源：http://hz.jyoumei.cn/gtrqaugvsf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.iojbl.cn/gtnqmtzplm.html

[S15] C：类型转换
来源：http://hz.nanxinkj.top/gtjxbbmssz.html

(double) a / b
来源：http://hz.yj20258.top/gtdazdgvte.html

[S16] C：位操作置位
来源：http://hz.jinghuilouyu.cn/gtkvydmhbn.html

x |= (1 << 3);
来源：http://hz.xinyue.icu/gthsklssil.html

[S17] C：安全拼接字符串
来源：http://hz.jianghu66.top/gtfnbxmadf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yj20258888.top/gtesazznzt.html

[S18] C：命令行参数
来源：http://hz.cashguo.top/gtocfzodqx.html

int main(int argc, char **argv)
来源：http://hz.ydjk.org.cn/gtcdzluaam.html

[S19] C：快速排序
来源：http://hz.wangshuangyany.cn/gtuyuxorjt.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.chenzaomai.com/gtnzdqzyif.html

[S20] C：二分查找
来源：http://hz.cucudq.cn/gtfkhbdama.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yangfankeji.com/gtoznjvvul.html

[S21] C：字符类别判断
来源：http://hz.yongpay.top/gtziivvxhn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.daria6918.cn/gtminxkxei.html

[S22] C：字符串转数字
来源：http://hz.zhoulong.xyz/gtmtxevibj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jinqigfzy.top/gtgcyayeff.html

[S23] C：随机数
来源：http://hz.snrcjt.cn/gtxvgczjlm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.guannengcc.top/gtuhoimaaj.html

[S24] C：获取本地时间
来源：http://hz.aizwys.cn/gtctabmmrh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.svipenyu.cn/gttjkelacv.html

[S25] C：内存拷贝
来源：http://hz.hongshengwenyu.top/gtnwdefxke.html

memcpy(dst, src, n);
来源：http://hz.cashguo.top/gtuchukjky.html

[S26] C：内存清零
来源：http://hz.xingfuxueyuan.xyz/gtqrxlpymf.html

memset(a, 0, sizeof a);
来源：http://hz.yongpay.top/gtidjxfeqn.html

[S27] C：定义常量
来源：http://hz.fengsongda.top/gtehlzocce.html

const double PI = 3.14159;
来源：http://hz.cdnleiting.top/gtuwerkbcm.html

[S28] C：静态变量
来源：http://hz.chenlongwang.top/gttvukzreu.html

static int counter = 0;
来源：http://hz.cqqwz.cn/gtazyqbdqt.html

[S29] C：变参函数
来源：http://hz.ybcxt.top/gtkutvycsf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yuanzhike.top/gtpdtgtllg.html

[S30] C：头文件保护
来源：http://hz.shangyingyoupin.top/gtkxiruilt.html

#ifndef X_H
来源：http://hz.zhiwuduotai.top/gtxsbwxjgw.html

#define X_H
来源：http://hz.yongpay.top/gtlawmhjrh.html

#endif
来源：http://hz.guowangkeji.top/gtvalwypgc.html

[S31] C++：Hello World
来源：http://hz.quarkkingdee.top/gtvejtipxo.html

#include <iostream>
来源：http://hz.yanxiufei.cn/gtsblhdmjg.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.sxryk.cn/gtordigcwb.html

[S32] C++：字符串
来源：http://hz.havefunace.top/gtlomxepcd.html

std::string s = "hi";  s += "!";
来源：http://hz.ybcxt.top/gtlwhfgitl.html

[S33] C++：vector 增删
来源：http://hz.cashguo.top/gtwaezvhpj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yongpay.top/gtuuluqdyu.html

[S34] C++：遍历 vector
来源：http://hz.xuetiantiany.cn/gtvqrexcwb.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.fzhhl.top/gtbbjkhvwz.html

[S35] C++：map
来源：http://hz.jinqigfzy.top/gtznvumhcj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnqzz.top/gtawbwidzv.html

[S36] C++：unordered_map
来源：http://hz.fengsongda.top/gtselgbyxe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zycfv.cn/gtnbdmmoge.html

[S37] C++：set
来源：http://hz.wangdashe.top/gtagfairpi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.tanke756.top/gtnfyydfwo.html

[S38] C++：排序
来源：http://hz.hywenlv.cn/gttazfgpwx.html

std::sort(v.begin(), v.end());
来源：http://hz.jiagoushi.top/gtczpunsml.html

[S39] C++：自定义比较器排序
来源：http://hz.vqdsnc.cn/gtiukpyqjy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.bjfxy.top/gtjtijbvdz.html

[S40] C++：查找元素
来源：http://hz.dashuyun.cn/gtozvaqsob.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.sxryk.cn/gtrztufwgw.html

[S41] C++：类与构造函数
来源：http://hz.shanyushiyangtech.top/gtboiltaro.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gaohongyu789.top/gthmbuawfr.html

[S42] C++：继承与虚函数
来源：http://hz.zhijiandao.cn/gtrnwjrjex.html

class B : public Base { public: void f() override {} };
来源：http://hz.birdmap.top/gtklhjoxhi.html

[S43] C++：智能指针
来源：http://hz.bjfxy.top/gttlspzjgj.html

auto p = std::make_unique<int>(5);
来源：http://hz.gogol.net.cn/gtwelylklt.html

[S44] C++：引用传参
来源：http://hz.gzhubu.top/gtrhuyinga.html

void inc(int &x) { ++x; }
来源：http://hz.quarkkingdee.top/gtcmfuqslz.html

[S45] C++：lambda
来源：http://hz.0kj1m.cn/gtsxnuyuvw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.wangshuangyany.cn/gtzcfkkyei.html

[S46] C++：函数模板
来源：http://hz.bjfxy.top/gtdadjfkot.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yj202588.top/gtfudmkkhf.html

[S47] C++：结构化绑定遍历
来源：http://hz.cqqwz.cn/gtvtlyctzv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.fengsongda.top/gtnpqgzvqr.html

[S48] C++：逐行读文件
来源：http://hz.zhaomingkeji.xyz/gtqlsjleyt.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hywenlv.cn/gtrlpszrln.html

while (std::getline(in, line)) { }
来源：http://hz.xingfuxueyuan.xyz/gtqbzhhzvi.html

[S49] C++：写文件
来源：http://hz.yj202588.top/gtuvpwfuwf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jqgufenzy.top/gtilwiyiyz.html

[S50] C++：格式化数字
来源：http://hz.yuanzhike.top/gtvcigjpdw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shangyingyoupin.top/gtyykptzji.html

[S51] C++：显式类型转换
来源：http://hz.nwbrower.top/gtbptmujta.html

static_cast<double>(a) / b
来源：http://hz.316326.xyz/gtckhdaptp.html

[S52] C++：const 与 noexcept
来源：http://hz.snrcjt.cn/gtgfwravji.html

int size() const noexcept { return n_; }
来源：http://hz.bjfxy.top/gtdngujlvk.html

[S53] C++：移动语义
来源：http://hz.chenlongwang.top/gtfpvduchy.html

std::vector<int> w = std::move(v);
来源：http://hz.yuanzhike.top/gtgbhsdzbj.html

[S54] C++：异常处理
来源：http://hz.chenjidiqi.icu/gtlridwtbe.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.pycfn.com/gtndpjymnx.html

[S55] C++：结构化绑定
来源：http://hz.sweek.top/gtwheofyfb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhijiandao.cn/gtkvzxaveq.html

[S56] C++：optional
来源：http://hz.kuanghao11.cn/gttvmdhbqy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xinyue.icu/gtzfkbjbnq.html

[S57] C++：编译期常量
来源：http://hz.meibo888.top/gtucugbota.html

constexpr int N = 10;
来源：http://hz.nwbrower.top/gtscoyxocg.html

[S58] C++：命名空间
来源：http://hz.daria6918.cn/gtxesdleza.html

namespace ns { int f() { return 1; } }
来源：http://hz.dianchejie.cn/gtfgbkeuyv.html

[S59] C++：静态断言
来源：http://hz.yj20258.top/gtsycvwmtm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.fzhhl.top/gtneyapkzb.html

[S60] C++：遍历并删除元素
来源：http://hz.cqqwz.cn/gtzhjqixeo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.quarkkingdee.top/gtvgjrhphj.html

================================================================================
来源：http://hz.hongshengwenyu.top/gthyyndrbs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hongshengwenyu.top/gtjnmjjefj.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtycnhchbr.html

[T01] Kotlin：Hello World
来源：http://hz.hongshengwenyu.top/gttpzteurh.html

println("Hello")
来源：http://hz.cqqwz.cn/gtxaakcavl.html

[T02] Kotlin：变量
来源：http://hz.jianghu66.top/gtqahhfivo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.9152youxi.cn/gtzvtelswz.html

[T03] Kotlin：字符串模板
来源：http://hz.cheryme.top/gtzhaetosn.html

"值: $b"
来源：http://hz.birdmap.top/gtdzvlldwm.html

[T04] Kotlin：空安全
来源：http://hz.daria6918.cn/gtxvreneqo.html

val n: String? = null;  n?.length
来源：http://hz.ydjk.org.cn/gtuwwejppe.html

[T05] Kotlin：when 表达式
来源：http://hz.yj202588.top/gtagdybuce.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jyoumei.cn/gtswdtvdgn.html

[T06] Kotlin：集合映射
来源：http://hz.hammf.cn/gtunvlfkvt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zdqjudy.top/gtkykqbmfo.html

[T07] Kotlin：集合过滤
来源：http://hz.cheryme.top/gtaogknetm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cashguo.top/gtkwfuddce.html

[T08] Kotlin：数据类
来源：http://hz.wangshuangyany.cn/gthlqfihls.html

data class User(val name: String, val age: Int)
来源：http://hz.jqgfzy.top/gtztumumpw.html

[T09] Kotlin：扩展函数
来源：http://hz.cdnleiting.top/gtiurzpcup.html

fun String.exclaim() = this + "!"
来源：http://hz.sweek.top/gtovpgjggh.html

[T10] Kotlin：默认参数
来源：http://hz.iojbl.cn/gtzfintzqf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jqgfzy.top/gtfzmhhtkr.html

[T11] Kotlin：协程
来源：http://hz.wangdashe.top/gtlrdypnpm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.kuanghao11.cn/gtcsdevwyf.html

[T12] Kotlin：解构声明
来源：http://hz.jinqigufen.top/gttshbdvsy.html

val (a, b) = Pair(1, 2)
来源：http://hz.shuidangran.top/gtfdqibdpr.html

[T13] Kotlin：只读 Map
来源：http://hz.ehwqpu.com/gtlkxzimsg.html

val m = mapOf("a" to 1)
来源：http://hz.jqgufenzy.top/gtbqwbjrej.html

[T14] Kotlin：循环
来源：http://hz.jqgfzy.top/gtwvoimhmb.html

for (i in 1..10) println(i)
来源：http://hz.xuanzx.com/gtztsdigyu.html

[T15] Kotlin：接口
来源：http://hz.shangyingyoupin.top/gtkrhfuong.html

interface Shape { fun area(): Double }
来源：http://hz.kuanghao11.cn/gtphfxolxc.html

[T16] Swift：Hello World
来源：http://hz.kuanghao11.cn/gtqkzwdiwk.html

print("Hello")
来源：http://hz.zhengqikj.top/gtlgrzeqzt.html

[T17] Swift：变量与常量
来源：http://hz.ybcxt.top/gthxtzutqp.html

var a = 1;  let b = 2
来源：http://hz.zdqjudy.top/gttxzsbhik.html

[T18] Swift：字符串插值
来源：http://hz.aizwys.cn/gtrmgnvtva.html

"值: \(b)"
来源：http://hz.chenlongwang.top/gtltvxskcn.html

[T19] Swift：可选绑定
来源：http://hz.zycfv.cn/gtydxkknjp.html

if let n = opt { print(n) }
来源：http://hz.fzhhl.top/gtupmajcyd.html

[T20] Swift：数组操作
来源：http://hz.mhx1999.top/gtzivyjwgg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zycfv.cn/gtaiegwbzp.html

[T21] Swift：遍历
来源：http://hz.yj202588.top/gthpdtmeif.html

for x in a { print(x) }
来源：http://hz.yj20258.top/gtnotbwrkb.html

[T22] Swift：字典
来源：http://hz.jqgfzy.top/gtwnsyhyei.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.redwolf501.top/gtvdxkckwp.html

[T23] Swift：函数
来源：http://hz.daria6918.cn/gtumrdjjip.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.wangdashe.top/gtjaqqombl.html

[T24] Swift：闭包
来源：http://hz.dianchejie.cn/gtbodlihcw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.dashuyun.cn/gtqlgqgtwv.html

[T25] Swift：结构体
来源：http://hz.cashguo.top/gtjaswggpy.html

struct P { var x: Int }
来源：http://hz.xuetiantiany.cn/gtjkeqcpgr.html

[T26] Swift：类与重写
来源：http://hz.shuidangran.top/gtdjnzogsw.html

class A: Base { override func f() {} }
来源：http://hz.shzxlz.cn/gtxlpkavru.html

[T27] Swift：错误处理
来源：http://hz.0kj1m.cn/gtsmncfmwl.html

do { try f() } catch { print(error) }
来源：http://hz.yuxming.cn/gtxebooiin.html

[T28] Swift：枚举
来源：http://hz.iojbl.cn/gtaowrvyfx.html

enum Color { case red, green }
来源：http://hz.quarkkingdee.top/gtmiondfpw.html

[T29] Swift：guard 提前返回
来源：http://hz.ppjwa.cn/gtjcqzuxji.html

guard let x = opt else { return }
来源：http://hz.cashguo.top/gtflawkdtj.html

[T30] Swift：协议
来源：http://hz.xingfuxueyuan.xyz/gtvpwwxyyp.html

protocol Shape { func area() -> Double }
来源：http://hz.yuanzhike.top/gtwvcsqbtc.html

[T31] Lua：Hello World
来源：http://hz.cdnleiting.top/gtusisemvb.html

print("Hello")
来源：http://hz.52xcode.cn/gtzuozgbdu.html

[T32] Lua：局部变量
来源：http://hz.sweek.top/gtfqsdimsg.html

local a = 1
来源：http://hz.zhiwuduotai.top/gtxwseeqcq.html

[T33] Lua：表（数组）
来源：http://hz.shanyushiyangkeji.top/gtpizdyghl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.meibo888.top/gtgjvrlsru.html

[T34] Lua：遍历表
来源：http://hz.jianghu66.top/gtuahollgc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.tianlin.xyz/gtywmbtmjd.html

[T35] Lua：字典表
来源：http://hz.cdnleiting.top/gtsfrlfemb.html

local d = { a = 1 };  d.b = 2
来源：http://hz.feifeiyinyue.top/gtebcpodsa.html

[T36] Lua：函数
来源：http://hz.mhx1999.top/gtiqppmqjg.html

function add(a, b) return a + b end
来源：http://hz.tanke756.top/gtjkitbuxr.html

[T37] Lua：字符串拼接
来源：http://hz.zhoulong.xyz/gtjrvwzevs.html

"a" .. "b"
来源：http://hz.zhengqikj.top/gtrtmgdqml.html

[T38] Lua：条件
来源：http://hz.yvedp.cn/gtlaeqbful.html

if x > 0 then print("正") end
来源：http://hz.bjfxy.top/gtzldpcget.html

[T39] Lua：模式匹配
来源：http://hz.redwolf501.top/gtmxqlmqne.html

string.find(s, "%d+")
来源：http://hz.sxryk.cn/gtmunqawhz.html

[T40] Lua：元表
来源：http://hz.jinghuilouyu.cn/gtghscbgry.html

setmetatable({}, { __index = base })
来源：http://hz.jqgfzy.top/gtzhoczsau.html


<!-- 参考信息 -->