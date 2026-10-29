代发 wailian999

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/ghoajbzjx.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gafelmvyi.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gydkybtta.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gabmuhyuu.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gustppsyh.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gcrovugqf.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gwxhobrdv.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gtsuzciwp.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gxywprgga.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/glbobkdkq.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/grzjxmyvt.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gtptmzhhm.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/giiauwbbg.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/glbpyyvwq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gnoiyojrt.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gieqdogku.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gferbhvqs.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/geiwcnfuo.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gfjmbveyg.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gecsjmgzy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gdybujifk.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gmmhnsmej.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/glmubfaxt.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gmopnqgox.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gradgrbwl.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gddmmbmpc.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gqfhmcowg.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/grtavpgxk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gbethnlgs.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gjuodbawv.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gsjlvnzvv.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gcrrjwpzp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gknalfjdt.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gzbucvxxr.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gcgnaqrbh.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gqogtsyxn.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gxkdydcnp.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gixqqhpau.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gblvpnngy.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gewlbeirr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gpdtrvaup.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/govrpjukq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gkkugfgkf.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gqkeogkpu.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gmjjfasfw.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gkxkwkhwm.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gxyrwqeun.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gdgbwcjta.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/ggzjsdjnt.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gdunqzfpj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/grnlxaiyz.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gskxoldxh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gaxaowbpb.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gxigcrmdz.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gimlewhmw.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/garoyjwqc.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gxzvqxlad.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gyfcndspt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gujajalvn.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gpqxubftd.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gtjjdkzio.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gqlggvurn.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gmscscdkz.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/guhaeodwq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gbovxzpmu.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gdjqpmgma.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/guruwlsez.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/giuohdkgn.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gvhvgjkgo.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/geiruvbhz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gkwzodvie.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gvmibqnft.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gyzohgtat.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gmrwtzplz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/guvxygbjx.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gfjfgbgvg.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gsspuozfv.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gqdsydxpn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/grideykny.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gzhdmfwxd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gbnpjiwey.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/grexyrwaq.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/ggjzugzlr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxbpehdgi.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gvtfoobii.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glhkpqfaj.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gtkkjnyfs.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/goselarjt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gwcbxlvny.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gpxkdlljb.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gflcatgfl.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gjvqwcvat.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/geitjigoc.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/geuxxvddk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/guejjkjqe.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/guodbdxmf.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkbxumdvd.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gdxhuuzwy.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/grlrgyajq.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gvlvnqvmt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gvzhwjsou.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gyyvtycjz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gwfzxwmuy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/grqlaawer.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gosybgixx.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gtsgdkgiz.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gpddnsjje.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gfmgyrdnf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gmxortgqs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gvnqomgdz.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gupnvwnjq.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gaastwpfm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gdfiowskv.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gzcijttxx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/ggauscknp.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gdqkaixkw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/glepqarse.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gxnjbqcbk.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gbtcstzqv.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/grgmpruoz.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gyrtllhle.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gspapkugk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gwgnndeld.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gvafspvhd.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gfrxocnia.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gfrhuwtjg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gzdafopuc.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gkevksxis.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/ghkwmqdkp.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gwraycbdw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gkjumkfip.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gvpbenpro.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/guqnpqwgy.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/giofduntx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gctysdkoh.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gdjluprrd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gqvbasgob.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/grchchvjs.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gkgidkppo.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/guojomzts.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gkrgnoszr.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gzhzwjnnt.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gtlvowtix.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/grixudzfj.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gfnhlpyep.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gnbjsujqt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/ggigataqi.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gcvontitl.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gnefxrlqo.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gjfhwwbdp.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/ggieygxcq.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gxdrkfady.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gwpwkatva.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gbwgysvqc.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gleshouhs.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gtymtfjul.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gevdnuufa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gunpyedrz.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/glsdntmso.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gnjgppkkw.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gxlndyazk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gnxbeiika.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/glelgoiqq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gauhploot.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gqagxilzr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gqhrbhehs.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gvcjpotqg.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/ghgkwtlne.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gaqyaafnq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gvgusaqvf.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gklliofko.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gqgifafbq.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gxdipexjg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gcisjhvwg.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gljhudcmc.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/giowvkwef.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/ggqgzboba.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gxprzkzwf.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gtwmmnukt.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gexuqkgpk.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gchynaslm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gjmadzqdo.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gybdbopvx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gjvouxmuj.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gtnbsgjna.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gvypxkyfv.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gvvuidksf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/glysmocna.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gnphrvvmw.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gpflpftqs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gstudhjww.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gmcwgjemj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gpoecbfxc.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gaeboyovm.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gywtpsyor.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gqflxnhmz.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/ghrmggomc.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gccsenros.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gmsnbjics.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gfgsxlpik.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gbxcqltxy.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gyouxckic.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gwzcapqzf.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/ghodiohsv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gaqtzxcwt.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gttvbiyap.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gydxccemp.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/ghrwkolsk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gilomqnym.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gpsdildze.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gxkukfhdh.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/ghbgyhxvm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/ghncwvwwx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyueyockq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/ggagsprtr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghqyeansz.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gmwttauxi.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gqqgwxuaw.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gcfifvlpl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gudyyemms.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gffdbpnnf.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gqohvvysl.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gujsemmti.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/ggcvnsaav.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gbxmteygq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gxxsojqfk.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/guzfuzpfg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gauxtifub.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gdhvijcnx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gfbamuahj.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/guxbrdzeu.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/ggpomzbiw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/galrpfqzj.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gxxcstiuo.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gcdncsisy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gsmmszghl.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gbxbzsbjs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gsgnupiuk.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/ghpodzdpv.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gevldgewb.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gtkzuuejb.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gufbqwuuz.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/ggheqohsf.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gdivhhsfa.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gfgvnkhug.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gzxjhshmp.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gxukdrart.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gmsyckklf.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/grlwkohhk.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/geeaotxwv.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gcmlxtcss.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gsttnzcvt.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gdykkmuru.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gsavvqvpg.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gwcjnukhn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/glsqkicps.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gwxktbsov.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gkddiumir.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gmdhfarsm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/guynqihvb.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gqrarrpzq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/grhpodydf.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gspccugas.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gladgzmmd.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/ggbfyiapb.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gpidduucq.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gudactqym.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gcscozkmv.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gutwpvqeu.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/grplmhcum.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gvfxhsroa.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gcufmcmqz.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/ggvgqrcda.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gzsyioszk.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gexfgfblh.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gturgxagf.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gympfjowv.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gnrzodcok.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/ggzukpvuw.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gdeyruijg.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gnevivjcr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/ggnxqepfs.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gjlwgfwvn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gbzkiuqew.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/grjjwthgm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gkhdrarnb.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/ghijtmjdf.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gumrkakon.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/ggrlzbvxu.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gjqjfgbxu.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gqfqkhhht.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/glvrgtkzu.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gywndznqo.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gwhwwczxd.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gmunnlbxb.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gwedxwjix.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gxpzkocmz.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gcmpjbulf.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gatjvgffx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gcxsjzsit.sHtML


<!-- 参考信息 -->